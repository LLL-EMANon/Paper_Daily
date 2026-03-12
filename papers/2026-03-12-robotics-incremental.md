# Daily Papers - 2026-03-12

**Topic**: robotics (incremental)  
**Filter**: last 7 days
**Count**: 10

---

## 1. Semantic Landmark Particle Filter for Robot Localisation in Vineyards

**Meta**
- Authors: Rajitha de Silva, Jonathan Cox, James R. Heselden, Marija Popović, Cesar Cadena, Riccardo Polvara
- Published: 2026-03-11
- arXiv: https://arxiv.org/abs/2603.10847v1

**Abstract**
Reliable localisation in vineyards is hindered by row-level perceptual aliasing: parallel crop rows produce nearly identical LiDAR observations, causing geometry-only and vision-based SLAM systems to converge towards incorrect corridors, particularly during headland transitions. We present a Semantic Landmark Particle Filter (SLPF) that integrates trunk and pole landmark detections with 2D LiDAR within a probabilistic localisation framework. Detected trunks are converted into semantic walls, forming structural row boundaries embedded in the measurement model to improve discrimination between adjacent rows. GNSS is incorporated as a lightweight prior that stabilises localisation when semantic observations are sparse.   Field experiments in a 10-row vineyard demonstrate consistent improvements over geometry-only (AMCL), vision-based (RTAB-Map), and GNSS baselines. Compared to AMCL, SLPF reduces Absolute Pose Error by 22% and 65% across two traversal directions; relative to a NoisyGNSS baseline, APE decreases by 65% and 61%. Row correctness improves from 0.67 to 0.73, while mean cross-track error decreases from 1.40 m to 1.26 m. These results show that embedding row-level structural semantics within the measurement model enables robust localisation in highly repetitive outdoor agricultural environments.

---

## 2. Sublinear-Time Reconfiguration of Programmable Matter with Joint Movements

**Meta**
- Authors: Manish Kumar, Othon Michail, Andreas Padalkin, Christian Scheideler
- Published: 2026-03-11
- arXiv: https://arxiv.org/abs/2603.10720v1

**Abstract**
We study centralized reconfiguration problems for geometric amoebot structures. A set of $n$ amoebots occupy nodes on the triangular grid and can reconfigure via expansion and contraction operations. We focus on the joint movement extension, where amoebots may expand and contract in parallel, enabling coordinated motion of larger substructures. Prior work introduced this extension and analyzed reconfiguration under additional assumptions such as metamodules.   In contrast, we investigate the intrinsic dynamics of reconfiguration without such assumptions by restricting attention to centralized algorithms, leaving distributed solutions for future work. We study the reconfiguration problem between two classes of amoebot structures $A$ and $B$: For every structure $S\in A$, the goal is to compute a schedule that reconfigures $S$ into some structure $S'\in B$. Our focus is on sublinear-time algorithms.   We affirmatively answer the open problem by Padalkin et al. (Auton. Robots, 2025) whether a within-the-model sublinear-time universal reconfiguration algorithm is possible, by proving that any structure can be reconfigured into a canonical line-segment structure in $O(\sqrt{n}\log n)$ rounds. Additionally, we give a constant-time algorithm for reconfiguring any spiral structure into a line segment. These results are enabled by new constant-time primitives that facilitate efficient parallel movement.   Our findings demonstrate that the joint movement model supports sublinear reconfiguration without auxiliary assumptions. A central open question is whether universal reconfiguration within this model can be achieved in polylogarithmic or even constant time.

---

## 3. ASTER: Attitude-aware Suspended-payload Quadrotor Traversal via Efficient Reinforcement Learning

**Meta**
- Authors: Dongcheng Cao, Jin Zhou, Shuo Li
- Published: 2026-03-11
- arXiv: https://arxiv.org/abs/2603.10715v1

