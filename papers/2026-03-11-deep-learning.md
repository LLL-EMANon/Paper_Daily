# Daily Papers - 2026-03-11

**Topic**: deep learning  
**Filter**: last 7 days
**Count**: 10

---

## 1. Impermanent: A Live Benchmark for Temporal Generalization in Time Series Forecasting

**Meta**
- Authors: Azul Garza, Renée Rosillo, Rodrigo Mendoza-Smith, David Salinas, Andrew Robert Williams, Arjun Ashok, Mononito Goswami, José Martín Juárez
- Published: 2026-03-10
- arXiv: https://arxiv.org/abs/2603.08707v1

**Abstract**
Recent advances in time-series forecasting increasingly rely on pre-trained foundation-style models. While these models often claim broad generalization, existing evaluation protocols provide limited evidence. Indeed, most current benchmarks use static train-test splits that can easily lead to contamination as foundation models can inadvertently train on test data or perform model selection using test scores, which can inflate performance. We introduce Impermanent, a live benchmark that evaluates forecasting models under open-world temporal change by scoring forecasts sequentially over time on continuously updated data streams, enabling the study of temporal robustness, distributional shift, and performance stability rather than one-off accuracy on a frozen test set. Impermanent is instantiated on GitHub open-source activity, providing a naturally live and highly non-stationary dataset shaped by releases, shifting contributor behavior, platform/tooling changes, and external events. We focus on the top 400 repositories by star count and construct time series from issues opened, pull requests opened, push events, and new stargazers, evaluated over a rolling window with daily updates, alongside standardized protocols and leaderboards for reproducible, ongoing comparison. By shifting evaluation from static accuracy to sustained performance, Impermanent takes a concrete step toward assessing when and whether foundation-level generalization in time-series forecasting can be meaningfully claimed. Code and a live dashboard are available at https://github.com/TimeCopilot/impermanent and https://impermanent.timecopilot.dev.

---

## 2. Agentic Critical Training

**Meta**
- Authors: Weize Liu, Minghui Liu, Sy-Tuyen Ho, Souradip Chakraborty, Xiyao Wang, Furong Huang
- Published: 2026-03-10
- arXiv: https://arxiv.org/abs/2603.08706v1

**Abstract**
Training large language models (LLMs) as autonomous agents often begins with imitation learning, but it only teaches agents what to do without understanding why: agents never contrast successful actions against suboptimal alternatives and thus lack awareness of action quality. Recent approaches attempt to address this by introducing self-reflection supervision derived from contrasts between expert and alternative actions. However, the training paradigm fundamentally remains imitation learning: the model imitates pre-constructed reflection text rather than learning to reason autonomously. We propose Agentic Critical Training (ACT), a reinforcement learning paradigm that trains agents to identify the better action among alternatives. By rewarding whether the model's judgment is correct, ACT drives the model to autonomously develop reasoning about action quality, producing genuine self-reflection rather than imitating it. Across three challenging agent benchmarks, ACT consistently improves agent performance when combined with different post-training methods. It achieves an average improvement of 5.07 points over imitation learning and 4.62 points over reinforcement learning. Compared to approaches that inject reflection capability through knowledge distillation, ACT also demonstrates clear advantages, yielding an average improvement of 2.42 points. Moreover, ACT enables strong out-of-distribution generalization on agentic benchmarks and improves performance on general reasoning benchmarks without any reasoning-specific training data, highlighting the value of our method. These results suggest that ACT is a promising path toward developing more reflective and capable LLM agents.

---

## 3. Split Federated Learning Architectures for High-Accuracy and Low-Delay Model Training

**Meta**
- Authors: Yiannis Papageorgiou, Yannis Thomas, Ramin Khalili, Iordanis Koutsopoulos
- Published: 2026-03-10
- arXiv: https://arxiv.org/abs/2603.08687v1

**Abstract**
Can we find a network architecture for ML model training so as to optimize training loss (and thus, accuracy) in Split Federated Learning (SFL)? And can this architecture also reduce training delay and communication overhead? While accuracy is not influenced by how we split the model in ordinary, state-of-the-art SFL, in this work we answer the questions above in the affirmative. Recent Hierarchical SFL (HSFL) architectures adopt a three-tier training structure consisting of clients, (local) aggregators, and a central server. In this architecture, the model is partitioned at two partitioning layers into three sub-models, which are executed across the three tiers. Despite their merits, HSFL architectures overlook the impact of the partitioning layers and client-to-aggregator assignments on accuracy, delay, and overhead. This work explicitly captures the impact of the partitioning layers and client-to-aggregator assignments on accuracy, delay and overhead by formulating a joint optimization problem. We prove that the problem is NP-hard and propose the first accuracy-aware heuristic algorithm that explicitly accounts for model accuracy, while remaining delay-efficient. Simulation results on public datasets show that our approach can improve accuracy by 3%, while reducing delay by 20% and overhead by 50%, compared to state-of-the-art SFL and HSFL schemes.

---

