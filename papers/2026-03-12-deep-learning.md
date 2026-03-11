# Daily Papers - 2026-03-12

**Topic**: deep learning  
**Filter**: last 7 days
**Count**: 10

---

## 1. Task Aware Modulation Using Representation Learning for Upsaling of Terrestrial Carbon Fluxes

**Meta**
- Authors: Aleksei Rozanov, Arvind Renganathan, Vipin Kumar
- Published: 2026-03-11
- arXiv: https://arxiv.org/abs/2603.09974v1

**Abstract**
Accurately upscaling terrestrial carbon fluxes is central to estimating the global carbon budget, yet remains challenging due to the sparse and regionally biased distribution of ground measurements. Existing data-driven upscaling products often fail to generalize beyond observed domains, leading to systematic regional biases and high predictive uncertainty. We introduce Task-Aware Modulation with Representation Learning (TAM-RL), a framework that couples spatio-temporal representation learning with knowledge-guided encoder-decoder architecture and loss function derived from the carbon balance equation. Across 150+ flux tower sites representing diverse biomes and climate regimes, TAM-RL improves predictive performance relative to existing state-of-the-art datasets, reducing RMSE by 8-9.6% and increasing explained variance ($R^2$) from 19.4% to 43.8%, depending on the target flux. These results demonstrate that integrating physically grounded constraints with adaptive representation learning can substantially enhance the robustness and transferability of global carbon flux estimates.

---

## 2. From Data Statistics to Feature Geometry: How Correlations Shape Superposition

**Meta**
- Authors: Lucas Prieto, Edward Stevinson, Melih Barsbey, Tolga Birdal, Pedro A. M. Mediano
- Published: 2026-03-11
- arXiv: https://arxiv.org/abs/2603.09972v1

**Abstract**
A central idea in mechanistic interpretability is that neural networks represent more features than they have dimensions, arranging them in superposition to form an over-complete basis. This framing has been influential, motivating dictionary learning approaches such as sparse autoencoders. However, superposition has mostly been studied in idealized settings where features are sparse and uncorrelated. In these settings, superposition is typically understood as introducing interference that must be minimized geometrically and filtered out by non-linearities such as ReLUs, yielding local structures like regular polytopes. We show that this account is incomplete for realistic data by introducing Bag-of-Words Superposition (BOWS), a controlled setting to encode binary bag-of-words representations of internet text in superposition. Using BOWS, we find that when features are correlated, interference can be constructive rather than just noise to be filtered out. This is achieved by arranging features according to their co-activation patterns, making interference between active features constructive, while still using ReLUs to avoid false positives. We show that this kind of arrangement is more prevalent in models trained with weight decay and naturally gives rise to semantic clusters and cyclical structures which have been observed in real language models yet were not explained by the standard picture of superposition. Code for this paper can be found at https://github.com/LucasPrietoAl/correlations-feature-geometry.

---

## 3. TiPToP: A Modular Open-Vocabulary Planning System for Robotic Manipulation

**Meta**
- Authors: William Shen, Nishanth Kumar, Sahit Chintalapudi, Jie Wang, Christopher Watson, Edward Hu, Jing Cao, Dinesh Jayaraman, Leslie Pack Kaelbling, Tomás Lozano-Pérez
- Published: 2026-03-11
- arXiv: https://arxiv.org/abs/2603.09971v1

**Abstract**
We present TiPToP, an extensible modular system that combines pretrained vision foundation models with an existing Task and Motion Planner (TAMP) to solve multi-step manipulation tasks directly from input RGB images and natural-language instructions. Our system aims to be simple and easy-to-use: it can be installed and run on a standard DROID setup in under one hour and adapted to new embodiments with minimal effort. We evaluate TiPToP -- which requires zero robot data -- over 28 tabletop manipulation tasks in simulation and the real world and find it matches or outperforms $π_{0.5}\text{-DROID}$, a vision-language-action (VLA) model fine-tuned on 350 hours of embodiment-specific demonstrations. TiPToP's modular architecture enables us to analyze the system's failure modes at the component level. We analyze results from an evaluation of 173 trials and identify directions for improvement. We release TiPToP open-source to further research on modular manipulation systems and tighter integration between learning and planning. Project website and code: https://tiptop-robot.github.io

---

## 4. Think Before You Lie: How Reasoning Improves Honesty

**Meta**
- Authors: Ann Yuan, Asma Ghandeharioun, Carter Blum, Alicia Machado, Jessica Hoffmann, Daphne Ippolito, Martin Wattenberg, Lucas Dixon, Katja Filippova
- Published: 2026-03-11
- arXiv: https://arxiv.org/abs/2603.09957v1

