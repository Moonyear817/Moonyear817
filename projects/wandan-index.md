# 持续经营脆弱性指数（GCVI）

Going-Concern Vulnerability Index

[返回主页](../README.md) · [计算实现](https://github.com/Moonyear817/gcvi) · [方法文档](https://github.com/Moonyear817/gcvi/blob/main/docs/method.md)

## 研究概述

GCVI 是面向小型商业组织的持续经营状态测度框架。研究以六维经营状态为输入，在非补偿性约束下结合风险聚合与致命否决，并通过可行状态枚举处理不完全信息。指数描述既定对象、时点与证据范围内的经营能力受损状态。

## 方法结构

1. **状态空间界定**：对现金、业务与收入、交付、团队、治理及必要经营条件进行五级离散编码，保留分档依据和缺失信息。
2. **致命否决与聚合**：已核实的致命条件优先于非致命合成；比较允许风险叠加升档的 A 与保持最高严重档优先的 B，当前采用 B。
3. **区间识别**：致命未知或证据未复核时不发布点值；在致命已排除的条件下，对未定输入枚举可行补全并报告上下界。
4. **可复现计算**：使用有理数算术实现聚合和取整，提供构造算例、评估模板、测试及形式状态枚举脚本。

## 校核与研究边界

8 项测试已通过；全部 62,425 个可行形式状态上的基本边界、单项保真、单步单调性与 B 的档位区间已校核。该计数不是企业样本量，形式校核不构成预测效度证据。

分档可靠性、参数适用性与外部效度仍需经验研究。指数不解释为破产概率或剩余存续期限。公开版提供构造算例，个案材料保留在私有项目中。

---

GCVI is a framework for measuring the current vulnerability of small commercial organizations to loss of going-concern capacity. It combines discrete operating states, non-compensatory constraints, fatal-condition vetoes and interval identification under incomplete information. The public implementation includes exact arithmetic and exhaustive finite-state checks; empirical validity remains to be established.
