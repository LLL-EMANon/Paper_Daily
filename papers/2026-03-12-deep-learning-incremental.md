# Daily Papers - 2026-03-12

**Topic**: deep learning (incremental)  
**Filter**: last 7 days
**Count**: 10

---

## 1. ForwardFlow: Simulation only statistical inference using deep learning

**Meta**
- Authors: Stefan Böhringer
- Published: 2026-03-12
- arXiv: https://arxiv.org/abs/2603.10991v1

**Abstract**
Deep learning models are being used for the analysis of parametric statistical models based on simulation-only frameworks. Bayesian models using normalizing flows simulate data from a prior distribution and are composed of two deep neural networks: a summary network that learns a sufficient statistic for the parameter and a normalizing flow that conditional on the summary network can approximate the posterior distribution. Here, we explore frequentist models that are based on a single summary network. During training, input of the network is a simulated data set based on a parameter and the loss function minimizes the mean-square error between learned summary and parameter. The network thereby solves the inverse problem of parameter estimation. We propose a branched network structure that contains collapsing layers that reduce a data set to summary statistics that are further mapped through fully connected layers to approximate the parameter estimate. We motivate our choice of network structure by theoretical considerations.   In simulations we demonstrate three desirable properties of parameter estimates: finite sample exactness, robustness to data contamination, and algorithm approximation. These properties are achieved offering the the network varying sample size, contaminated data, and data needing algorithmic reconstruction during the training phase. In our simulations an EM-algorithm for genetic data is automatically approximated by the network.   Simulation only approaches seem to offer practical advantages in complex modeling tasks where the simpler data simulation part is left to the researcher and the more complex problem of solving the inverse problem is left to the neural network. Challenging future work includes offering pre-trained models that can be used in a wide variety of applications.

---

## 2. Too Vivid to Be Real? Benchmarking and Calibrating Generative Color Fidelity

**Meta**
- Authors: Zhengyao Fang, Zexi Jia, Yijia Zhong, Pengcheng Luo, Jinchao Zhang, Guangming Lu, Jun Yu, Wenjie Pei
- Published: 2026-03-12
- arXiv: https://arxiv.org/abs/2603.10990v1

**Abstract**
Recent advances in text-to-image (T2I) generation have greatly improved visual quality, yet producing images that appear visually authentic to real-world photography remains challenging. This is partly due to biases in existing evaluation paradigms: human ratings and preference-trained metrics often favor visually vivid images with exaggerated saturation and contrast, which make generations often too vivid to be real even when prompted for realistic-style images. To address this issue, we present Color Fidelity Dataset (CFD) and Color Fidelity Metric (CFM) for objective evaluation of color fidelity in realistic-style generations. CFD contains over 1.3M real and synthetic images with ordered levels of color realism, while CFM employs a multimodal encoder to learn perceptual color fidelity. In addition, we propose a training-free Color Fidelity Refinement (CFR) that adaptively modulates spatial-temporal guidance scale in generation, thereby enhancing color authenticity. Together, CFD supports CFM for assessment, whose learned attention further guides CFR to refine T2I fidelity, forming a progressive framework for assessing and improving color fidelity in realistic-style T2I generation. The dataset and code are available at https://github.com/ZhengyaoFang/CFM.

---

## 3. MCMC Informed Neural Emulators for Uncertainty Quantification in Dynamical Systems

**Meta**
- Authors: Heikki Haario, Zhi-Song Liu, Martin Simon, Hendrik Weichel
- Published: 2026-03-12
- arXiv: https://arxiv.org/abs/2603.10987v1

**Abstract**
Neural networks are a commonly used approach to replace physical models with computationally cheap surrogates. Parametric uncertainty quantification can be included in training, assuming that an accurate prior distribution of the model parameters is available. Here we study the common opposite situation, where direct screening or random sampling of model parameters leads to exhaustive training times and evaluations at unphysical parameter values. Our solution is to decouple uncertainty quantification from network architecture. Instead of sampling network weights, we introduce the model-parameter distribution as an input to network training via Markov chain Monte Carlo (MCMC). In this way, the surrogate achieves the same uncertainty quantification as the underlying physical model, but with substantially reduced computation time. The approach is fully agnostic with respect to the neural network choice. In our examples, we present a quantile emulator for prediction and a novel autoencoder-based ODE network emulator that can flexibly estimate different trajectory paths corresponding to different ODE model parameters. Moreover, we present a mathematical analysis that provides a transparent way to relate potential performance loss to measurable distribution mismatch.

---

## 4. The Discrete Charm of the MLP: Binary Routing of Continuous Signals in Transformer Feed-Forward Layers

**Meta**
- Authors: Peter Balogh
- Published: 2026-03-12
- arXiv: https://arxiv.org/abs/2603.10985v1