**Abstract**
While existing evaluations of large language models (LLMs) measure deception rates, the underlying conditions that give rise to deceptive behavior are poorly understood. We investigate this question using a novel dataset of realistic moral trade-offs where honesty incurs variable costs. Contrary to humans, who tend to become less honest given time to deliberate (Capraro, 2017; Capraro et al., 2019), we find that reasoning consistently increases honesty across scales and for several LLM families. This effect is not only a function of the reasoning content, as reasoning traces are often poor predictors of final behaviors. Rather, we show that the underlying geometry of the representational space itself contributes to the effect. Namely, we observe that deceptive regions within this space are metastable: deceptive answers are more easily destabilized by input paraphrasing, output resampling, and activation noise than honest ones. We interpret the effect of reasoning in this vein: generating deliberative tokens as part of moral reasoning entails the traversal of a biased representational space, ultimately nudging the model toward its more stable, honest defaults.

---

## 5. Kinodynamic Motion Retargeting for Humanoid Locomotion via Multi-Contact Whole-Body Trajectory Optimization

**Meta**
- Authors: Xiaoyu Zhang, Steven Haener, Varun Madabushi, Maegan Tucker
- Published: 2026-03-11
- arXiv: https://arxiv.org/abs/2603.09956v1

**Abstract**
We present the KinoDynamic Motion Retargeting (KDMR) framework, a novel approach for humanoid locomotion that models the retargeting process as a multi-contact, whole-body trajectory optimization problem. Conventional kinematics-based retargeting methods rely solely on spatial motion capture (MoCap) data, inevitably introducing physically inconsistent artifacts, such as foot sliding and ground penetration, that severely degrade the performance of downstream imitation learning policies. To bridge this gap, KDMR extends beyond pure kinematics by explicitly enforcing rigid-body dynamics and contact complementarity constraints. Further, by integrating ground reaction force (GRF) measurements alongside MoCap data, our method automatically detects heel-toe contact events to accurately replicate complex human-like contact patterns. We evaluate KDMR against the state-of-the-art baseline, GMR, across three key dimensions: 1) the dynamic feasibility and smoothness of the retargeted motions, 2) the accuracy of GRF tracking compared to raw source data, and 3) the training efficiency and final performance of downstream control policies trained via the BeyondMimic framework. Experimental results demonstrate that KDMR significantly outperforms purely kinematic methods, yielding dynamically viable reference trajectories that accelerate policy convergence and enhance overall locomotion stability. Our end-to-end pipeline will be open-sourced upon publication.

---

## 6. From Semantics to Pixels: Coarse-to-Fine Masked Autoencoders for Hierarchical Visual Understanding

**Meta**
- Authors: Wenzhao Xiang, Yue Wu, Hongyang Yu, Feng Gao, Fan Yang, Xilin Chen
- Published: 2026-03-11
- arXiv: https://arxiv.org/abs/2603.09955v1

**Abstract**
Self-supervised visual pre-training methods face an inherent tension: contrastive learning (CL) captures global semantics but loses fine-grained detail, while masked image modeling (MIM) preserves local textures but suffers from "attention drift" due to semantically-agnostic random masking. We propose C2FMAE, a coarse-to-fine masked autoencoder that resolves this tension by explicitly learning hierarchical visual representations across three data granularities: semantic masks (scene-level), instance masks (object-level), and RGB images (pixel-level). Two synergistic innovations enforce a strict top-down learning principle. First, a cascaded decoder sequentially reconstructs from scene semantics to object instances to pixel details, establishing explicit cross-granularity dependencies that parallel decoders cannot capture. Second, a progressive masking curriculum dynamically shifts the training focus from semantic-guided to instance-guided and finally to random masking, creating a structured learning path from global context to local features. To support this framework, we construct a large-scale multi-granular dataset with high-quality pseudo-labels for all 1.28M ImageNet-1K images. Extensive experiments show that C2FMAE achieves significant performance gains on image classification, object detection, and semantic segmentation, validating the effectiveness of our hierarchical design in learning more robust and generalizable representations.

---

## 7. Leveraging whole slide difficulty in Multiple Instance Learning to improve prostate cancer grading

**Meta**
- Authors: Marie Arrivat, Rémy Peyret, Elsa Angelini, Pietro Gori
- Published: 2026-03-11
- arXiv: https://arxiv.org/abs/2603.09953v1

**Abstract**
Multiple Instance Learning (MIL) has been widely applied in histopathology to classify Whole Slide Images (WSIs) with slide-level diagnoses. While the ground truth is established by expert pathologists, the slides can be difficult to diagnose for non-experts and lead to disagreements between the annotators. In this paper, we introduce the notion of Whole Slide Difficulty (WSD), based on the disagreement between an expert and a non-expert pathologist. We propose two different methods to leverage WSD, a multi-task approach and a weighted classification loss approach, and we apply them to Gleason grading of prostate cancer slides. Results show that integrating WSD during training consistently improves the classification performance across different feature encoders and MIL methods, particularly for higher Gleason grades (i.e. worse diagnosis).

---

## 8. On the Width Scaling of Neural Optimizers Under Matrix Operator Norms I: Row/Column Normalization and Hyperparameter Transfer