**Abstract**
Agile maneuvering of the quadrotor cable-suspended system is significantly hindered by its non-smooth hybrid dynamics. While model-free Reinforcement Learning (RL) circumvents explicit differentiation of complex models, achieving attitude-constrained or inverted flight remains an open challenge due to the extreme reward sparsity under strict orientation requirements. This paper presents ASTER, a robust RL framework that achieves, to our knowledge, the first successful autonomous inverted flight for the cable-suspended system. We propose hybrid-dynamics-informed state seeding (HDSS), an initialization strategy that back-propagates target configurations through physics-consistent kinematic inversions across both taut and slack cable phases. HDSS enables the policy to discover aggressive maneuvers that are unreachable via standard exploration. Extensive simulations and real-world experiments demonstrate remarkable agility, precise attitude alignment, and robust zero-shot sim-to-real transfer across complex trajectories.

---

## 4. MAVEN: A Meta-Reinforcement Learning Framework for Varying-Dynamics Expertise in Agile Quadrotor Maneuvers

**Meta**
- Authors: Jin Zhou, Dongcheng Cao, Xian Wang, Shuo Li
- Published: 2026-03-11
- arXiv: https://arxiv.org/abs/2603.10714v1

**Abstract**
Reinforcement learning (RL) has emerged as a powerful paradigm for achieving online agile navigation with quadrotors. Despite this success, policies trained via standard RL typically fail to generalize across significant dynamic variations, exhibiting a critical lack of adaptability. This work introduces MAVEN, a meta-RL framework that enables a single policy to achieve robust end-to-end navigation across a wide range of quadrotor dynamics. Our approach features a novel predictive context encoder, which learns to infer a latent representation of the system dynamics from interaction history. We demonstrate our method in agile waypoint traversal tasks under two challenging scenarios: large variations in quadrotor mass and severe single-rotor thrust loss. We leverage a GPU-vectorized simulator to distribute tasks across thousands of parallel environments, overcoming the long training times of meta-RL to converge in less than an hour. Through extensive experiments in both simulation and the real world, we validate that MAVEN achieves superior adaptation and agility. The policy successfully executes zero-shot sim-to-real transfer, demonstrating robust online adaptation by performing high-speed maneuvers despite mass variations of up to 66.7% and single-rotor thrust losses as severe as 70%.

---

## 5. FutureVLA: Joint Visuomotor Prediction for Vision-Language-Action Model

**Meta**
- Authors: Xiaoxu Xu, Hao Li, Jinhui Ye, Yilun Chen, Jia Zeng, Xinyi Chen, Linning Xu, Dahua Lin, Weixin Li, Jiangmiao Pang
- Published: 2026-03-11
- arXiv: https://arxiv.org/abs/2603.10712v1

**Abstract**
Predictive foresight is important to intelligent embodied agents. Since the motor execution of a robot is intrinsically constrained by its visual perception of environmental geometry, effectively anticipating the future requires capturing this tightly coupled visuomotor interplay. While recent vision-language-action models attempt to incorporate future guidance, they struggle with this joint modeling. Existing explicit methods divert capacity to task-irrelevant visual details, whereas implicit methods relying on sparse frame pairs disrupt temporal continuity. By heavily relying on visual reconstruction, these methods become visually dominated, entangling static scene context with dynamic action intent. We argue that effective joint visuomotor predictive modeling requires both temporal continuity and visually-conditioned supervision decoupling. To this end, we propose FutureVLA, featuring a novel Joint Visuomotor Predictive Architecture. FutureVLA is designed to extract joint visuomotor embeddings by first decoupling visual and motor information, and then jointly encoding generalized physical priors. Specifically, in the pretraining stage, we leverage heterogeneous manipulation datasets and introduce a Joint Visuomotor Gating mechanism to structurally separate visual state preservation from temporal action modeling. It allows the motor stream to focus on continuous physical dynamics while explicitly querying visual tokens for environmental constraints, yielding highly generalizable joint visuomotor embeddings. Subsequently, in the post-training stage, we employ a latent embeddings alignment strategy, enabling diverse downstream VLA models to internalize these temporal priors without modifying their inference architectures. Extensive experiments demonstrate that FutureVLA consistently improves VLA frameworks.

