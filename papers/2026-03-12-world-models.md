# Daily Papers - 2026-03-12

**Topic**: world models  
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

## 2. Agentar-Fin-OCR

**Meta**
- Authors: Siyi Qian, Xiongfei Bai, Bingtao Fu, Yichen Lu, Gaoyang Zhang, Xudong Yang, Peng Zhang
- Published: 2026-03-12
- arXiv: https://arxiv.org/abs/2603.11044v1

**Abstract**
In this paper, we propose Agentar-Fin-OCR, a document parsing system tailored to financial-domain documents, transforming ultra-long financial PDFs into semantically consistent, highly accurate, structured outputs with auditing-grade provenance. To address finance-specific challenges such as complex layouts, cross-page structural discontinuities, and cell-level referencing capability, Agentar-Fin-OCR combines (1) a Cross-page Contents Consolidation algorithm to restore continuity across pages and a Document-level Heading Hierarchy Reconstruction (DHR) module to build a globally consistent Table of Contents (TOC) tree for structure-aware retrieval, and (2) a difficulty-adaptive curriculum learning training strategy for table parsing, together with a CellBBoxRegressor module that uses structural anchor tokens to localize table cells from decoder hidden states without external detectors. Experiments demonstrate that our model shows high performance on the table parsing metrics of OmniDocBench. To enable realistic evaluation in the financial vertical, we further introduce FinDocBench, a benchmark that includes six financial document categories with expert-verified annotations and evaluation metrics including Table of Contents edit-distance-based similarity (TocEDS), cross-page concatenated TEDS, and Table Cell Intersection over Union (C-IoU). We evaluate a wide range of state-of-the-art models on FinDocBench to assess their capabilities and remaining limitations on financial documents. Overall, Agentar-Fin-OCR and FinDocBench provide a practical foundation for reliable downstream financial document applications.

---

## 3. V2M-Zero: Zero-Pair Time-Aligned Video-to-Music Generation

**Meta**
- Authors: Yan-Bo Lin, Jonah Casebeer, Long Mai, Aniruddha Mahapatra, Gedas Bertasius, Nicholas J. Bryan
- Published: 2026-03-12
- arXiv: https://arxiv.org/abs/2603.11042v1

**Abstract**
Generating music that temporally aligns with video events is challenging for existing text-to-music models, which lack fine-grained temporal control. We introduce V2M-Zero, a zero-pair video-to-music generation approach that outputs time-aligned music for video. Our method is motivated by a key observation: temporal synchronization requires matching when and how much change occurs, not what changes. While musical and visual events differ semantically, they exhibit shared temporal structure that can be captured independently within each modality. We capture this structure through event curves computed from intra-modal similarity using pretrained music and video encoders. By measuring temporal change within each modality independently, these curves provide comparable representations across modalities. This enables a simple training strategy: fine-tune a text-to-music model on music-event curves, then substitute video-event curves at inference without cross-modal training or paired data. Across OES-Pub, MovieGenBench-Music, and AIST++, V2M-Zero achieves substantial gains over paired-data baselines: 5-21% higher audio quality, 13-15% better semantic alignment, 21-52% improved temporal synchronization, and 28% higher beat alignment on dance videos. We find similar results via a large crowd-source subjective listening test. Overall, our results validate that temporal alignment through within-modality features, rather than paired cross-modal supervision, is effective for video-to-music generation. Results are available at https://genjib.github.io/v2m_zero/

---

## 4. DynVLA: Learning World Dynamics for Action Reasoning in Autonomous Driving

**Meta**
- Authors: Shuyao Shang, Bing Zhan, Yunfei Yan, Yuqi Wang, Yingyan Li, Yasong An, Xiaoman Wang, Jierui Liu, Lu Hou, Lue Fan, Zhaoxiang Zhang, Tieniu Tan
- Published: 2026-03-12
- arXiv: https://arxiv.org/abs/2603.11041v1

**Abstract**
We propose DynVLA, a driving VLA model that introduces a new CoT paradigm termed Dynamics CoT. DynVLA forecasts compact world dynamics before action generation, enabling more informed and physically grounded decision-making. To obtain compact dynamics representations, DynVLA introduces a Dynamics Tokenizer that compresses future evolution into a small set of dynamics tokens. Considering the rich environment dynamics in interaction-intensive driving scenarios, DynVLA decouples ego-centric and environment-centric dynamics, yielding more accurate world dynamics modeling. We then train DynVLA to generate dynamics tokens before actions through SFT and RFT, improving decision quality while maintaining latency-efficient inference. Compared to Textual CoT, which lacks fine-grained spatiotemporal understanding, and Visual CoT, which introduces substantial redundancy due to dense image prediction, Dynamics CoT captures the evolution of the world in a compact, interpretable, and efficient form. Extensive experiments on NAVSIM, Bench2Drive, and a large-scale in-house dataset demonstrate that DynVLA consistently outperforms Textual CoT and Visual CoT methods, validating the effectiveness and practical value of Dynamics CoT.