**Meta**
- Authors: Ruihan Xu, Jiajin Li, Yiping Lu
- Published: 2026-03-11
- arXiv: https://arxiv.org/abs/2603.09952v1

**Abstract**
A central question in modern deep learning is how to design optimizers whose behavior remains stable as the network width $w$ increases. We address this question by interpreting several widely used neural-network optimizers, including \textrm{AdamW} and \textrm{Muon}, as instances of steepest descent under matrix operator norms. This perspective links optimizer geometry with the Lipschitz structure of the network forward map, and enables width-independent control of both Lipschitz and smoothness constants. However, steepest-descent rules induced by standard $p \to q$ operator norms lack layerwise composability and therefore cannot provide width-independent bounds in deep architectures. We overcome this limitation by introducing a family of mean-normalized operator norms, denoted $\pmean \to \qmean$, that admit layerwise composability, yield width-independent smoothness bounds, and give rise to practical optimizers such as \emph{rescaled} \textrm{AdamW}, row normalization, and column normalization. The resulting learning rate width-aware scaling rules recover $μ$P scaling~\cite{yang2021tensor} as a special case and provide a principled mechanism for cross-width learning-rate transfer across a broad class of optimizers. We further show that \textrm{Muon} can suffer an $\mathcal{O}(\sqrt{w})$ worst-case growth in the smoothness constant, whereas a new family of row-normalized optimizers we propose achieves width-independent smoothness guarantees. Based on the observations, we propose MOGA (Matrix Operator Geometry Aware), a width-aware optimizer based only on row/column-wise normalization that enables stable learning-rate transfer across model widths. Large-scale pre-training on GPT-2 and LLaMA shows that MOGA, especially with row normalization, is competitive with Muon while being notably faster in large-token and low-loss regimes.

---

## 9. Towards a Neural Debugger for Python

**Meta**
- Authors: Maximilian Beck, Jonas Gehring, Jannik Kossen, Gabriel Synnaeve
- Published: 2026-03-11
- arXiv: https://arxiv.org/abs/2603.09951v1

**Abstract**
Training large language models (LLMs) on Python execution traces grounds them in code execution and enables the line-by-line execution prediction of whole Python programs, effectively turning them into neural interpreters (FAIR CodeGen Team et al., 2025). However, developers rarely execute programs step by step; instead, they use debuggers to stop execution at certain breakpoints and step through relevant portions only while inspecting or modifying program variables. Existing neural interpreter approaches lack such interactive control. To address this limitation, we introduce neural debuggers: language models that emulate traditional debuggers, supporting operations such as stepping into, over, or out of functions, as well as setting breakpoints at specific source lines. We show that neural debuggers -- obtained via fine-tuning large LLMs or pre-training smaller models from scratch -- can reliably model both forward execution (predicting future states and outputs) and inverse execution (inferring prior states or inputs) conditioned on debugger actions. Evaluated on CruxEval, our models achieve strong performance on both output and input prediction tasks, demonstrating robust conditional execution modeling. Our work takes first steps towards future agentic coding systems in which neural debuggers serve as a world model for simulated debugging environments, providing execution feedback or enabling agents to interact with real debugging tools. This capability lays the foundation for more powerful code generation, program understanding, and automated debugging.

---

## 10. When Learning Rates Go Wrong: Early Structural Signals in PPO Actor-Critic

**Meta**
- Authors: Alberto Fernández-Hernández, Cristian Pérez-Corral, Jose I. Mestre, Manuel F. Dolz, Jose Duato, Enrique S. Quintana-Ortí
- Published: 2026-03-11
- arXiv: https://arxiv.org/abs/2603.09950v1

**Abstract**
Deep Reinforcement Learning systems are highly sensitive to the learning rate (LR), and selecting stable and performant training runs often requires extensive hyperparameter search. In Proximal Policy Optimization (PPO) actor--critic methods, small LR values lead to slow convergence, whereas large LR values may induce instability or collapse. We analyse this phenomenon from the behavior of the hidden neurons in the network using the Overfitting-Underfitting Indicator (OUI), a metric that quantifies the balance of binary activation patterns over a fixed probe batch. We introduce an efficient batch-based formulation of OUI and derive a theoretical connection between LR and activation sign changes, clarifying how a correct evolution of the neuron's inner structure depends on the step size.   Empirically, across three discrete-control environments and multiple seeds, we show that OUI measured at only 10\% of training already discriminates between LR regimes. We observe a consistent asymmetry: critic networks achieving highest return operate in an intermediate OUI band (avoiding saturation), whereas actor networks achieving highest return exhibit comparatively high OUI values. We then compare OUI-based screening rules against early return, clip-based, divergence-based, and flip-based criteria under matched recall over successful runs. In this setting, OUI provides the strongest early screening signal: OUI alone achieves the best precision at broader recall, while combining early return with OUI yields the highest precision in best-performing screening regimes, enabling aggressive pruning of unpromising runs without requiring full training.

---