## 4. Benchmarking Language Modeling for Lossless Compression of Full-Fidelity Audio

**Meta**
- Authors: Phillip Long, Zachary Novack, Chris Donahue
- Published: 2026-03-10
- arXiv: https://arxiv.org/abs/2603.08683v1

**Abstract**
Autoregressive "language" models (LMs) trained on raw waveforms can be repurposed for lossless audio compression, but prior work is limited to 8-bit audio, leaving open whether such approaches work for practical settings (16/24-bit) and can compete with existing codecs. We benchmark LM-based compression on full-fidelity audio across diverse domains (music, speech, bioacoustics), sampling rates (16kHz-48kHz), and bit depths (8, 16, 24-bit). Standard sample-level tokenization becomes intractable at higher bit depths due to vocabulary size (65K for 16-bit; 16.7M for 24-bit). We propose Trilobyte, a byte-level tokenization schema for full resolution audio, improving vocabulary scaling from $O(2^{b})$ to $O(1)$ and enabling the first tractable 24-bit LM-based lossless compression. While LMs consistently outperform FLAC and yield state-of-the-art compression at 8-bit and 16-bit, we observe that compression gains become more modest as bit depth increases beyond 8-bit.

---

## 5. Structural Causal Bottleneck Models

**Meta**
- Authors: Simon Bing, Jonas Wahl, Jakob Runge
- Published: 2026-03-10
- arXiv: https://arxiv.org/abs/2603.08682v1

**Abstract**
We introduce structural causal bottleneck models (SCBMs), a novel class of structural causal models. At the core of SCBMs lies the assumption that causal effects between high-dimensional variables only depend on low-dimensional summary statistics, or bottlenecks, of the causes. SCBMs provide a flexible framework for task-specific dimension reduction while being estimable via standard, simple learning algorithms in practice. We analyse identifiability in SCBMs, connect them to information bottlenecks in the sense of Tishby & Zaslavsky (2015), and illustrate how to estimate them experimentally. We also demonstrate the benefit of bottlenecks for effect estimation in low-sample transfer learning settings. We argue that SCBMs provide an alternative to existing causal dimension reduction frameworks like causal representation learning or causal abstraction learning.

---

## 6. ER-Pose: Rethinking Keypoint-Driven Representation Learning for Real-Time Human Pose Estimation

**Meta**
- Authors: Nanjun Li, Pinqi Cheng, Zean Liu, Minghe Tian, Xuanyin Wang
- Published: 2026-03-10
- arXiv: https://arxiv.org/abs/2603.08681v1

**Abstract**
Single-stage multi-person pose estimation aims to jointly perform human localization and keypoint prediction within a unified framework, offering advantages in inference efficiency and architectural simplicity. Consequently, multi-scale real-time detection architectures, such as YOLO-like models, are widely adopted for real-time pose estimation. However, these approaches typically inherit a box-driven modeling paradigm from object detection, in which pose estimation is implicitly constrained by bounding-box supervision during training. This formulation introduces biases in sample assignment and feature representation, resulting in task misalignment and ultimately limiting pose estimation accuracy. In this work, we revisit box-driven single-stage pose estimation from a keypoint-driven perspective and identify semantic conflicts among parallel objectives as a key source of performance degradation. To address this issue, we propose a keypoint-driven learning paradigm that elevates pose estimation to a primary prediction objective. Specifically, we remove bounding-box prediction and redesign the prediction head to better accommodate the high-dimensional structured representations for pose estimation. We further introduce a keypoint-driven dynamic sample assignment strategy to align training objectives with pose evaluation metrics, enabling dense supervision during training and efficient NMS-free inference. In addition, we propose a smooth OKS-based loss function to stabilize optimization in regression-based pose estimation. Based on these designs, we develop a single-stage multi-person pose estimation framework, termed ER-Pose. On MS COCO and CrowdPose, ER-Pose-n achieves AP improvements of 3.2/6.7 without pre-training and 7.4/4.9 with pre-training respectively compared with the baseline YOLO-Pose. These improvements are achieved with fewer parameters and higher inference efficiency.

---

## 7. A New Lower Bound for the Random Offerer Mechanism in Bilateral Trade using AI-Guided Evolutionary Search

**Meta**
- Authors: Yang Cai, Vineet Gupta, Zun Li, Aranyak Mehta
- Published: 2026-03-10
- arXiv: https://arxiv.org/abs/2603.08679v1