---

## 6. Parallel-in-Time Nonlinear Optimal Control via GPU-native Sequential Convex Programming

**Meta**
- Authors: Yilin Zou, Zhong Zhang, Fanghua Jiang
- Published: 2026-03-11
- arXiv: https://arxiv.org/abs/2603.10711v1

**Abstract**
Real-time trajectory optimization for nonlinear constrained autonomous systems is critical and typically performed by CPU-based sequential solvers. Specifically, reliance on global sparse linear algebra or the serial nature of dynamic programming algorithms restricts the utilization of massively parallel computing architectures like GPUs. To bridge this gap, we introduce a fully GPU-native trajectory optimization framework that combines sequential convex programming with a consensus-based alternating direction method of multipliers. By applying a temporal splitting strategy, our algorithm decouples the optimization horizon into independent, per-node subproblems that execute massively in parallel. The entire process runs fully on the GPU, eliminating costly memory transfers and large-scale sparse factorizations. This architecture naturally scales to multi-trajectory optimization. We validate the solver on a quadrotor agile flight task and a Mars powered descent problem using an on-board edge computing platform. Benchmarks reveal a sustained 4x throughput speedup and a 51% reduction in energy consumption over a heavily optimized 12-core CPU baseline. Crucially, the framework saturates the hardware, maintaining over 96% active GPU utilization to achieve planning rates exceeding 100 Hz. Furthermore, we demonstrate the solver's extensibility to robust Model Predictive Control by jointly optimizing dynamically coupled scenarios under stochastic disturbances, enabling scalable and safe autonomy.

---

## 7. MapGCLR: Geospatial Contrastive Learning of Representations for Online Vectorized HD Map Construction

**Meta**
- Authors: Jonas Merkert, Alexander Blumberg, Jan-Hendrik Pauls, Christoph Stiller
- Published: 2026-03-11
- arXiv: https://arxiv.org/abs/2603.10688v1

**Abstract**
Autonomous vehicles rely on map information to understand the world around them. However, the creation and maintenance of offline high-definition (HD) maps remains costly. A more scalable alternative lies in online HD map construction, which only requires map annotations at training time. To further reduce the need for annotating vast training labels, self-supervised training provides an alternative. This work focuses on improving the latent birds-eye-view (BEV) feature grid representation within a vectorized online HD map construction model by enforcing geospatial consistency between overlapping BEV feature grids as part of a contrastive loss function. To ensure geospatial overlap for contrastive pairs, we introduce an approach to analyze the overlap between traversals within a given dataset and generate subsidiary dataset splits following adjustable multi-traversal requirements. We train the same model supervised using a reduced set of single-traversal labeled data and self-supervised on a broader unlabeled set of data following our multi-traversal requirements, effectively implementing a semi-supervised approach. Our approach outperforms the supervised baseline across the board, both quantitatively in terms of the downstream tasks vectorized map perception performance and qualitatively in terms of segmentation in the principal component analysis (PCA) visualization of the BEV feature space.

---

## 8. OnFly: Onboard Zero-Shot Aerial Vision-Language Navigation toward Safety and Efficiency

**Meta**
- Authors: Guiyong Zheng, Yueting Ban, Mingjie Zhang, Juepeng Zheng, Boyu Zhou
- Published: 2026-03-11
- arXiv: https://arxiv.org/abs/2603.10682v1

