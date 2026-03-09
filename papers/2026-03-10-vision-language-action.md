# 📚 每日论文速递 - 2026-03-10

**研究方向**: vision-language-action models, deep learning, robotics, world models  
**筛选条件**: 顶会顶刊 (CCF-A / CORE A* / CORE A)  
**论文数量**: 2

---

## 1. A Survey on Vision-Language-Action Models: An Action Tokenization Perspective

**基本信息**
- 作者：Yifan Zhong, Fengshuo Bai, Shaofei Cai, Xuchuan Huang, Zhang Chen, Xiaowei Zhang, Yuanfei Wang, Shaoyang Guo, Tianrui Guan, Ka Nam Lui, Zhiquan Qi, Yitao Liang, Yuanpei Chen, Yaodong Yang
- 发布：2025-07-02
- 会议/期刊：arXiv preprint (Preprint)
- 引用数：0 📈
- arXiv: [arXiv ID](https://arxiv.org/abs/2507.01925)

**主要贡献**
- 提出了 VLA 模型的统一框架，将看似不同的方法整合到一个共同范式下
- 建立了动作 token 的分类体系，涵盖语言描述、代码、功能、轨迹、目标状态、潜在表示、原始动作和推理等 8 种类型
- 系统性地梳理了现有 VLA 研究，分析了每种 token 类型的优缺点

**方法**
- 统一框架：视觉和语言输入通过一系列 VLA 模块处理，产生动作 token 链，逐步编码更接地气的可行动信息
- 动作 token 分类学：从表达能力和应用场景两个维度对不同类型的动作 token 进行系统分类
- 架构趋势分析：提出分层架构设计，顶层使用语言描述和代码进行长程规划，底层集成视频预测、流建模和 3D 交互预测

**实验**
- 综述覆盖了当前主要的 VLA 模型和方法
- 提供了详细的动作 token 类型对比分析
- 指出了各类型 token 的适用场景和局限性

**结论**
- VLA 模型的未来不在于单一主导的动作 token，而在于不同类型 token 的战略合成
- 语言 motion 表达能力有限，不太可能成为主流；语言计划对于任务分解仍然至关重要
- 代码作为强有力的替代方案，需要构建综合函数库来整合感知和行动原语
- 功能（affordances）和轨迹（trajectories）之间形成关键协同，world models 可以支持这种协同
- 有效的 VLA 模型应采用分层架构，顶层进行长程规划和逻辑控制

---

## 2. Vision-Language-Action (VLA) Models: Concepts, Progress, Applications and Challenges

**基本信息**
- 作者：Ranjan Sapkota, Sagar Bhattarai, Minh-Triet Tran
- 发布：2025-05-07 (v2: 2026-01-29)
- 会议/期刊：arXiv preprint (Preprint)
- 引用数：0 📈
- arXiv: [arXiv ID](https://arxiv.org/abs/2505.04769)

**主要贡献**
- 全面综述了 VLA 模型在过去三年的发展，覆盖超过 80 个 VLA 模型
- 系统性地组织了五个主题支柱：概念基础、进展、应用、挑战和未来方向
- 提出了针对实时控制、多模态动作表示、系统可扩展性等挑战的解决方案

**方法**
- 概念基础：追溯 VLA 系统从跨模态学习架构到通用智能体的演变
- 架构创新：分析参数高效训练策略和实时推理加速技术
- 应用探索：涵盖人形机器人、自动驾驶车辆、医疗和工业机器人、精准农业、AR 导航等领域

**实验**
- 详细比较了不同 VLA 模型的架构设计和训练方法
- 评估了各模型在不同应用场景中的表现
- 分析了数据集偏差、泛化能力和系统集成的复杂性

**结论**
- VLA 模型标志着人工智能的变革性进步，旨在将感知、自然语言理解和具身行动统一在一个计算框架内
- 未来的发展方向包括：智能体 AI 适应、跨形态泛化、统一神经符号规划
- VLA 模型、VLM 和智能体 AI 将融合以推动社会对齐、自适应和通用具身智能体发展
- 需要在实时推理约束、多模态动作表示和安全保障方面继续突破

---

**报告生成时间**: 2026-03-10  
**数据来源**: arXiv, Semantic Scholar