---

## 5. Instruction set for the representation of graphs

**Meta**
- Authors: Ezequiel Lopez-Rubio, Mario Pascual-Gonzalez
- Published: 2026-03-12
- arXiv: https://arxiv.org/abs/2603.11039v1

**Abstract**
We present IsalGraph, a method for representing the structure of any finite, simple graph as a compact string over a nine-character instruction alphabet. The encoding is executed by a small virtual machine comprising a sparse graph, a circular doubly-linked list (CDLL) of graph-node references, and two traversal pointers. Instructions either move a pointer through the CDLL or insert a node or edge into the graph. A key design property is that every string over the alphabet decodes to a valid graph, with no invalid states reachable. A greedy \emph{GraphToString} algorithm encodes any connected graph into a string in time polynomial in the number of nodes; an exhaustive-backtracking variant produces a canonical string by selecting the lexicographically smallest shortest string across all starting nodes and all valid traversal orders. We evaluate the representation on five real-world graph benchmark datasets (IAM Letter LOW/MED/HIGH, LINUX, and AIDS) and show that the Levenshtein distance between IsalGraph strings correlates strongly with graph edit distance (GED). Together, these properties make IsalGraph strings a compact, isomorphism-invariant, and language-model-compatible sequential encoding of graph structure, with direct applications in graph similarity search, graph generation, and graph-conditioned language modelling

---

## 6. Beyond the Illusion of Consensus: From Surface Heuristics to Knowledge-Grounded Evaluation in LLM-as-a-Judge

**Meta**
- Authors: Mingyang Song, Mao Zheng, Chenning Xu
- Published: 2026-03-12
- arXiv: https://arxiv.org/abs/2603.11027v1

**Abstract**
The paradigm of LLM-as-a-judge relies on a critical assumption, namely that high inter-evaluator agreement indicates reliable and objective evaluation. We present two complementary findings that challenge this assumption. \textbf{First}, we demonstrate that this consensus is frequently illusory. We identify and formalize \textbf{Evaluation Illusion}, a phenomenon where LLM judges generate sophisticated critiques yet anchor scores on shared surface heuristics rather than substantive quality. Through a large-scale study of 105,600 evaluation instances (32 LLMs $\times$ 3 frontier judges $\times$ 100 tasks $\times$ 11 temperatures), we show that model-level agreement (Spearman $ρ= 0.99$) masks fragile sample-level agreement (Pearson $\bar{r} = 0.72$; absolute agreement ICC $= 0.67$), that merely sharing rubric structure restores 62\% of total agreement, and that high-quality outputs paradoxically receive the \textit{least} consistent evaluations. \textbf{Second}, we demonstrate that dynamically generating evaluation rubrics grounded in domain knowledge produces more meaningful assessment. We introduce MERG (Metacognitive Enhanced Rubric Generation), a knowledge-driven rubric generation framework whose domain-selective effects confirm this. Agreement \textit{increases} in codified domains (Education +22\%, Academic +27\%) where knowledge anchors evaluators on shared standards, while it decreases in subjective domains where genuine evaluative pluralism emerges. These findings suggest that evaluation rubrics should be dynamically enriched with expert knowledge rather than relying on generic criteria, with implications for reward modeling in RLAIF.

---

## 7. Does AI See like Art Historians? Interpreting How Vision Language Models Recognize Artistic Style

**Meta**
- Authors: Marvin Limpijankit, Milad Alshomary, Yassin Oulad Daoud, Amith Ananthram, Tim Trombley, Elias Stengel-Eskin, Mohit Bansal, Noam M. Elcott, Kathleen McKeown
- Published: 2026-03-12
- arXiv: https://arxiv.org/abs/2603.11024v1

