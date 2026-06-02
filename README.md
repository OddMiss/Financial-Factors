中文 | [English](README_EN.md)

# Financial-Factors

基于财报与行情数据的财务因子研究与计算笔记。本仓库以沪深 300 成分股为示例，包含从财报数据计算各类财务因子、因子增量/全量计算流程、以及因子脚本与测试框架的整理。

## 仓库内容

- `财报因子v1.ipynb` ~ `财报因子v4.ipynb`：财报因子计算的迭代版本，包含因子计算逻辑与注意事项。
- `财务因子v0.ipynb`：早期版本的财务因子计算探索。
- `脚本因子代码测试框架.ipynb`：因子脚本与测试用例的模板框架。
- `Name-Table.ipynb`：财务字段与字典说明整理。
- `Financial Analysis Framework.png`：财务分析框架示意图。
- 参考论文：`The Journal of Finance - June 1992 - FAMA - The Cross‐Section of Expected Stock Returns.pdf`、`Do-investors-overvalue-firms-with-bloated-balance-sheets.pdf`

## 主要特性

- **财报因子计算**：从资产负债表、利润表、现金流等数据提取并计算常见财务因子。
- **增量与全量计算**：`财报因子v4.ipynb`整合了增量计算模块与全量计算模块。
- **数据处理细节**：处理季度累计值、公告日期、缺失值、对齐顺序等问题。
- **脚本化与测试**：提供因子脚本与测试框架模板，便于扩展与验证。

## 环境依赖

该仓库主要以 Jupyter Notebook 形式组织，依赖常见的 Python 数据分析库与行情/财务数据接口，典型依赖包括：

- Python 3.x
- numpy、pandas
- statsmodels、matplotlib、seaborn
- `cylib` 与 `xtdata`（用于获取行情与财报数据的外部接口）

> 由于 `cylib` 与 `xtdata` 为外部数据接口，请根据本地数据环境自行安装与配置。

## 使用方式

1. 准备好可用的行情与财报数据接口（例如 `xtdata`）。
2. 选择目标 Notebook（推荐从 `财报因子v4.ipynb` 开始）。
3. 按 Notebook 内的参数说明设置 `trade_date`、`start_date` 等关键参数。
4. 运行 Notebook 进行因子计算或验证。

## 备注

- 多数 Notebook 以 **HS300** 为示例。
- 数据口径与字段含义参考 `Name-Table.ipynb` 及外部字典链接。

## 参考资料

- Fama, E. F., & French, K. R. (1992). The Cross‑Section of Expected Stock Returns. *The Journal of Finance*, 47(2), 427–465.
- Hirshleifer, D., Hou, K., Teoh, S. H., & Zhang, Y. (2004). Do Investors Overvalue Firms with Bloated Balance Sheets? *Journal of Accounting and Economics*, 38, 297–331.
