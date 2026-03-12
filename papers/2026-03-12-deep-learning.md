# Daily Papers - 2026-03-12

**Topic**: deep learning  
**Filter**: last 7 days
**Count**: 10

---

## 1. LiTo: Surface Light Field Tokenization

**Meta**
- Authors: Jen-Hao Rick Chang, Xiaoming Zhao, Dorian Chan, Oncel Tuzel
- Published: 2026-03-12
- arXiv: https://arxiv.org/abs/2603.11047v1

**Abstract**
We propose a 3D latent representation that jointly models object geometry and view-dependent appearance. Most prior works focus on either reconstructing 3D geometry or predicting view-independent diffuse appearance, and thus struggle to capture realistic view-dependent effects. Our approach leverages that RGB-depth images provide samples of a surface light field. By encoding random subsamples of this surface light field into a compact set of latent vectors, our model learns to represent both geometry and appearance within a unified 3D latent space. This representation reproduces view-dependent effects such as specular highlights and Fresnel reflections under complex lighting. We further train a latent flow matching model on this representation to learn its distribution conditioned on a single input image, enabling the generation of 3D objects with appearances consistent with the lighting and materials in the input. Experiments show that our approach achieves higher visual quality and better input fidelity than existing methods.

---

## 2. Neural Field Thermal Tomography: A Differentiable Physics Framework for Non-Destructive Evaluation

**Meta**
- Authors: Tao Zhong, Yixun Hu, Dongzhe Zheng, Aditya Sood, Christine Allen-Blanchette
- Published: 2026-03-12
- arXiv: https://arxiv.org/abs/2603.11045v1

**Abstract**
We propose Neural Field Thermal Tomography (NeFTY), a differentiable physics framework for the quantitative 3D reconstruction of material properties from transient surface temperature measurements. While traditional thermography relies on pixel-wise 1D approximations that neglect lateral diffusion, and soft-constrained Physics-Informed Neural Networks (PINNs) often fail in transient diffusion scenarios due to gradient stiffness, NeFTY parameterizes the 3D diffusivity field as a continuous neural field optimized through a rigorous numerical solver. By leveraging a differentiable physics solver, our approach enforces thermodynamic laws as hard constraints while maintaining the memory efficiency required for high-resolution 3D tomography. Our discretize-then-optimize paradigm effectively mitigates the spectral bias and ill-posedness inherent in inverse heat conduction, enabling the recovery of subsurface defects at arbitrary scales. Experimental validation on synthetic data demonstrates that NeFTY significantly improves the accuracy of subsurface defect localization over baselines. Additional details at https://cab-lab-princeton.github.io/nefty/

---

## 3. Agentar-Fin-OCR

**Meta**
- Authors: Siyi Qian, Xiongfei Bai, Bingtao Fu, Yichen Lu, Gaoyang Zhang, Xudong Yang, Peng Zhang
- Published: 2026-03-12
- arXiv: https://arxiv.org/abs/2603.11044v1

**Abstract**
In this paper, we propose Agentar-Fin-OCR, a document parsing system tailored to financial-domain documents, transforming ultra-long financial PDFs into semantically consistent, highly accurate, structured outputs with auditing-grade provenance. To address finance-specific challenges such as complex layouts, cross-page structural discontinuities, and cell-level referencing capability, Agentar-Fin-OCR combines (1) a Cross-page Contents Consolidation algorithm to restore continuity across pages and a Document-level Heading Hierarchy Reconstruction (DHR) module to build a globally consistent Table of Contents (TOC) tree for structure-aware retrieval, and (2) a difficulty-adaptive curriculum learning training strategy for table parsing, together with a CellBBoxRegressor module that uses structural anchor tokens to localize table cells from decoder hidden states without external detectors. Experiments demonstrate that our model shows high performance on the table parsing metrics of OmniDocBench. To enable realistic evaluation in the financial vertical, we further introduce FinDocBench, a benchmark that includes six financial document categories with expert-verified annotations and evaluation metrics including Table of Contents edit-distance-based similarity (TocEDS), cross-page concatenated TEDS, and Table Cell Intersection over Union (C-IoU). We evaluate a wide range of state-of-the-art models on FinDocBench to assess their capabilities and remaining limitations on financial documents. Overall, Agentar-Fin-OCR and FinDocBench provide a practical foundation for reliable downstream financial document applications.

---

## 4. V2M-Zero: Zero-Pair Time-Aligned Video-to-Music Generation

**Meta**
- Authors: Yan-Bo Lin, Jonah Casebeer, Long Mai, Aniruddha Mahapatra, Gedas Bertasius, Nicholas J. Bryan
- Published: 2026-03-12
- arXiv: https://arxiv.org/abs/2603.11042v1