**Abstract**
VLMs have become increasingly proficient at a range of computer vision tasks, such as visual question answering and object detection. This includes increasingly strong capabilities in the domain of art, from analyzing artwork to generation of art. In an interdisciplinary collaboration between computer scientists and art historians, we characterize the mechanisms underlying VLMs' ability to predict artistic style and assess the extent to which they align with the criteria art historians use to reason about artistic style. We employ a latent-space decomposition approach to identify concepts that drive art style prediction and conduct quantitative evaluations, causal analysis and assessment by art historians. Our findings indicate that 73% of the extracted concepts are judged by art historians to exhibit a coherent and semantically meaningful visual feature and 90% of concepts used to predict style of a given artwork were judged relevant. In cases where an irrelevant concept was used to successfully predict style, art historians identified possible reasons for its success; for example, the model might "understand" a concept in more formal terms, such as dark/light contrasts.

---

## 8. Leech Lattice Vector Quantization for Efficient LLM Compression

**Meta**
- Authors: Tycho F. A. van der Ouderaa, Mart van Baalen, Paul Whatmough, Markus Nagel
- Published: 2026-03-12
- arXiv: https://arxiv.org/abs/2603.11021v1

**Abstract**
Scalar quantization of large language models (LLMs) is fundamentally limited by information-theoretic bounds. While vector quantization (VQ) overcomes these limits by encoding blocks of parameters jointly, practical implementations must avoid the need for expensive lookup mechanisms or other explicit codebook storage. Lattice approaches address this through highly structured and dense packing. This paper explores the Leech lattice, which, with its optimal sphere packing and kissing configurations at 24 dimensions, is the highest dimensional lattice known with such optimal properties. To make the Leech lattice usable for LLM quantization, we extend an existing search algorithm based on the extended Golay code construction, to i) support indexing, enabling conversion to and from bitstrings without materializing the codebook, ii) allow angular search over union of Leech lattice shells, iii) propose fully-parallelisable dequantization kernel. Together this yields a practical algorithm, namely Leech Lattice Vector Quantization (LLVQ). LLVQ delivers state-of-the-art LLM quantization performance, outperforming recent methods such as Quip\#, QTIP, and PVQ. These results highlight the importance of high-dimensional lattices for scalable, theoretically grounded model compression.

---

## 9. A Systematic Study of Pseudo-Relevance Feedback with LLMs

**Meta**
- Authors: Nour Jedidi, Jimmy Lin
- Published: 2026-03-12
- arXiv: https://arxiv.org/abs/2603.11008v1

**Abstract**
Pseudo-relevance feedback (PRF) methods built on large language models (LLMs) can be organized along two key design dimensions: the feedback source, which is where the feedback text is derived from and the feedback model, which is how the given feedback text is used to refine the query representation. However, the independent role that each dimension plays is unclear, as both are often entangled in empirical evaluations. In this paper, we address this gap by systematically studying how the choice of feedback source and feedback model impact PRF effectiveness through controlled experimentation. Across 13 low-resource BEIR tasks with five LLM PRF methods, our results show: (1) the choice of feedback model can play a critical role in PRF effectiveness; (2) feedback derived solely from LLM-generated text provides the most cost-effective solution; and (3) feedback derived from the corpus is most beneficial when utilizing candidate documents from a strong first-stage retriever. Together, our findings provide a better understanding of which elements in the PRF design space are most important.

---

## 10. RCTs & Human Uplift Studies: Methodological Challenges and Practical Solutions for Frontier AI Evaluation

**Meta**
- Authors: Patricia Paskov, Kevin Wei, Shen Zhou Hong, Dan Bateyko, Xavier Roberts-Gaal, Carson Ezell, Gailius Praninskas, Valerie Chen, Umang Bhatt, Ella Guest
- Published: 2026-03-12
- arXiv: https://arxiv.org/abs/2603.11001v1

**Abstract**
Human uplift studies - or studies that measure AI effects on human performance relative to a status quo, typically using randomized controlled trial (RCT) methodology - are increasingly used to inform deployment, governance, and safety decisions for frontier AI systems. While the methods underlying these studies are well-established, their interaction with the distinctive properties of frontier AI systems remains underexamined, particularly when results are used to inform high-stakes decisions. We present findings from interviews with 16 expert practitioners with experience conducting human uplift studies in domains including biosecurity, cybersecurity, education, and labor. Across interviews, experts described a recurring tension between standard causal inference assumptions and the object of study itself. Rapidly evolving AI systems, shifting baselines, heterogeneous and changing user proficiency, and porous real-world settings strain assumptions underlying internal, external, and construct validity, complicating the interpretation and appropriate use of uplift evidence. We synthesize these challenges across key stages of the human uplift research lifecycle and map them to practitioner-reported solutions, clarifying both the limits and the appropriate uses of evidence from human uplift studies in high-stakes decision-making.

---