**Abstract**
We show that MLP layers in transformer language models perform binary routing of continuous signals: the decision of whether a token needs nonlinear processing is well-captured by binary neuron activations, even though the signals being routed are continuous. In GPT-2 Small (124M parameters), we find that specific neurons implement a consensus architecture -- seven "default-ON" neurons and one exception handler (N2123 in Layer 11) that are 93-98% mutually exclusive -- creating a binary routing switch. A cross-layer analysis reveals a developmental arc: early layers (L1-3) use single gateway neurons to route exceptions without consensus quorums; middle layers (L4-6) show diffuse processing with neither gateway nor consensus; and late layers (L7-11) crystallize full consensus/exception architectures with increasing quorum size (1 to 3 to 7 consensus neurons). Causal validation confirms the routing is functional: removing the MLP at consensus breakdown costs 43.3% perplexity, while at full consensus removing it costs only 10.1% -- exceeding a 4x difference. Comparing binary vs. continuous features for the routing decision confirms that binarization loses essentially no information (79.2% vs. 78.8% accuracy), while continuous activations carry additional magnitude information (R^2 = 0.36 vs. 0.22). This binary routing structure explains why smooth polynomial approximation fails: cross-validated polynomial fits (degrees 2-7) never exceed R^2 = 0.06 for highly nonlinear layers. We propose that the well-established piecewise-affine characterization of deep networks can be complemented by a routing characterization: along the natural data manifold, the piecewise boundaries implement binary decisions about which tokens need nonlinear processing, routing continuous signals through qualitatively different computational paths.

---

## 5. Federated Learning-driven Beam Management in LEO 6G Non-Terrestrial Networks

**Meta**
- Authors: Maria Lamprini Bartsioka, Ioannis A. Bartsiokas, Athanasios D. Panagopoulos, Dimitra I. Kaklamani, Iakovos S. Venieris
- Published: 2026-03-12
- arXiv: https://arxiv.org/abs/2603.10983v1

**Abstract**
Low Earth Orbit (LEO) Non-Terrestrial Networks (NTNs) require efficient beam management under dynamic propagation conditions. This work investigates Federated Learning (FL)-based beam selection in LEO satellite constellations, where orbital planes operate as distributed learners through the utilization of High-Altitude Platform Stations (HAPS). Two models, a Multi-Layer Perceptron (MLP) and a Graph Neural Network (GNN), are evaluated using realistic channel and beamforming data. Results demonstrate that GNN surpasses MLP in beam prediction accuracy and stability, particularly at low elevation angles, enabling lightweight and intelligent beam management for future NTN deployments.

---

## 6. PPGuide: Steering Diffusion Policies with Performance Predictive Guidance

**Meta**
- Authors: Zixing Wang, Devesh K. Jha, Ahmed H. Qureshi, Diego Romeres
- Published: 2026-03-12
- arXiv: https://arxiv.org/abs/2603.10980v1

**Abstract**
Diffusion policies have shown to be very efficient at learning complex, multi-modal behaviors for robotic manipulation. However, errors in generated action sequences can compound over time which can potentially lead to failure. Some approaches mitigate this by augmenting datasets with expert demonstrations or learning predictive world models which might be computationally expensive. We introduce Performance Predictive Guidance (PPGuide), a lightweight, classifier-based framework that steers a pre-trained diffusion policy away from failure modes at inference time. PPGuide makes use of a novel self-supervised process: it uses attention-based multiple instance learning to automatically estimate which observation-action chunks from the policy's rollouts are relevant to success or failure. We then train a performance predictor on this self-labeled data. During inference, this predictor provides a real-time gradient to guide the policy toward more robust actions. We validated our proposed PPGuide across a diverse set of tasks from the Robomimic and MimicGen benchmarks, demonstrating consistent improvements in performance.

---

## 7. Learning Adaptive Force Control for Contact-Rich Sample Scraping with Heterogeneous Materials

**Meta**
- Authors: Cenk Cetin, Shreyas Pouli, Gabriella Pizzuto
- Published: 2026-03-12
- arXiv: https://arxiv.org/abs/2603.10979v1

**Abstract**
The increasing demand for accelerated scientific discovery, driven by global challenges, highlights the need for advanced AI-driven robotics. Deploying robotic chemists in human-centric labs is key for the next horizon of autonomous discovery, as complex tasks still demand the dexterity of human scientists. Robotic manipulation in this context is uniquely challenged by handling diverse chemicals (granular, powdery, or viscous liquids), under varying lab conditions. For example, humans use spatulas for scraping materials from vial walls. Automating this process is challenging because it goes beyond simple robotic insertion tasks and traditional lab automation, requiring the execution of fine-granular movements within a constrained environment (the sample vial). Our work proposes an adaptive control framework to address this, relying on a low-level Cartesian impedance controller for stable and compliant physical interaction and a high-level reinforcement learning agent that learns to dynamically adjust interaction forces at the end-effector. The agent is guided by perception feedback, which provides the material's location. We first created a task-representative simulation environment with a Franka Research 3 robot, a scraping tool, and a sample vial containing heterogeneous materials. To facilitate the learning of an adaptive policy and model diverse characteristics, the sample is modelled as a collection of spheres, where each sphere is assigned a unique dislodgement force threshold, which is procedurally generated using Perlin noise. We train an agent to autonomously learn and adapt the optimal contact wrench for a sample scraping task in simulation and then successfully transfer this policy to a real robotic setup. Our method was evaluated across five different material setups, outperforming a fixed-wrench baseline by an average of 10.9%.

