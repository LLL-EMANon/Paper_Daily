# Daily Papers - 2026-03-10

**Topic**: deep learning  
**Filter**: last 7 days
**Count**: 10

---

## 1. BEVLM: Distilling Semantic Knowledge from LLMs into Bird's-Eye View Representations

**Meta**
- Authors: Thomas Monninger, Shaoyuan Xie, Qi Alfred Chen, Sihao Ding
- Published: 2026-03-07
- arXiv: https://arxiv.org/abs/2603.06576v1

**Abstract**
The integration of Large Language Models (LLMs) into autonomous driving has attracted growing interest for their strong reasoning and semantic understanding abilities, which are essential for handling complex decision-making and long-tail scenarios. However, existing methods typically feed LLMs with tokens from multi-view and multi-frame images independently, leading to redundant computation and limited spatial consistency. This separation in visual processing hinders accurate 3D spatial reasoning and fails to maintain geometric coherence across views. On the other hand, Bird's-Eye View (BEV) representations learned from geometrically annotated tasks (e.g., object detection) provide spatial structure but lack the semantic richness of foundation vision encoders. To bridge this gap, we propose BEVLM, a framework that connects a spatially consistent and semantically distilled BEV representation with LLMs. Through extensive experiments, we show that BEVLM enables LLMs to reason more effectively in cross-view driving scenes, improving accuracy by 46%, by leveraging BEV features as unified inputs. Furthermore, by distilling semantic knowledge from LLMs into BEV representations, BEVLM significantly improves closed-loop end-to-end driving performance by 29% in safety-critical scenarios.

---

## 2. An ode to instantons

**Meta**
- Authors: Oliver Janssen, Joel Karlsson, Flavio Riccardi, Mattia Varrone
- Published: 2026-03-07
- arXiv: https://arxiv.org/abs/2603.06575v1

**Abstract**
We present a formalism for semiclassical time evolution in quantum mechanics, building on a century of work. We identify complex saddle points in real time, real saddle points in complex time, and complex saddle points in complex time that reproduce the known answers in classic problems. For the decay of a metastable state, we find finite time and finite energy analogs of the "bounce" which do not have strict zero or negative modes. The one-loop phase of the wave function and the multiplicity of bounce solutions at late times are discussed. The motivation of this work is to learn how to compute decay rates in quantum field theory in situations with non-trivial time dependence, by first taking a humble step backwards to the fascinating world of quantum mechanics.

---

## 3. SCOPE: Scene-Contextualized Incremental Few-Shot 3D Segmentation

**Meta**
- Authors: Vishal Thengane, Zhaochong An, Tianjin Huang, Son Lam Phung, Abdesselam Bouzerdoum, Lu Yin, Na Zhao, Xiatian Zhu
- Published: 2026-03-07
- arXiv: https://arxiv.org/abs/2603.06572v1

**Abstract**
Incremental Few-Shot (IFS) segmentation aims to learn new categories over time from only a few annotations. Although widely studied in 2D, it remains underexplored for 3D point clouds. Existing methods suffer from catastrophic forgetting or fail to learn discriminative prototypes under sparse supervision, and often overlook a key cue: novel categories frequently appear as unlabelled background in base-training scenes. We introduce SCOPE (Scene-COntextualised Prototype Enrichment), a plug-and-play background-guided prototype enrichment framework that integrates with any prototype-based 3D segmentation method. After base training, a class-agnostic segmentation model extracts high-confidence pseudo-instances from background regions to build a prototype pool. When novel classes arrive with few labelled samples, relevant background prototypes are retrieved and fused with few-shot prototypes to form enriched representations without retraining the backbone or adding parameters. Experiments on ScanNet and S3DIS show that SCOPE achieves SOTA performance, improving novel-class IoU by up to 6.98% and 3.61%, and mean IoU by 2.25% and 1.70%, respectively, while maintaining low forgetting. Code is available https://github.com/Surrey-UP-Lab/SCOPE.

---

## 4. Penguin-VL: Exploring the Efficiency Limits of VLM with LLM-based Vision Encoders

**Meta**
- Authors: Boqiang Zhang, Lei Ke, Ruihan Yang, Qi Gao, Tianyuan Qu, Rossell Chen, Dong Yu, Leoweiliang
- Published: 2026-03-07
- arXiv: https://arxiv.org/abs/2603.06569v1