**Abstract**
The celebrated Myerson--Satterthwaite theorem shows that in bilateral trade, no mechanism can be simultaneously fully efficient, Bayesian incentive compatible (BIC), and budget balanced (BB). This naturally raises the question of how closely the gains from trade (GFT) achievable by a BIC and BB mechanism can approximate the first-best (fully efficient) benchmark. The optimal BIC and BB mechanism is typically complex and highly distribution-dependent, making it difficult to characterize directly. Consequently, much of the literature analyzes simpler mechanisms such as the Random-Offerer (RO) mechanism and establishes constant-factor guarantees relative to the first-best GFT. An important open question concerns the worst-case performance of the RO mechanism relative to first-best (FB) efficiency. While it was originally hypothesized that the approximation ratio $\frac{\text{GFT}_{\text{FB}}}{\text{GFT}_{\text{RO}}}$ is bounded by $2$, recent work provided counterexamples to this conjecture: Cai et al. proved that the ratio can be strictly larger than $2$, and Babaioff et al. exhibited an explicit example with ratio approximately $2.02$.   In this work, we employ AlphaEvolve, an AI-guided evolutionary search framework, to explore the space of value distributions. We identify a new worst-case instance that yields an improved lower bound of $\frac{\text{GFT}_{\text{FB}}}{\text{GFT}_{\text{RO}}} \ge \textbf{2.0749}$. This establishes a new lower bound on the worst-case performance of the Random-Offerer mechanism, demonstrating a wider efficiency gap than previously known.

---

## 8. Momentum SVGD-EM for Accelerated Maximum Marginal Likelihood Estimation

**Meta**
- Authors: Adam Rozzio, Rafael Athanasiades, O. Deniz Akyildiz
- Published: 2026-03-10
- arXiv: https://arxiv.org/abs/2603.08676v1

**Abstract**
Maximum marginal likelihood estimation (MMLE) can be formulated as the optimization of a free energy functional. From this viewpoint, the Expectation-Maximisation (EM) algorithm admits a natural interpretation as a coordinate descent method over the joint space of model parameters and probability measures. Recently, a significant body of work has adopted this perspective, leading to interacting particle algorithms for MMLE. In this paper, we propose an accelerated version of one such procedure, based on Stein variational gradient descent (SVGD), by introducing Nesterov acceleration in both the parameter updates and in the space of probability measures. The resulting method, termed Momentum SVGD-EM, consistently accelerates convergence in terms of required iterations across various tasks of increasing difficulty, demonstrating effectiveness in both low- and high-dimensional settings.

---

## 9. Characterization and upgrade of a quantum graph neural network for charged particle tracking

**Meta**
- Authors: Matteo Argenton, Laura Cappelli, Concezio Bozzi
- Published: 2026-03-10
- arXiv: https://arxiv.org/abs/2603.08667v1

**Abstract**
In the forthcoming years the LHC experiments are going to be upgraded to benefit from the substantial increase of the LHC instantaneous luminosity, which will lead to larger, denser events, and, consequently, greater complexity in reconstructing charged particle tracks, motivating frontier research in new technologies. Quantum machine learning models are being investigated as potential new approaches to high energy physics (HEP) tasks. We characterize and upgrade a quantum graph neural network (QGNN) architecture for charged particle track reconstruction on a simulated high luminosity dataset. The model operates on a set of event graphs, each built from the hits generated in tracking detector layers by particles produced in proton collisions, performing a classification of the possible hit connections between adjacent layers. In this approach the QGNN is designed as a hybrid architecture, interleaving classical feedforward networks with parametrized quantum circuits. We characterize the interplay between the classical and quantum components. We report on the principal upgrades to the original design, and present new evidence of improved training behavior, specifically in terms of convergence toward the final trained configuration.

---

## 10. How Far Can Unsupervised RLVR Scale LLM Training?

**Meta**
- Authors: Bingxiang He, Yuxin Zuo, Zeyuan Liu, Shangziqi Zhao, Zixuan Fu, Junlin Yang, Cheng Qian, Kaiyan Zhang, Yuchen Fan, Ganqu Cui, Xiusi Chen, Youbang Sun, Xingtai Lv, Xuekai Zhu, Li Sheng, Ran Li, Huan-ang Gao, Yuchen Zhang, Bowen Zhou, Zhiyuan Liu, Ning Ding
- Published: 2026-03-10
- arXiv: https://arxiv.org/abs/2603.08660v1

**Abstract**
Unsupervised reinforcement learning with verifiable rewards (URLVR) offers a pathway to scale LLM training beyond the supervision bottleneck by deriving rewards without ground truth labels. Recent works leverage model intrinsic signals, showing promising early gains, yet their potential and limitations remain unclear. In this work, we revisit URLVR and provide a comprehensive analysis spanning taxonomy, theory and extensive experiments. We first classify URLVR methods into intrinsic versus external based on reward sources, then establish a unified theoretical framework revealing that all intrinsic methods converge toward sharpening the model's initial distribution This sharpening mechanism succeeds when initial confidence aligns with correctness but fails catastrophically when misaligned. Through systematic experiments, we show intrinsic rewards consistently follow a rise-then-fall pattern across methods, with collapse timing determined by model prior rather than engineering choices. Despite these scaling limits, we find intrinsic rewards remain valuable in test-time training on small datasets, and propose Model Collapse Step to measure model prior, serving as a practical indicator for RL trainability. Finally, we explore external reward methods that ground verification in computational asymmetries, showing preliminary evidence they may escape the confidence-correctness ceiling. Our findings chart boundaries for intrinsic URLVR while motivating paths toward scalable alternatives.

---
