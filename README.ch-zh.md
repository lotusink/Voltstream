[English](README.md)|[中文简体](README.ch-zh.md)

# **VoltStream：流式电力负荷预测框架**

VoltStream 是一个基于 Apache Spark 与 Kafka 构建的实时电力负荷预测框架，面向智能电网应用。
项目融合了 多源数据（包括实时功率采样、气象信息与建筑属性），以提升预测精度与模型鲁棒性。
系统实现了 分布式模型训练与流式预测推理，支持可扩展、低延迟、动态更新的能量预测。

具体信息参考[项目文档](Document/README.ch-zh.md)

**技术栈：** Spark · Kafka · Python · 机器学习 · 随机森林 · 梯度提升树