**Abstract**
Aerial vision-language navigation (AVLN) enables UAVs to follow natural-language instructions in complex 3D environments. However, existing zero-shot AVLN methods often suffer from unstable single-stream Vision-Language Model decision-making, unreliable long-horizon progress monitoring, and a trade-off between safety and efficiency. We propose OnFly, a fully onboard, real-time framework for zero-shot AVLN. OnFly adopts a shared-perception dual-agent architecture that decouples high-frequency target generation from low-frequency progress monitoring, thereby stabilizing decision-making. It further employs a hybrid keyframe-recent-frame memory to preserve global trajectory context while maintaining KV-cache prefix stability, enabling reliable long-horizon monitoring with termination and recovery signals. In addition, a semantic-geometric verifier refines VLM-predicted targets for instruction consistency and geometric safety using VLM features and depth cues, while a receding-horizon planner generates optimized collision-free trajectories under geometric safety constraints, improving both safety and efficiency. In simulation, OnFly improves task success from 26.4% to 67.8%, compared with the strongest state-of-the-art baseline, while fully onboard real-world flights validate its feasibility for real-time deployment. The code will be released at https://github.com/Robotics-STAR-Lab/OnFly

---

## 9. Cybo-Waiter: A Physical Agentic Framework for Humanoid Whole-Body Locomotion-Manipulation

**Meta**
- Authors: Peng Ren, Haoyang Ge, Chuan Qi, Cong Huang, Hong Li, Jiang Zhao, Pei Chi, Kai Chen
- Published: 2026-03-11
- arXiv: https://arxiv.org/abs/2603.10675v1

**Abstract**
Robots are increasingly expected to execute open ended natural language requests in human environments, which demands reliable long horizon execution under partial observability. This is especially challenging for humanoids because locomotion and manipulation are tightly coupled through stance, reachability, and balance. We present a humanoid agent framework that turns VLM plans into verifiable task programs and closes the loop with multi object 3D geometric supervision. A VLM planner compiles each instruction into a typed JSON sequence of subtasks with explicit predicate based preconditions and success conditions. Using SAM3 and RGB-D, we ground all task relevant entities in 3D, estimate object centroids and extents, and evaluate predicates over stable frames to obtain condition level diagnostics. The supervisor uses these diagnostics to verify subtask completion and to provide condition-level feedback for progression and replanning. We execute each subtask by coordinating humanoid locomotion and whole-body manipulation, selecting feasible motion primitives under reachability and balance constraints. Experiments on tabletop manipulation and long horizon humanoid loco manipulation tasks show improved robustness from multi object grounding, temporal stability, and recovery driven replanning.

---

## 10. Dynamic Modeling and Attitude Control of a Reaction-Wheel-Based Low-Gravity Bipedal Hopper

**Meta**
- Authors: Shriram Hari, M Venkata Sai Nikhil, R Prasanth Kumar
- Published: 2026-03-11
- arXiv: https://arxiv.org/abs/2603.10670v1

**Abstract**
Planetary bodies characterized by low gravitational acceleration, such as the Moon and near-Earth asteroids, impose unique locomotion constraints due to diminished contact forces and extended airborne intervals. Among traversal strategies, hopping locomotion offers high energy efficiency but is prone to mid-flight attitude instability caused by asymmetric thrust generation and uneven terrain interactions. This paper presents an underactuated bipedal hopping robot that employs an internal reaction wheel to regulate body posture during the ballistic flight phase. The system is modeled as a gyrostat, enabling analysis of the dynamic coupling between torso rotation and reaction wheel momentum. The locomotion cycle comprises three phases: a leg-driven propulsive jump, mid-air attitude stabilization via an active momentum exchange controller, and a shock-absorbing landing. A reduced-order model is developed to capture the critical coupling between torso rotation and reaction wheel dynamics. The proposed framework is evaluated in MuJoCo-based simulations under lunar gravity conditions (g = 1.625 m/s^2). Results demonstrate that activation of the reaction wheel controller reduces peak mid-air angular deviation by more than 65% and constrains landing attitude error to within 3.5 degrees at touchdown. Additionally, actuator saturation per hop cycle is reduced, ensuring sufficient control authority. Overall, the approach significantly mitigates in-flight attitude excursions and enables consistent upright landings, providing a practical and control-efficient solution for locomotion on irregular extraterrestrial terrains.

---