**Abstract**
Generating music that temporally aligns with video events is challenging for existing text-to-music models, which lack fine-grained temporal control. We introduce V2M-Zero, a zero-pair video-to-music generation approach that outputs time-aligned music for video. Our method is motivated by a key observation: temporal synchronization requires matching when and how much change occurs, not what changes. While musical and visual events differ semantically, they exhibit shared temporal structure that can be captured independently within each modality. We capture this structure through event curves computed from intra-modal similarity using pretrained music and video encoders. By measuring temporal change within each modality independently, these curves provide comparable representations across modalities. This enables a simple training strategy: fine-tune a text-to-music model on music-event curves, then substitute video-event curves at inference without cross-modal training or paired data. Across OES-Pub, MovieGenBench-Music, and AIST++, V2M-Zero achieves substantial gains over paired-data baselines: 5-21% higher audio quality, 13-15% better semantic alignment, 21-52% improved temporal synchronization, and 28% higher beat alignment on dance videos. We find similar results via a large crowd-source subjective listening test. Overall, our results validate that temporal alignment through within-modality features, rather than paired cross-modal supervision, is effective for video-to-music generation. Results are available at https://genjib.github.io/v2m_zero/

---

## 5. DynVLA: Learning World Dynamics for Action Reasoning in Autonomous Driving

**Meta**
- Authors: Shuyao Shang, Bing Zhan, Yunfei Yan, Yuqi Wang, Yingyan Li, Yasong An, Xiaoman Wang, Jierui Liu, Lu Hou, Lue Fan, Zhaoxiang Zhang, Tieniu Tan
- Published: 2026-03-12
- arXiv: https://arxiv.org/abs/2603.11041v1

**Abstract**
We propose DynVLA, a driving VLA model that introduces a new CoT paradigm termed Dynamics CoT. DynVLA forecasts compact world dynamics before action generation, enabling more informed and physically grounded decision-making. To obtain compact dynamics representations, DynVLA introduces a Dynamics Tokenizer that compresses future evolution into a small set of dynamics tokens. Considering the rich environment dynamics in interaction-intensive driving scenarios, DynVLA decouples ego-centric and environment-centric dynamics, yielding more accurate world dynamics modeling. We then train DynVLA to generate dynamics tokens before actions through SFT and RFT, improving decision quality while maintaining latency-efficient inference. Compared to Textual CoT, which lacks fine-grained spatiotemporal understanding, and Visual CoT, which introduces substantial redundancy due to dense image prediction, Dynamics CoT captures the evolution of the world in a compact, interpretable, and efficient form. Extensive experiments on NAVSIM, Bench2Drive, and a large-scale in-house dataset demonstrate that DynVLA consistently outperforms Textual CoT and Visual CoT methods, validating the effectiveness and practical value of Dynamics CoT.

---

## 6. Leech Lattice Vector Quantization for Efficient LLM Compression

**Meta**
- Authors: Tycho F. A. van der Ouderaa, Mart van Baalen, Paul Whatmough, Markus Nagel
- Published: 2026-03-12
- arXiv: https://arxiv.org/abs/2603.11021v1

**Abstract**
Scalar quantization of large language models (LLMs) is fundamentally limited by information-theoretic bounds. While vector quantization (VQ) overcomes these limits by encoding blocks of parameters jointly, practical implementations must avoid the need for expensive lookup mechanisms or other explicit codebook storage. Lattice approaches address this through highly structured and dense packing. This paper explores the Leech lattice, which, with its optimal sphere packing and kissing configurations at 24 dimensions, is the highest dimensional lattice known with such optimal properties. To make the Leech lattice usable for LLM quantization, we extend an existing search algorithm based on the extended Golay code construction, to i) support indexing, enabling conversion to and from bitstrings without materializing the codebook, ii) allow angular search over union of Leech lattice shells, iii) propose fully-parallelisable dequantization kernel. Together this yields a practical algorithm, namely Leech Lattice Vector Quantization (LLVQ). LLVQ delivers state-of-the-art LLM quantization performance, outperforming recent methods such as Quip\#, QTIP, and PVQ. These results highlight the importance of high-dimensional lattices for scalable, theoretically grounded model compression.

---

## 7. Cross-Species Transfer Learning for Electrophysiology-to-Transcriptomics Mapping in Cortical GABAergic Interneurons

**Meta**
- Authors: Theo Schwider, Ramin Ramezani
- Published: 2026-03-12
- arXiv: https://arxiv.org/abs/2603.11000v1