**Abstract**
Vision Language Model (VLM) development has largely relied on scaling model size, which hinders deployment on compute-constrained mobile and edge devices such as smartphones and robots. In this work, we explore the performance limits of compact (e.g., 2B and 8B) VLMs. We challenge the prevailing practice that state-of-the-art VLMs must rely on vision encoders initialized via massive contrastive pretraining (e.g., CLIP/SigLIP). We identify an objective mismatch: contrastive learning, optimized for discrimination, enforces coarse and category-level invariances that suppress fine-grained visual cues needed for dense captioning and complex VLM reasoning. To address this issue, we present Penguin-VL, whose vision encoder is initialized from a text-only LLM. Our experiments reveal that Penguin-Encoder serves as a superior alternative to traditional contrastive pretraining, unlocking a higher degree of visual fidelity and data efficiency for multimodal understanding. Across various image and video benchmarks, Penguin-VL achieves performance comparable to leading VLMs (e.g., Qwen3-VL) in mathematical reasoning and surpasses them in tasks such as document understanding, visual knowledge, and multi-perspective video understanding. Notably, these gains are achieved with a lightweight architecture, demonstrating that improved visual representation rather than model scaling is the primary driver of performance. Our ablations show that Penguin-Encoder consistently outperforms contrastive-pretrained encoders, preserving fine-grained spatial and temporal cues that are critical for dense perception and complex reasoning. This makes it a strong drop-in alternative for compute-efficient VLMs and enables high performance in resource-constrained settings. Code: https://github.com/tencent-ailab/Penguin-VL

---

## 5. A recipe for scalable attention-based MLIPs: unlocking long-range accuracy with all-to-all node attention

**Meta**
- Authors: Eric Qu, Brandon M. Wood, Aditi S. Krishnapriyan, Zachary W. Ulissi
- Published: 2026-03-07
- arXiv: https://arxiv.org/abs/2603.06567v1

**Abstract**
Machine-learning interatomic potentials (MLIPs) have advanced rapidly, with many top models relying on strong physics-based inductive biases. However, as models scale to larger systems like biomolecules and electrolytes, they struggle to accurately capture long-range (LR) interactions, leading current approaches to rely on explicit physics-based terms or components. In this work, we propose AllScAIP, a straightforward, attention-based, and energy-conserving MLIP model that scales to O(100 million) training samples. It addresses the long-range challenge using an all-to-all node attention component that is data-driven. Extensive ablations reveal that in low-data/small-model regimes, inductive biases improve sample efficiency. However, as data and model size scale, these benefits diminish or even reverse, while all-to-all attention remains critical for capturing LR interactions. Our model achieves state-of-the-art energy/force accuracy on molecular systems, as well as a number of physics-based evaluations (OMol25), while being competitive on materials (OMat24) and catalysts (OC20). Furthermore, it enables stable, long-timescale MD simulations that accurately recover experimental observables, including density and heat of vaporization predictions.

---

## 6. Boosting deep Reinforcement Learning using pretraining with Logical Options

**Meta**
- Authors: Zihan Ye, Phil Chau, Raban Emunds, Jannis Blüml, Cedric Derstroff, Quentin Delfosse, Oleg Arenz, Kristian Kersting
- Published: 2026-03-07
- arXiv: https://arxiv.org/abs/2603.06565v1

**Abstract**
Deep reinforcement learning agents are often misaligned, as they over-exploit early reward signals. Recently, several symbolic approaches have addressed these challenges by encoding sparse objectives along with aligned plans. However, purely symbolic architectures are complex to scale and difficult to apply to continuous settings. Hence, we propose a hybrid approach, inspired by humans' ability to acquire new skills. We use a two-stage framework that injects symbolic structure into neural-based reinforcement learning agents without sacrificing the expressivity of deep policies. Our method, called Hybrid Hierarchical RL (H^2RL), introduces a logical option-based pretraining strategy to steer the learning policy away from short-term reward loops and toward goal-directed behavior while allowing the final policy to be refined via standard environment interaction. Empirically, we show that this approach consistently improves long-horizon decision-making and yields agents that outperform strong neural, symbolic, and neuro-symbolic baselines.

---

## 7. Convergence of Neural Network Policies for Risk--Reward Optimization

**Meta**
- Authors: Chang Chen, Duy-Minh Dang
- Published: 2026-03-07
- arXiv: https://arxiv.org/abs/2603.06563v1

**Abstract**
We develop a neural-network framework for multi-period risk--reward stochastic control problems with constrained two-step feedback policies that may be discontinuous in the state. We allow a broad class of objectives built on a finite-dimensional performance vector, including terminal and path-dependent statistics, with risk functionals admitting auxiliary-variable optimization representations (e.g.\ Conditional Value-at-Risk and buffered probability of exceedance) and optional moment dependence. Our approach parametrizes the two-step policy using two coupled feedforward networks with constraint-enforcing output layers, reducing the constrained control problem to unconstrained training over network parameters. Under mild regularity conditions, we prove that the empirical optimum of the NN-parametrized objective converges in probability to the true optimal value as network capacity and training sample size increase. The proof is modular, separating policy approximation, propagation through the controlled recursion, and preservation under the scalarized risk--reward objective. Numerical experiments confirm the predicted convergence-in-probability behavior, show close agreement between learned and reference control heat maps, and demonstrate out-of-sample robustness on a large independent scenario set.

---

## 8. EgoReasoner: Learning Egocentric 4D Reasoning via Task-Adaptive Structured Thinking

