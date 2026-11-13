# 临界指数 · 方法与计算

[返回主页](../README.md) · [GitHub 项目](https://github.com/Moonyear817/criticality-index) · [方法说明](https://github.com/Moonyear817/criticality-index/blob/main/docs/method.md)

一家店的经营能力受损到什么程度？这个试行框架以六个系统的档位、致命条件与证据范围描述当前状态。

**公开内容**　方法说明 · 六系统判据 · 模拟算例 · 评估模板 · Python 精确计算器 · 形式枚举

## 制作过程

### 先定义对象与证据

固定评估对象、时点和观察范围，分别核对现金、业务与收入、交付、团队、治理、必要经营条件。未知单独记录，不填成零。

### 拆开致命、状态与未知

已核实致命直接为 100；致命未知或资料未复核时待补证。仅档位或作用链未定时，报告与证据相容的可行范围。

### 比较 A 与 B

A 允许叠加升档；当前推荐 B 保留最高档优先，在档内反映其余问题。公开文档用同一组构造输入演示两种规则的取舍。

### 用代码复算

从已有书稿与数学工作稿整理公开说明，使用 Fraction 实现精确计算；8 项测试通过，包括全部 62,425 个可行形式状态的基本性质与单步单调性。算例与检查可在仓库内自行运行。

## 当前边界

本项目是研究中的方法原型，尚未完成多案例实证验证。分数不表示倒闭概率或剩余寿命；形式状态计数也不是真实企业样本量。公开版使用构造算例，真实案例材料留在私有项目中。

---

An experimental framework for describing impairment of operating capacity, with methods, criteria, constructed examples, an exact Python calculator and formal rule checks. The currently preferred B rule preserves highest-tier priority; A remains a comparison. Formal checks do not establish predictive validity.