**Abstract**
Single-cell electrophysiological recordings provide a powerful window into neuronal functional diversity and offer an interpretable route for linking intrinsic physiology to transcriptomic identity. Here, we replicate and extend the electrophysiology-to-transcriptomics framework introduced by Gouwens et al. (2020) using publicly available Allen Institute Patch-seq datasets from both mouse and human cortex. We focus on GABAergic inhibitory interneurons to target a subclass structure (Lamp5, Pvalb, Sst, Vip) that is comparable and conserved across species. After quality control, we analyzed 3,699 mouse visual cortex neurons and 506 human neocortical neurons from neurosurgical resections. Using standardized electrophysiological features and sparse PCA, we reproduced the major class-level separations reported in the original mouse study. For supervised prediction, a class-balanced random forest provided a strong feature-engineered baseline in mouse data and a reduced but still informative baseline in human data. We then developed an attention-based BiLSTM that operates directly on the structured IPFX feature-family representation, avoiding sPCA and providing feature-family-level interpretability via learned attention weights. Finally, we evaluated a cross-species transfer setting in which the sequence model is pretrained on mouse data and fine-tuned on human data for an aligned 4-class task, improving human macro-F1 relative to a human-only training baseline. Together, these results confirm reproducibility of the Gouwens pipeline in mouse data, demonstrate that sequence models can match feature-engineered baselines, and show that mouse-to-human transfer learning can provide measurable gains for human subclass prediction.

---

## 8. Factorized Neural Implicit DMD for Parametric Dynamics

**Meta**
- Authors: Siyuan Chen, Zhecheng Wang, Yixin Chen, Yue Chang, Peter Yichen Chen, Eitan Grinspun, Jonathan Panuelos
- Published: 2026-03-12
- arXiv: https://arxiv.org/abs/2603.10995v1

**Abstract**
A data-driven, model-free approach to modeling the temporal evolution of physical systems mitigates the need for explicit knowledge of the governing equations. Even when physical priors such as partial differential equations are available, such systems often reside in high-dimensional state spaces and exhibit nonlinear dynamics, making traditional numerical solvers computationally expensive and ill-suited for real-time analysis and control. Consider the problem of learning a parametric flow of a dynamical system: with an initial field and a set of physical parameters, we aim to predict the system's evolution over time in a way that supports long-horizon rollouts, generalization to unseen parameters, and spectral analysis.   We propose a physics-coded neural field parameterization of the Koopman operator's spectral decomposition. Unlike a physics-constrained neural field, which fits a single solution surface, and neural operators, which directly approximate the solution operator at fixed time horizons, our model learns a factorized flow operator that decouples spatial modes and temporal evolution. This structure exposes underlying eigenvalues, modes, and stability of the underlying physical process to enable stable long-term rollouts, interpolation across parameter spaces, and spectral analysis. We demonstrate the efficacy of our method on a range of dynamics problems, showcasing its ability to accurately predict complex spatiotemporal phenomena while providing insights into the system's dynamic behavior.

---

## 9. Artificial Intelligence as a Catalyst for Innovation in Software Engineering

**Meta**
- Authors: Carlos Alberto Fernández-y-Fernández, Jorge R. Aguilar-Cisneros
- Published: 2026-03-12
- arXiv: https://arxiv.org/abs/2603.10994v1

**Abstract**
The rapid evolution and inherent complexity of modern software requirements demand highly flexible and responsive development methodologies. While Agile frameworks have become the industry standard for prioritizing iteration, collaboration, and adaptability, software development teams continue to face persistent challenges in managing constantly evolving requirements and maintaining product quality under tight deadlines. This article explores the intersection of Artificial Intelligence (AI) and Software Engineering (SE), to analyze how AI serves as a powerful catalyst for enhancing agility and fostering innovation. The research combines a comprehensive review of existing literature with an empirical study, utilizing a survey directed at Software Engineering professionals to assess the perception, adoption, and impact of AI-driven tools. Key findings reveal that the integration of AI (specifically through Machine Learning (ML) and Natural Language Processing (NLP) )facilitates the automation of tedious tasks, from requirement management to code generation and testing . This paper demonstrates that AI not only optimizes current Agile practices but also introduces new capabilities essential for sustaining quality, speed, and innovation in the future landscape of software development.

---

## 10. Bayesian Optimization with Gaussian Processes to Accelerate Stationary Point Searches

**Meta**
- Authors: Rohit Goswami
- Published: 2026-03-12
- arXiv: https://arxiv.org/abs/2603.10992v1

**Abstract**
Accelerating the explorations of stationary points on potential energy surfaces building local surrogates spans decades of effort. Done correctly, surrogates reduce required evaluations by an order of magnitude while preserving the accuracy of the underlying theory. We present a unified Bayesian Optimization view of minimization, single point saddle searches, and double ended saddle searches through a unified six-step surrogate loop, differing only in the inner optimization target and acquisition criterion. The framework uses Gaussian process regression with derivative observations, inverse-distance kernels, and active learning. The Optimal Transport GP extensions of farthest point sampling with Earth mover's distance, MAP regularization via variance barrier and oscillation detection, and adaptive trust radius form concrete extensions of the same basic methodology, improving accuracy and efficiency. We also demonstrate random Fourier features decouple hyperparameter training from predictions enabling favorable scaling for high-dimensional systems. Accompanying pedagogical Rust code demonstrates that all applications use the exact same Bayesian optimization loop, bridging the gap between theoretical formulation and practical execution.

---