**Meta**
- Authors: Fangrui Zhu, Yunfeng Xi, Jianmo Ni, Mu Cai, Boqing Gong, Long Zhao, Chen Qu, Ian Miao, Yi Li, Cheng Zhong, Huaizu Jiang, Shwetak Patel
- Published: 2026-03-07
- arXiv: https://arxiv.org/abs/2603.06561v1

**Abstract**
Egocentric video understanding is inherently complex due to the dynamic 4D nature of the environment, where camera motion and object displacements necessitate a continuous re-evaluation of spatial relations. In this work, we target a suite of under-explored egocentric 4D reasoning tasks, including fixture interaction counting, viewpoint-relative fixture location, object movement itinerary tracking, and stationary object localization, that require fundamentally different cognitive operations: spatial anchoring, temporal tracking, and duration reasoning. We observe that these structural differences make task-agnostic approaches insufficient: generic Chain-of-Thought methods lack task-appropriate reasoning primitives, and uniform reinforcement learning actively destabilizes performance on spatial tasks. To address this, we propose EgoReasoner, a two-stage framework that aligns both the reasoning scaffold and the reward signal to each task's cognitive structure. In the first stage, Task-Adaptive Thinking Templates guide the synthesis of structured CoT traces that teach the model to reason adaptively across task types via supervised fine-tuning. In the second stage, task-aware reward functions verify entity grounding, temporal alignment, and task-adaptive logical consistency, selectively strengthening each reasoning pathway via reinforcement fine-tuning with GRPO. Our 3B-parameter model, trained on only 16K samples, achieves 37.5% average accuracy on the challenging HD-EPIC benchmark, surpassing Qwen2.5-VL-7B (25.7%) by over 10 points.

---

## 9. Causal Interpretation of Neural Network Computations with Contribution Decomposition

**Meta**
- Authors: Joshua Brendan Melander, Zaki Alaoui, Shenghua Liu, Surya Ganguli, Stephen A. Baccus
- Published: 2026-03-07
- arXiv: https://arxiv.org/abs/2603.06557v1

**Abstract**
Understanding how neural networks transform inputs into outputs is crucial for interpreting and manipulating their behavior. Most existing approaches analyze internal representations by identifying hidden-layer activation patterns correlated with human-interpretable concepts. Here we take a direct approach to examine how hidden neurons act to drive network outputs. We introduce CODEC (Contribution Decomposition), a method that uses sparse autoencoders to decompose network behavior into sparse motifs of hidden-neuron contributions, revealing causal processes that cannot be determined by analyzing activations alone. Applying CODEC to benchmark image-classification networks, we find that contributions grow in sparsity and dimensionality across layers and, unexpectedly, that they progressively decorrelate positive and negative effects on network outputs. We further show that decomposing contributions into sparse modes enables greater control and interpretation of intermediate layers, supporting both causal manipulations of network output and human-interpretable visualizations of distinct image components that combine to drive that output. Finally, by analyzing state-of-the-art models of neural activity in the vertebrate retina, we demonstrate that CODEC uncovers combinatorial actions of model interneurons and identifies the sources of dynamic receptive fields. Overall, CODEC provides a rich and interpretable framework for understanding how nonlinear computations evolve across hierarchical layers, establishing contribution modes as an informative unit of analysis for mechanistic insights into artificial neural networks.

---

## 10. Hierarchical Industrial Demand Forecasting with Temporal and Uncertainty Explanations

**Meta**
- Authors: Harshavardhan Kamarthi, Shangqing Xu, Xinjie Tong, Xingyu Zhou, James Peters, Joseph Czyzyk, B. Aditya Prakash
- Published: 2026-03-07
- arXiv: https://arxiv.org/abs/2603.06555v1

**Abstract**
Hierarchical time-series forecasting is essential for demand prediction across various industries. While machine learning models have obtained significant accuracy and scalability on such forecasting tasks, the interpretability of their predictions, informed by application, is still largely unexplored. To bridge this gap, we introduce a novel interpretability method for large hierarchical probabilistic time-series forecasting, adapting generic interpretability techniques while addressing challenges associated with hierarchical structures and uncertainty. Our approach offers valuable interpretative insights in response to real-world industrial supply chain scenarios, including 1) the significance of various time-series within the hierarchy and external variables at specific time points, 2) the impact of different variables on forecast uncertainty, and 3) explanations for forecast changes in response to modifications in the training dataset. To evaluate the explainability method, we generate semi-synthetic datasets based on real-world scenarios of explaining hierarchical demands for over ten thousand products at a large chemical company. The experiments showed that our explainability method successfully explained state-of-the-art industrial forecasting methods with significantly higher explainability accuracy. Furthermore, we provide multiple real-world case studies that show the efficacy of our approach in identifying important patterns and explanations that help stakeholders better understand the forecasts. Additionally, our method facilitates the identification of key drivers behind forecasted demand, enabling more informed decision-making and strategic planning. Our approach helps build trust and confidence among users, ultimately leading to better adoption and utilization of hierarchical forecasting models in practice.

---