---

## 8. FRIEND: Federated Learning for Joint Optimization of multi-RIS Configuration and Eavesdropper Intelligent Detection in B5G Networks

**Meta**
- Authors: Maria Lamprini A. Bartsioka, Ioannis A. Bartsiokas, Anastasios K. Papazafeiropoulos, Maria A. Seimeni, Dimitra I. Kaklamani, Iakovos S. Venieris
- Published: 2026-03-12
- arXiv: https://arxiv.org/abs/2603.10977v1

**Abstract**
As wireless systems evolve toward Beyond 5G (B5G), the adoption of cell-free (CF) millimeter-wave (mmWave) architectures combined with Reconfigurable Intelligent Surfaces (RIS) is emerging as a key enabler for ultra-reliable, high-capacity, scalable, and secure Industrial Internet of Things (IIoT) communications. However, safeguarding these complex and distributed environments against eavesdropping remains a critical challenge, particularly when conventional security mechanisms struggle to overcome scalability, and latency constraints. In this paper, a novel framework for detecting malicious users in RIS-enhanced cell-free mmWave networks using Federated Learning (FL) is presented. The envisioned setup features multiple access points (APs) operating without traditional cell boundaries, assisted by RIS nodes to dynamically shape the wireless propagation environment. Edge devices collaboratively train a Deep Convolutional Neural Network (DCNN) on locally observed Channel State Information (CSI), eliminating the need for raw data exchange. Moreover, an early-exit mechanism is incorporated in that model to jointly satisfy computational complexity requirements. Performance evaluation indicates that the integration of FL and multi-RIS coordination improves approximately 30% the achieved secrecy rate (SR) compared to baseline non-RIS-assisted methods while maintaining near-optimal detection accuracy levels. This work establishes a distributed, privacy-preserving approach to physical layer eavesdropping detection tailored for next-generation IIoT deployments.

---

## 9. Contact Coverage-Guided Exploration for General-Purpose Dexterous Manipulation

**Meta**
- Authors: Zixuan Liu, Ruoyi Qiao, Chenrui Tie, Xuanwei Liu, Yunfan Lou, Chongkai Gao, Zhixuan Xu, Lin Shao
- Published: 2026-03-12
- arXiv: https://arxiv.org/abs/2603.10971v1

**Abstract**
Deep Reinforcement learning (DRL) has achieved remarkable success in domains with well-defined reward structures, such as Atari games and locomotion. In contrast, dexterous manipulation lacks general-purpose reward formulations and typically depends on task-specific, handcrafted priors to guide hand-object interactions. We propose Contact Coverage-Guided Exploration (CCGE), a general exploration method designed for general-purpose dexterous manipulation tasks. CCGE represents contact state as the intersection between object surface points and predefined hand keypoints, encouraging dexterous hands to discover diverse and novel contact patterns, namely which fingers contact which object regions. It maintains a contact counter conditioned on discretized object states obtained via learned hash codes, capturing how frequently each finger interacts with different object regions. This counter is leveraged in two complementary ways: (1) to assign a count-based contact coverage reward that promotes exploration of novel contact patterns, and (2) an energy-based reaching reward that guides the agent toward under-explored contact regions. We evaluate CCGE on a diverse set of dexterous manipulation tasks, including cluttered object singulation, constrained object retrieval, in-hand reorientation, and bimanual manipulation. Experimental results show that CCGE substantially improves training efficiency and success rates over existing exploration methods, and that the contact patterns learned with CCGE transfer robustly to real-world robotic systems. Project page is https://contact-coverage-guided-exploration.github.io.

---

## 10. TOSSS: a CVE-based Software Security Benchmark for Large Language Models

**Meta**
- Authors: Marc Damie, Murat Bilgehan Ertan, Domenico Essoussi, Angela Makhanu, Gaëtan Peter, Roos Wensveen
- Published: 2026-03-12
- arXiv: https://arxiv.org/abs/2603.10969v1

**Abstract**
With their increasing capabilities, Large Language Models (LLMs) are now used across many industries. They have become useful tools for software engineers and support a wide range of development tasks. As LLMs are increasingly used in software development workflows, a critical question arises: are LLMs good at software security? At the same time, organizations worldwide invest heavily in cybersecurity to reduce exposure to disruptive attacks. The integration of LLMs into software engineering workflows may introduce new vulnerabilities and weaken existing security efforts.   We introduce TOSSS (Two-Option Secure Snippet Selection), a benchmark that measures the ability of LLMs to choose between secure and vulnerable code snippets. Existing security benchmarks for LLMs cover only a limited range of vulnerabilities. In contrast, TOSSS relies on the CVE database and provides an extensible framework that can integrate newly disclosed vulnerabilities over time. Our benchmark gives each model a security score between 0 and 1 based on its behavior; a score of 1 indicates that the model always selects the secure snippet, while a score of 0 indicates that it always selects the vulnerable one. We evaluate 14 widely used open-source and closed-source models on C/C++ and Java code and observe scores ranging from 0.48 to 0.89. LLM providers already publish many benchmark scores for their models, and TOSSS could become a complementary security-focused score to include in these reports.

---
