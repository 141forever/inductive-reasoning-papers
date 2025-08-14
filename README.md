# The Paper Collection of Inductive Reasoning



## Importance

1.  **When Is Inductive Inference Possible?** [NIPS2024] [[paper link](https://papers.nips.cc/paper_files/paper/2024/file/a8808b75b299d64a23255bc8d30fb786-Paper-Conference.pdf)]

      归纳推理的小综述。


    

## Benchmarks, Datasets and Tasks

1.  **On the Transfer of Inductive Bias from Simulation to the Real World: a New Disentanglement Dataset** [NIPS2019] [[paper link](https://papers.nips.cc/paper_files/paper/2019/file/d97d404b6119214e4a7018391195240a-Paper.pdf)]

      提出了一个数据集，通过真实机械臂采样而来的，包含超过一百万张物理三维物体的图像，拥有三个子集，以提升模型的迁移效果和inductive bias。【MPI3D】【disentanglement metrics】【各类VAE模型】
    
2.  **Learning abstract structure for drawing by efficient motor program induction** [NIPS2020] [[paper link](https://papers.nips.cc/paper_files/paper/2020/file/1c104b9c0accfca52ef21728eaf01453-Paper.pdf)]

     研究人类如何几次演练后便构建出抽象的、可复用的程序性先验知识，供模型学习。揭示两大元学习原则：abstraction（抽象）和compositionality（组合）是构成人类快速学习结构化表示的关键，同时强调motor efficiency的先验在真实行为再现中必不可少。【手绘风格图形】【stroke order, motor trajectory, 模型重现度】【PI,Hybrid等】

3.  **A large-scale benchmark for few-shot program induction and synthesis** [ICML2021] [[paper link](https://proceedings.mlr.press/v139/alet21a/alet21a.pdf)]
   
      PROGES，一个程序归纳benchmark。
    
4.  **What Has a Foundation Model Found? Inductive Bias Reveals World Models** [ICML2025] [[paper link](https://openreview.net/pdf?id=i9npQatSev)]
   
      通过构造与已知世界模型（如牛顿力学）一致的合成数据集，测试基础模型在新任务上的适应能力，进而评估其归纳偏差是否与世界模型一致。

5. **Unsupervised Vision-Language Grammar Induction with Shared Structure Modeling** [ICLR2022] [[paper link](https://openreview.net/pdf?id=N0n_QyQ5lBF)]

      无监督的视觉–语言（vision‑language, VL）语法归纳任务，即从给定的图像与其描述文字对中，同时归纳出共享的、层级化的结构（如句法树），旨在促进对图像与语言中共同结构的深层理解。任务名称：VL grammar induction。数据集名称：Flickr30k Entities。指标：CCRA。

6. **GeoILP: A Synthetic Dataset to Guide Large‑Scale Rule Induction** [ICLR2025] [[paper link](https://openreview.net/pdf?id=cfGpIcOIa5)]

      传统 Inductive Logic Programming（ILP）系统 通常只针对小规模、语言偏见单一的任务设计，对于包含复杂语言偏差的大规模几何归纳任务表现有限。且大多数 ILP 系统需要专家手工设定语言 bias（例如定义可用谓词、递归深度等），这限制了 ILP 的自动化应用和普适化发展。因此，论文动机在于创建一个大规模、涵盖多种语言 bias 的合成数据集，推动研究者探索无需人工干预、可自动进行规则归纳的系统。数据集名称：GeoILP。

7. **MIRAGE: Evaluating and Explaining Inductive Reasoning Process in Language Models** [ICLR2025] [[paper link](https://arxiv.org/pdf/2410.09542)]

      MIRAGE数据集。

8.  **Code-Driven Inductive Synthesis: Enhancing Reasoning Abilities of Large Language Models with Sequences** [Arxiv2025] [[paper link](https://arxiv.org/abs/2503.13109)]
   
      提出了一种基于数列的类比推理合成数据管线，以code为呈现形式构建了一批SFT合成数据，有效的提高了LLMs的类比推理和code推理能力。

9.  **MTR:A Dataset Fusing Inductive, Deductive, and Defeasible Reasoning** [ACL2023] [[paper link](https://aclanthology.org/2023.findings-acl.640.pdf)]

     现有的数据集大多只关注单一类型的推理，提出了一个新的数据集MTR，旨在融合归纳推理、演绎推理和可废止推理，采用半自动方法生成数据集，包括逻辑生成、逻辑修正和自然语言生成。
【关系推理任务】【MTR】【准确率】【BiLSTM、BERT等】

10.  **InductionBench: LLMs Fail in the Simplest Complexity Class** [ACL2025] [[paper link](https://aclanthology.org/2025.acl-long.1287.pdf)]

     提出InductionBench，一个基于子正则函数层级（subregular hierarchy）的基准测试，通过生成不同复杂度的字符串转换任务（如ISL、L-OSL、R-OSL函数），评估LLM从输入-输出对中推断规则的能力。
【字符串到字符串的转换，要求模型从输入-输出对中推断规则】【动态生成的合成数据集】【精确率、召回率、兼容性】【LLMs】

11.  **Enhancing Large Language Models Against Inductive Instructions with Dual-critique Prompting** [NAACL2024] [[paper link](https://aclanthology.org/2024.naacl-long.299.pdf)]

     研究LLMs在处理包含错误前提或恶意意图的用户指令时的表现。构建INDUST基准：包含三种类型的归纳指令（事实检查指令FCI、基于错误前提的问题QFP、基于错误前提的创造性指令CIFP）。通过两个步骤增强模型对错误指令的识别能力：
用户批判（User-critique）：模型检查用户指令中的错误或有害信息。自我批判（Self-critique）：模型在生成回答时自我审查以避免传播错误内容。
【评估和改进LLMs对归纳指令的处理能力】【INDUST，LINDUST】【真实性（Truthfulness），帮助性（Helpfulness）】【LLMs】

12.  **CLUTRR:ADiagnostic Benchmark for Inductive Reasoning from Text** [EMNLP2019] [[paper link](https://aclanthology.org/D19-1458.pdf)]

     自然语言理解（NLU）在未见过的逻辑规则组合或噪声数据时表现不佳。引入基准测试（CLUTRR），评估模型在归纳推理和系统性泛化方面的能力。通过生成涉及虚构家族的短篇故事，要求模型推断未明确提及的两个家庭成员之间的关系。文本模型模型（如BERT、MAC）在系统性泛化上落后于直接处理符号化输入的GAT模型。
【短篇故事中推断亲属关系】【CLUTRR（半合成生成的故事）】【准确率】【文本模型、GAT】

13.  **A Benchmark for Semi-Inductive Link Prediction in Knowledge Graphs** [EMNLP2023] [[paper link](https://aclanthology.org/2023.findings-emnlp.713.pdf)]

     提出Wikidata5M-SI的基准测试，用于评估知识图谱中半归纳链接预测模型。该基准基于Wikidata5M数据集。任务类型：直推式、少量样本和零样本链接预测；上下文信息：从仅依赖KG结构、包含实体提及到包含详细描述。
【半归纳链接预测（SI-LP）】【Wikidata5M-SI】【MRR和Hits@K（K=1, 3, 10）】【图模型、文本模型、混合模型】


## Explanations and Explorations

1. **A New Neural Kernel Regime: The Inductive Bias of Multi-Task Learning** [NIPS2024] [[paper link](https://papers.nips.cc/paper_files/paper/2024/file/fdff3c4130c24c40c88aa41eb52d2a27-Paper-Conference.pdf)]
  
   多任务学习（MTL）的归纳偏置如何影响神经网络的泛化行为？。扩展神经核理论到MTL场景，定义多任务神经核（Multi-Task Neural Kernel, MTNK），刻画任务梯度交互对核演化的影响。【多任务回归与分类】【MultiMNIST,CelebA】【核相似性和任务性能】【MLP,ResNet】

2. **The Evolution of Statistical Induction Heads: In-Context Learning Markov Chains** [NIPS2024] [[paper link](https://papers.nips.cc/paper_files/paper/2024/file/75b0edb869e2cd509d64d0e8ff446bc1-Paper-Conference.pdf)]

     使用induction head来解释LLM的ICL内在机理。【ICL‑MC】【合成马尔可夫链序列数据集】【与uniform,unigram,bigram策略计算KL散度】【2‑layer attention‑only Transformer】
    
3. **Unveiling Induction Heads: Provable Training Dynamics and Feature Learning in Transformers** [NIPS2024] [[paper link](https://papers.nips.cc/paper_files/paper/2024/file/7aae9e3ec211249e05bd07271a6b1441-Paper-Conference.pdf)]

     Transformer在大规模语言模型中展现出强大的ICL能力，而“induction heads”作为关键结构已被经验发现，但其训练动力学与各组件如何协同构建这种机制仍缺乏理论性的解析。最后证明了证明在真实Transformer架构中，训练过程自发构建generalized induction head。【n‑gram马尔可夫链中的next‑token预测】【合成马尔可夫链序列数据集】【loss等】【2‑layer attention‑only Transformer】

4. **Inductive biases of multi-task learning and finetuning: multiple regimes of feature reuse** [NIPS2024] [[paper link](https://papers.nips.cc/paper_files/paper/2024/file/d7346ff79699b5bba26f8af89e700a95-Paper-Conference.pdf)]

     理解多任务学习（MTL）和微调（finetuning）中特征重用的内在机制。现有研究缺乏对这两种范式下模型参数如何动态变化、不同层特征如何被重用以及任务相似性如何影响性能的系统分析。【多任务分类,跨域分类】【MultiMNIST,CIFAR】【准确率】【MLP,resnet,ViT】
   
5. **Demystifying Inductive Biases for (Beta-)VAE Based Architectures** [ICML2021] [[paper link](http://proceedings.mlr.press/v139/zietlow21a/zietlow21a.pdf)]

    明确指出β‑VAE能disentangle的成功并非来自模型本身的能力，而是dataset varianc 结构与模型 objective 的偶然对齐。通过dataset perturbation实验呈现：当这种结构被破坏后，即factors labels仍保留，β‑VAE系统仍失败，说明评测需考虑bias而非模型普适性。强调开发更一般的disentangle方法需要设计更通用的 inductive bias或弱监督，而不能依赖dataset人为结构。【无监督disentangled表征学习】【dSprites和Shapes3D】【disentanglement metrics】【VAE系列】

6. **Fast Rates for Noisy Interpolation Require Rethinking the Effects of Inductive Bias** [ICML2022] [[paper link](https://proceedings.mlr.press/v162/donhauser22a/donhauser22a.pdf)]

    传统统计观点认为：过拟合（interpolation）噪声会导致泛化性能差，因此需要正则化。但现代深度或高维模型在噪声情况下仍能很好泛化，尤其是在无正则化下。作者认为这与“明确的强inductive bias不再总是优越，尤其在存在噪声时可能反而适得其反。他们提出：更弱一些（适中）的inductive bias可能带来更好泛化性能。【回归与分类任务】【MNIST/CNTK】【estimation error或分类error rate】【ML方法】

7. **Inductive Biases and Variable Creation in Self-Attention Mechanisms** [ICML2022] [[paper link](https://proceedings.mlr.press/v162/edelman22a/edelman22a.pdf)]

    该论文旨在从理论角度揭示Transformer自注意力模块的inductive bias。Inductive bias 的定义：模型的结构假设引导其在有限样本下偏向某类函数，从而实现泛化。在本作中，提出的sparse variable creation概念恰恰是Transformer的一种inductive bias：偏向于表示输入中少数子集上的稀疏依赖函数。该bias从理论上限制了模型的容量（norm-bound + covering bounds），并导致泛化样本复杂度只与s而非T线性相关，是一种隐含inductive偏好。

8. **The SSL Interplay: Augmentations, Inductive Bias, and Generalization** [ICML2023] [[paper link](https://openreview.net/pdf?id=d2aohFmZoB)]

    数据增强（Augmentations）和归纳偏置（Inductive Biases）在自监督学习中的作用。（1）卷积神经网络的平移不变性：卷积操作本身就带有一种自然的归纳偏置，即对平移的不变性。文章探讨了这种归纳偏置如何与数据增强方法（如裁剪、旋转）相互作用，帮助模型在训练过程中有效学习。（2）对称性、稀疏性等偏置：通过在网络设计中引入对称性、稀疏性等结构性归纳偏置，模型能够更加高效地从数据中提取信息。（3）数据增强中的归纳偏置：不同的增强方法（如颜色变换、旋转等）也引入了不同的归纳偏置，文章讨论了如何选择适合特定任务的增强策略，并通过归纳偏置优化模型性能。【自监督学习】【CIFAR-100, ImageNet等】【ACC】【CNN, Transformers等等】

9. **Position: The No Free Lunch Theorem, Kolmogorov Complexity, and the Role of Inductive Biases in Machine Learning** [ICML2024] [[paper link](https://openreview.net/pdf?id=EaJ7nqJ2Fa)]

    simplicity bias（即偏好简单假设），并将其视为一种inductive bias，主张神经网络结构与训练过程（尤其是 SGD）天然偏向于低Kolmogorov复杂度的函数解释，这本身即体现inductive bias的作用。

10. **Towards Understanding Inductive Bias in Transformers: A View From Infinity** [ICML2024] [[paper link](https://openreview.net/pdf?id=HOMXUneCTR)]

    为什么Transformer在训练样本有限的情况下也能泛化？论文核心即在探讨Transformer 的inductive bias：通过 GP prior（kernel）定义其偏好函数空间，即定义其 inductive bias；EK谱分解里的eigenvalues与eigenfunctions表征哪些函数更易学习，哪些难以学习，是inductive bias的具体体现；基于置换对称性的表示论结构，说明 Transformer 更倾向于学习对置换不变或高度对称的函数，这是模型的归纳偏好直接机制。

11. **What needs to go right for an induction head? A mechanistic study of in-context learning circuits and their formation** [ICML2024] [[paper link](https://openreview.net/pdf?id=O8rrXl71D5)]

    深入理解Transformer中in‑context learning（ICL）的机制，induction head是match‑and‑copy操作的attention head，用于识别上下文token并复制它们，是in‑context learning的关键induction operator。

12. **When Diffusion Models Memorize: Inductive Biases in Probability Flow of Minimum-Norm Shallow Neural Nets** [ICML2025] [[paper link](https://openreview.net/pdf?id=WD2CKUrxmx)]

    diffusion中最小范数解的选择实际上是一种inductive bias：模型偏好ℓ₂-minimization的denoiser，从而影响生成轨迹。Moonlight的score flow和probability flow的收敛特性体现出对训练样本结构的inductive preference：如正交几何结构引导流向训练点或组合点。early stopping time scheduler本质也是一种inductive bias：它决定模型 bias towards generalization（选择 manifold 点）或 memorization（停在训练样本）。

13. **Beyond Induction Heads: In-Context Meta Learning Induces Multi-Phase Circuit Emergence** [ICML2025] [[paper link](https://openreview.net/pdf?id=Xw01vF13aV)]

      先前的研究将诱导头（induction heads）与 ICL通过准确率的突然跃升联系起来，但这仅能解释在上下文中包含答案时的ICL。然而，实际应用中的ICL特性是模型能够从上下文中元学习如何解决任务，而不仅仅是复制上下文中的答案。如何在训练过程中获得这种能力仍然是一个未解之谜。本研究旨在通过分析模型在训练过程中的电路动态，实验性地阐明这种元学习能力是如何获得的。

14. **Stability and Generalization Capability of Subgraph Reasoning Models for Inductive Knowledge Graph Completion** [ICML2025] [[paper link](https://openreview.net/pdf?id=NE6Px91RkQ)]

      传统的图神经网络（GNN）在处理知识图谱（KG）补全任务时，通常假设训练和推理阶段的图结构相同。然而，在实际应用中，推理阶段可能会遇到新的实体和关系，这要求模型具备归纳能力。子图推理模型通过利用目标三元组周围的子图进行推理，已在归纳知识图谱补全（Inductive KGC）任务中取得了显著的实证成功。然而，这些模型的理论性质，如稳定性和泛化能力，尚未得到充分研究。因此，本文旨在首次从理论上分析子图推理模型的稳定性与其泛化能力之间的关系。本文通过引入稳定性度量和泛化界限，从理论上分析了子图推理模型的稳定性与其泛化能力之间的关系。

15. **The Inductive Bias of ReLU Networks on Orthogonally Separable Data** [ICLR2021] [[paper link](https://openreview.net/pdf?id=krz7T0xU9Z_)]

      理解 ReLU 神经网络的隐式归纳偏置（inductive bias）：即训练算法（gradient flow）在无限多零训练误差解中会偏向哪个，并决定其泛化能力。此前线性模型（如 Logistic regression）已有 max‑margin 偏置理论，但对于非线性的 ReLU 网络尚无类似明确定理。无论网络宽度多大，gradient flow 最终会使 neuron 聚焦于正负两个子集的 max-margin 划分方向，具有普适性。

16. **What they do when in doubt: a study of inductive biases in seq2seq learners** [ICLR2021] [[paper link](https://arxiv.org/abs/2006.14953)]

      seq2seq 模型广泛应用于翻译、对话等任务，但对其 归纳偏置（inductive bias） 仅有有限理解——即训练数据不足时它们会倾向哪种“规则”进行泛化？系统比较不同 seq2seq 架构（LSTM、Transformer、CNN）在面对高度歧义训练数据时的泛化偏好（即喜欢哪类规则）。不同架构之间表现出稳定且系统的偏好：LSTM 和 Transformer 更偏向 hierarchical induction（层次结构），CNN 更偏向 linear / sequential generalization（线性位置规则）。同时，CNN（以及 LSTM）更倾向 compositional reasoning（组合泛化），Transformer 则偏向 memorization。【四个合成任务】【四种模式合成任务对应数据集】【FPA, description length】【LSTM/CNN/Transformer】

17. **Predicting Inductive Biases of Pre-Trained Models** [ICLR2021] [[paper link](https://openreview.net/pdf?id=mNtmhaDkAr)]

      当前主流 预训练‑微调模型 在 NLP 任务中广受成功，但研究发现两种分析方法产生的结论常常矛盾：Probing classifier 表明预训练模型中能提取丰富的语言结构特征；Challenge set 分析却显示微调后的模型往往使用训练集中常见的启发式（spurious heuristic），未使用潜在语言知识。t：target feature（理论上应当依赖的结构语言特征，如语法结构）。s：spurious feature（与目标标签相关但非语法结构的启发式特征，如特定词语出现）。因此，作者提出假设：对于某个特征t，其是否被 fine‑tuned 模型采纳，取决于两个因素：在预训练表示中该特征的 extractability（可提取性）；在微调数据中该特征作为标签线索的 co‑occurrence frequency（证据量）。作者将 probing 中的 feature extractability 视为预训练模型的 inductive bias，即模型更容易使用的特征。【synthetic NLI/P probing tasks与自然语言推理challenge‑set】【多种合成数据与真实的NLI数据集】【测量是否模型依赖t还是s】【Bert和GPT系列】

18. **Deconstructing the Inductive Biases of Hamiltonian Neural Networks** [ICLR2022] [[paper link](https://arxiv.org/pdf/2202.04836)]

      物理启发型模型（如 Hamiltonian Neural Networks, HNN）因强 inductive bias 通常比普通神经网络更能泛化，但它们难以应用于不满足能量守恒或存在碰撞、摩擦等情境（如机器人与强化学习任务中常见）。作者质疑传统观点——认为 HNN 的优越表现源自对称几何结构或能量守恒；于是他们希望拆分 HNN 内部的偏置成分，理解究竟哪些 bias 在实际成功中起主导作用，以及如何在非理想系统中调整这类偏好。

19. **The Inductive Bias of In-Context Learning: Rethinking Pretraining Example Design** [ICLR2022] [[paper link](https://arxiv.org/pdf/2110.04541)]

    在大规模语言模型（NLM）的预训练中，通常将文本切割成连续的训练示例（chunk）进行处理。作者提出：模型对那些出现在同一个训练示例内部的句子或片段，能够学习更强的依赖关系；而跨示例的信息关联能力则显著弱於前者，这形成了一种所谓的 in‑context bias（上下文内偏好）。

20. **A theoretical study of inductive biases in contrastive learning** [ICLR2023] [[paper link](https://arxiv.org/pdf/2211.14699)]
    
    文章探索模型结构中隐含的归纳偏好对 contrastive 学习重要性。即模型架构自身（如可表达性、维度限制）对学习过程施加归纳偏差，从而影响最终的聚类结构与下游性能。

21. **Strong inductive biases provably prevent harmless interpolation** [ICLR2023] [[paper link](https://arxiv.org/pdf/2301.07605)]
    
    传统观点认为，对噪声的拟合会损害泛化，因此应该避免“插值”（interpolation）。然而在过参数模型中，许多模型即使完美拟合噪声仍能泛化良好（即 benign overfitting 或 harmless interpolation）。本文提出：是否能做到 harmless interpolation，强烈依赖学习器的归纳偏好强度——太强的 inductive bias 反而阻碍在噪声上的 harmless 插值，而偏弱的 inductive bias 则可能需要拟合部分噪声才能泛化良好。

22. **Geometric Inductive Biases of Deep Networks: The Role of Data and Architecture** [ICLR2025] [[paper link](https://arxiv.org/pdf/2410.12025)]
    
    几何不变性假设（GIH）：该假设揭示了神经网络在输入空间的几何结构具有架构依赖的诱导偏置，即在特定方向上的曲率保持不变。这种几何结构的演化决定了模型的决策边界和泛化能力，体现了模型在输入空间中的归纳偏置。

23. **Generalization through variance: how noise shapes inductive biases in diffusion models** [ICLR2025] [[paper link](https://arxiv.org/pdf/2504.12532)]

    扩散模型（diffusion models）为何能够超越训练集生成新样本？这是一个令人疑惑的现象，因为理论上训练目标是学习训练分布的 score 函数，且网络表达能力足够强大到可以完全记忆训练数据。作者认为关键在于 DSM（denoising score matching）目标的一个特性：它并不是直接逼近真实 score，而是一个带噪声、在期望上等于真实 score的“代理 score”。这种噪声带来的方差成为模型泛化的重要来源。于是提出了“through variance generalization（通过方差实现泛化）”这一现象。
    
24. **Combining Induction and Transduction for Abstract Reasoning** [ICLR2025] [[paper link](https://arxiv.org/pdf/2411.02272)]

    人类通常 先归纳出一个潜在函数（rule），再用它解释示例并预测新输入；而神经网络则可直接 对测试输入进行预测（transduction），无需明确函数构建。作者探讨一个核心问题：在样本极少时，**首先找到潜在函数是否更优？或者直接预测结果更有效？这两种范式究竟有何不同？验证它们各擅所长：Induction 擅长精确计算、多概念复合；Transduction 更擅长处理含有不确定、模糊感知规则的场景；演示这两种范式互补，并通过集成方式提升整体性能，接近人类水平。【ARC】【ARC为基础的合成任务】【准确率】【Induction和Transduction两种模型】

    
25. **Language Models Need Inductive Biases to Count Inductively** [ICLR2025] [[paper link](https://arxiv.org/pdf/2405.20131)]

      Counting（计数） 是多跳推理、算法模拟、形式语言识别的核心能力。现有语言模型在训练长度有限、测试长度超出训练范围（long‑length OOD）时往往无法正确计数。作者聚焦一个更基础的问题：不同架构的语言模型能否“归纳”计数原理，以实现长度泛化？哪些 inductive bias 是必须的？。传统 RNN 自带归纳偏好，可自然泛化计数；Transformer 需要依赖某种位置编码才能支撑 OOD 泛化 —— 说明这些位置编码本身定义了一种 inductive bias；实验还揭示：现代 RNN（为并行化训练设计）反而丢失这种 inductive bias，性能下降。【count】【对应数据集】【准确率】【RNN/LSTM, Transformers, S4以及 RWKV】

26. **Examining the Inductive Bias of Neural Language Models with Artificial Languages** [ACL2021] [[paper link](https://aclanthology.org/2021.acl-long.38.pdf)]  

      探究神经语言模型（如LSTM和Transformer）是否对特定类型的语言结构具有归纳偏置（Inductive Bias）。通过概率上下文无关文法（PCFG）生成内容相同但词序不同的平行句子，以困惑度作为性能指标。发现：LSTM：对所有词序变体表现相似，无明显偏置。Transformer：对某些词序（如OVS）表现显著更好，但其偏置与自然语言的普遍词序（如SOV/SVO）无关。
【预测下一个词】【64种人工语言（通过PCFG生成）】【困惑度（Perplexity）】【LSTM、Transformer】

27. **Coloring the Blank Slate: Pre-training Imparts a Hierarchical Inductive Bias to Sequence-to-sequence Models**  [ACL2022] [[paper link](https://aclanthology.org/2022.findings-acl.106.pdf)] 

      证明预训练seq2seq模型能够通过大规模预训练，获得层次化的归纳偏置，从而在句法转换任务中表现出对句子层次结构的敏感性。
【疑问句生成、将主动句转换为被动句】【使用上下文无关语法生成的英语和德语句子】【序列准确率、主助动词准确率、宾语名词准确率】【预训练的seq2seq模型】

28. **Measuring Inductive Biases of In-Context Learning with Underspecified Demonstrations**  [ACL2023] [[paper link](https://aclanthology.org/2023.acl-long.632.pdf)] 

      研究ICL的inductive biases，在任务定义模糊的情况下，LLMs倾向于依赖哪些特征进行预测。如GPT-3更倾向情感而非标点符号。尝试多种干预方法（自然语言指令、语义标签、模板解释、去歧义示例）来引导模型偏好特定特征。
【文本分类（情感分析、毒性检测、自然语言推理、问答）的模糊上下文学习】【情感分析：IMDb + Yelp；毒性检测：CivilComments；自然语言推理：MultiNLI；问答：BoolQ】【h-accuracy】【GPT-3】

29. **How to Plant Trees in LMs: Data and Architectural  Effects on the Emergence of Syntactic Inductive Biases**  [ACL2023] [[paper link](https://aclanthology.org/2023.acl-long.629.pdf)] 

      探索预训练过程中哪些因素（如模型架构和训练数据）会影响LMs在微调任务中表现出层次化句法归纳偏好。用不同参数的模型在多种数据集上实验。发现，模型深度更为关键，模型在更简单的数据（如儿童导向语料）上能更快形成层次化归纳偏好。
【句法转换任务】【预训练数据：CHILDES（儿童导向语料）、维基百科、简化版维基百科、C4网页文本; 微调数据：基于McCoy et al.】【序列准确率、主助动词准确率、宾语准确率】【不同超参数T5】

30. **Instruction Induction: From Few Examples  to Natural Language Task Descriptions** [ACL2023] [[paper link](https://aclanthology.org/2023.acl-long.108.pdf)] 
      
      验证大语言模型能否通过归纳示例中的模式，生成可解释的自然语言指令。方法是用大模型生成指令，通过执行准确率和语义相似度评估。经过指令调优的模型（InstructGPT）能较好生成指令，达到人类性能的65.7%。
【指令归纳（从示例生成指令）及指令执行评估】【24个任务（如复数化、反义词生成、形式化转换、句子相似度等），部分来自公开数据集（如GLUE、WordNet），部分自建（如数字求和、翻译任务）】【BERTScore（语义相似度）、执行准确率】【GPT-3系列】

31. **Too Big to Fail: Larger Language Models are Disproportionately Resilient  to Induction of Dementia-Related Linguistic Anomalies** [ACL2024] 
[[paper link](https://aclanthology.org/2024.findings-acl.380.pdf)] 
      研究LLMs是否模型规模越大，对注意力头的掩码（模拟神经退行性损伤）表现出更强的抵抗力，从而探索其在模拟阿尔茨海默病等神经退行性疾病语言异常中的潜力。发现大型语言模型表现出更强的抗干扰能力。
【检测阿尔茨海默病相关的语言异常】【ADReSS（阿尔茨海默病语音识别挑战数据集）和WLS（威斯康星纵向研究数据集）】【困惑度、分类准确率、AUC】【GPT-2】

32. **Identifying Semantic Induction Heads to Understand In-Context Learning** [ACL2024] [[paper link](https://aclanthology.org/2024.findings-acl.412.pdf)] 
      
      研究LLMs中注意力头如何编码高级语义关系，以增强对模型内部机制和上下文学习（ICL）能力的理解，从而提高模型的可解释性。提出“语义归纳头”，将ICL能力分为三个层次（损失减少、格式遵循、模式发现），并研究其与语义归纳头的相关性。
【分析注意力头对语义关系的编码能力，研究ICL能力的渐进发展】【AGENDA（知识图谱生成数据集）、SlimPajama（训练用数据集）】【关系指数、复制分数、格式准确率、预测准确率】【InternLM2-1.8B】

33. **Information Locality as an Inductive Bias for Neural Language Models**  [ACL2025] [[paper link](https://aclanthology.org/2025.acl-long.1357.pdf)] 
      
      针对神经LMs与人类认知偏好的对齐争议，提出局部熵作为指标，通过扰动自然语言和合成语言实验，证明模型与人类共享“信息局部性”这一归纳偏置。提出m-local entropy框架，通过控制变量实验验证局部统计结构对神经LMs学习难度的影响。
【语言模型学习难度评估】【自然语言：BLLIP语料库、合成语言：PFSA生成的合成数据集】【下一符号交叉熵、KL散度】【LSTM、Transformer】

34. **Do Robot Snakes Dream like Electric Sheep?  Investigating the Effects of Architectural Inductive Biases on Hallucination**  [ACL2025] [[paper link](https://aclanthology.org/2025.findings-acl.60.pdf)] 
      
      针对LLMs幻觉问题，从架构的归纳偏差角度出发，对比不同模型在多样任务中的表现，揭示其与幻觉类型的关联性。方法：系统评估多种架构LLMs在标准化幻觉任务中的行为差异，结合规模与微调分析。
【闭卷问答、摘要生成、阅读理解、指令跟随、幻觉检测、事实核查】【NQ-Open、TriviaQA、TruthfulQA、PopQA、XSUM、CNN/DM、RACE、SQuADv2、MemoTrap、IFEval、FaithDial、HaluEval、FEVER等】【精确匹配（EM）、准确率（Accuracy）、Rouge-L等】【Transformer类：LLaMA2/3、Gemma、Falcon、Mistral、Mixtral；循环/混合类：Mamba、RecurrentGemma、FalconMamba、Jamba、RWKV/Finch】

35. **Can Input Attributions Explain Inductive Reasoning  in In-Context Learning?** [ACL2025] [[paper link](https://aclanthology.org/2025.findings-acl.1092.pdf)] 
      
      探讨输入归因（IA）能否有效解释LLM在ICL中的归纳推理过程，提出设计包含歧义示例和唯一关键示例的ICL任务，比较四种IA方法和基线方法（如注意力权重、自生成解释）在识别关键示例上的表现。
【合成归纳推理任务】【自建合成数据集】【Top-1和Top-2归因准确率】【Llama-2-7B/13B、Gemma-2-2B/9B/27B、Mistral-7B】

36. **GCG-Based Artificial Languages  for Evaluating Inductive Biases of Neural Language Models**  [ACL2025] [[paper link](https://aclanthology.org/2025.conll-1.35.pdf)] 
      
      探究LMs是否对高频语法模式（如特定词序）存在归纳偏好，使用PCFG生成人工语言而无法涵盖部分词序和复杂句法结构。提出通过广义范畴语法（GCG）构建更丰富的人工语言，通过困惑度分析LSTM和Transformer对词序的偏好动态。
【评估神经LMs在不同词序人工语言上的学习表现】【GCG-ALs：96种人工语言（含VSO、OSV等新增词序）】【困惑度（PPL）】【LSTM、Transformer】

## Evaluations

1. **Is Forgetting Less a Good Inductive Bias for Forward Transfer?** [ICLR2023] [[paper link](https://arxiv.org/pdf/2211.14699)]
    
    连续学习的核心目标之一是模型能从过去任务中积累知识，以更高效地学习新任务。然而，最近研究发现：减少灾难性遗忘（catastrophic forgetting）并不一定能带来正向迁移（forward transfer）的提升。这可能源自测量 forward transfer 的方式不当。作者认为，正确的 forward transfer Measure 应当聚焦于 在固定表示下新任务的适应难易程度，而不是不同任务训练策略之间的干扰。在训练序列中每到一个新任务时，冻结当前特征提取器 (feature extractor Φ)，只用少量样本学习线性分类器（k-shot probing），评估在下一任务上的泛化准确率。这里的 inductive bias 指：在连续学习过程中，对保留过去任务知识的偏好，可以提升未来任务的迁移效率。

## Methods

1. **A Sparse Interactive Model for Matrix Completion with Side Information** [NIPS2016] [[paper link](https://papers.nips.cc/paper_files/paper/2016/file/093b60fd0557804c8ba0cbf1453da22f-Paper.pdf)]
  
   一个inductive model用作矩阵补全任务。【矩阵补全】【矩阵补全数据集】【RMSE/MAE】【低秩方法与残差模型】

2.  **Neural Program Meta-Induction** [NIPS2017] [[paper link](https://arxiv.org/pdf/1710.04157)]

      集中在Neural Program Induction任务当中，对于其他域少量训练样本，使用知识迁移的方法，提升模型泛化能力。【Neural Program Induction】【人工构建Karel程序任务集】【I/O示例预测准确率】【各种设置下的transformer模型】

3. **Adapted Deep Embeddings: A Synthesis of Methods for k-Shot Inductive Transfer Learning** [NIPS2018] [[paper link](https://arxiv.org/pdf/1805.08402)]

   有关inductive transfer learning的一种方法。【K-ITL任务】【MNIST（数字识别）, Omniglot（手写字符）, Isolet（语音字母识别）,tinyImageNet（图像分类子集）】【准确率】【CNN模型】
   
4. **Library Learning for Neurally-Guided Bayesian Program Induction** [NIPS2018] [[paper link](https://papers.nips.cc/paper_files/paper/2018/file/7aa685b3b1dc1d6780bf36f7340078c9-Paper.pdf)]

   有关Program Induction任务，现有方法依赖于手工设计的DSL（领域特定语言），通用性和扩展性受限。解决方法是：构建算法 EC²，从任务中自动探索程序；压缩并归纳出可复用的DSL；学习神经网络来辅助搜索。【Neural Program Induction】【三个域数百个任务】【任务解决率等】【不同设定下的模型】

5. **On the Inductive Bias of Neural Tangent Kernels** [NIPS2019] [[paper link](https://papers.nips.cc/paper_files/paper/2019/file/c4ef9c39b300931b69a36fb3dbb8d60e-Paper.pdf)]

   对于模型优化过程神经切线核（NTK）的inductive bias的探索，本文给出了一种基于核函数的提高方法。【图像分类】【CIFAR-10, MNIST】【准确率】【CNN模型】
   
6. **Provable Non-linear Inductive Matrix Completion** [NIPS2019] [[paper link](https://papers.nips.cc/paper_files/paper/2019/file/ce5193a069bea027a60e06c57a106eb6-Paper.pdf)]

   是一种indcutive matrix补全的机器学习方法。【矩阵补全】【Movielens‑100K/Movielens‑10M】【RMSE/MAE】【矩阵补全模型】
   
7. **Discovering Symbolic Models from Deep Learning with Inductive Biases** [NIPS2020] [[paper link](https://arxiv.org/pdf/2006.11287)]

   通过引入强先验偏置和符号回归，从训练好的深度模型中提取出明确的物理规律和符号模型，以GNN模型类比物理反应。【物理建模领域】【粒子系统，暗物质模拟】【模拟准确性】【GNN模型】
   
8. **Latent Template Induction with Gumbel-CRFs** [NIPS2020] [[paper link](https://arxiv.org/pdf/2011.14244)]

   提出了一种结构化变分自编码器（Structured Variational Autoencoder）模型，利用连续松弛的条件随机场（CRF）推理机制，自动从文本数据中归纳出控制句子生成结构的潜在模板。【文本生成】【数据到文本生成R4R和无监督同义句生成ParaNMT】【BLEU, ROUGE, Success@1】【CRF模型】

9. **Fine-grained Generalization Analysis of Inductive Matrix Completion** [NIPS2021] [[paper link](https://proceedings.neurips.cc/paper_files/paper/2021/file/d6428eecbe0f7dff83fc607c5044b2b9-Paper.pdf)]

   旨在缩小归纳矩阵补全在理论分析方面与标准矩阵补全之间的差距：此前在无分布假设条件下，IMC 的样本复杂度最高达 $O(rd^2)$，作者努力证明更优的边界，并希望引入更高效的“带权迹范数”正则策略。【矩阵补全】【推荐数据】【理论界与实证loss】【IMC/ATR】

10. **Leveraging the Inductive Bias of Large Language Models for Abstract Textual Reasoning** [NIPS2021] [[paper link](https://arxiv.org/abs/2110.02370)]

     预训练的大型语言模型（如T5、GPT-3）是否具备对抽象文本推理任务（如容器操作、导航路径推断）的归纳偏置？微调 T5，设计 container/navigation/composite 任务，对比tabula rasa和英语vs猫语模板。【NLP任务泛化】【每个任务构造成训练集、插值和外推测试集，用于各类泛化测试（基数、符号、组合）】【Exact match,BLEU】【T5】

11. **Tailoring: encoding inductive biases by optimizing unsupervised objectives at prediction time** [NIPS2021] [[paper link](https://arxiv.org/abs/2009.10623)]

     监督学习中，辅助损失（auxiliary loss，如物理守恒、对比学习约束等）只在训练阶段使用，会带来泛化缺口，并且训练优化的是合并目标而非关注的任务损失。通过在inference时执行unsupervised优化，让inductive bias可对每个输入样本直接生效。【多任务】【多数据】【多指标】【多模型】

12. **Open Rule Induction** [NIPS2021] [[paper link](https://arxiv.org/pdf/2110.13577)]

     传统基于知识库（KB）的规则归纳只能从已有实体和关系中挖掘模式，表达能力有限；而当前基于语言模型（LM）的规则生成，如 Comet，依赖人工标注的规则，缺乏真正“归纳”能力，生成结果受限于训练样本，难以创造真实通用规则。提出 Open Rule Induction（ORI）问题：给定前提句子如 (x, rp, y)，从 LM 中挖掘 top‑k 个有效的结论 (x, rh, y) 规则，自动诱导的规则。【Open Rule Induction, 关系抽取】【自动生成开放规则与公开关系数据】【质量,F1】【BART】

13. **ViTAE: Vision Transformer Advanced by Exploring Intrinsic Inductive Bias** [NIPS2021] [[paper link](https://arxiv.org/pdf/2106.03348)]

     ViT将图像拆成1D token序列，缺乏CNN的内在归纳偏置，特别是在局部结构建模与多尺度变化上的能力。结果它需要极大规模数据和长训练才能“间接”学会这些偏置。本文将CNN的 locality和scale‑invariance偏置直接引入ViT。【图像分类和下游任务】【ImageNet-1K和下游数据集】【top1等】【ViT系列】
    
14. **INDIGO: GNN‑Based Inductive Knowledge Graph Completion Using Pair‑Wise Encoding** [NIPS2021] [[paper link](https://papers.nips.cc/paper_files/paper/2021/file/0fd600c953cde8121262e322ef09f70e-Paper.pdf)]

     GNN用类比的思路获取新实体的表示。【KG补全】【GraIL-BM等】【F1等】【GNN系列】

15. **Towards Open‑World Feature Extrapolation: An Inductive Graph Learning Approach** [NIPS2021] [[paper link](https://arxiv.org/abs/2110.04514)]

     为了使得训练阶段的特征外推到测试阶段新的特征，利用GNN每步随机抽取k个特征构建子图以训练外推能力。【分类和CTR任务】【对应数据集】【acc和ctr】【GNN系列】

16. **Using Natural Language and Program Abstractions to Instill Human Inductive Biases in Machines** [NIPS2022] [[paper link](https://papers.nips.cc/paper_files/paper/2022/file/0113ef4642264adc2e6924a3cbbdf532-Paper-Conference.pdf)]

     人类自然语言任务描述和程序归纳得到的抽象表示作为额外监督，可使训练出的agents更具人类式归纳偏置。【Meta-RL格式的网格游戏】【GSP人类采样网格和对照网络】【human priors分布和control分布对比】【meta‑RL的各种设定】

17. **Inductive Logical Query Answering in Knowledge Graphs** [NIPS2022] [[paper link](https://papers.nips.cc/paper_files/paper/2022/file/6246e04dcf42baf7c71e3a65d3d93b55-Paper-Conference.pdf)]

     同样是现实知识图随着新增节点/边变化，而使这些过去的模型不能泛化。该论文提出归纳式复杂查询回答任务，即在infer时遇到全新实体，仍能正确回答逻辑查询。【一阶逻辑查询】【FB15k‑237派生数据集】【Hits@10】【GNN系列】

18. **Learning Rule-Induced Subgraph Representations for Inductive Relation Prediction** [NIPS2023] [[paper link](https://papers.nips.cc/paper_files/paper/2023/file/0b06c8673ebb453e5e468f7743d8f54e-Paper-Conference.pdf)]

     解决传统方法无法处理未见过的实体或关系的问题（即inductive setting）。利用规则诱导的子图结构（rule-induced subgraphs）捕捉局部语义模式，从而提升模型在归纳场景下的泛化能力。【归纳式关系预测】【标准归纳数据集WN18RR-Ind、FB15k-237-Ind】【MRR（Mean Reciprocal Rank）、Hit@1/3/10】【归纳模型】

19. **Efficient Data Subset Selection to Generalize Training Across Models: Transductive and Inductive Networks** [NIPS2023] [[paper link](https://papers.nips.cc/paper_files/paper/2023/file/0f25eb6e9dc26c933a5d7516abf1eb8c-Paper-Conference.pdf)]

     当前机器学习模型训练通常依赖大量数据，但并非所有数据对模型泛化能力都有同等贡献。直推式（Transductive）方法（如传统监督学习）依赖固定数据集，难以适应新数据分布；归纳式（Inductive）方法（如元学习）虽然能适应新任务，但计算成本高。文章提出一种高效数据子集选择方法，旨在同时优化直推式和归纳式模型的泛化能力，减少训练数据需求，提高计算效率。【数据高效学习, 跨模型泛化】【直推式：CIFAR-10, ImageNet; 归纳式：Mini-ImageNet（元学习基准）, OGB（图神经网络基准）】【ACCh和泛化差距】【直推式：ResNet, ViT。归纳式：MAML（元学习）, GIN】

20. **Learning from Both Structural and Textual Knowledge for Inductive Knowledge Graph Completion** [NIPS2023] [[paper link](https://papers.nips.cc/paper_files/paper/2023/file/544242770e8333875325d013328b2079-Paper-Conference.pdf)]

     传统知识图谱补全泛化性差，仅利用图谱结构信息（如TransE）的方法难以处理新实体的语义关联，仅依赖文本描述（如BERT编码）的方法忽略图谱的拓扑结构，导致推理能力不足。所以提出一种联合结构与文本知识的归纳式KGC框架。【知识图谱补全】【WN18RR-Ind,FB15k-237-Ind】【MRR（平均倒数排名）, Hit@1/3/10】【直推式：TransE,RotatE,ComplEx。归纳式：GraIL,CoMPILE,Meta-KGC】

21. **C-Disentanglement: Discovering Causally-Independent Generative Factors under an Inductive Bias of Confounder** [NIPS2023] [[paper link](https://papers.nips.cc/paper_files/paper/2023/file/7ca55c8276acf1f0aa996cd3622d1df4-Paper-Conference.pdf)]

     当前大多数表征学习认为观察数据是由多个生成因子生成的，且这些因子应该是因果可解耦的——即一个因子的变化不应影响另一个。然而，绝大多数工作忽略了生成因子之间可能存在的混杂变量（confounder），而只追求统计独立，却无法识别那些在观测数据中存在相关性的真实因果因素将先验知识作为可观测标签引入inductive bias。这个 bias 是指用领域知识提供的混淆变量信息，用于在训练中分区拟合并强制条件独立。【图像重构,分类任务】【3dshape,Candle,CelebA】【重构误差和因果指标】【VAE系列】

22. **An Inductive Bias for Tabular Deep Learning** [NIPS2023] [[paper link](https://papers.nips.cc/paper_files/paper/2023/file/8671b6dffc08b4fcf5b8ce26799b2bef-Paper-Conference.pdf)]

     引入一种偏向低频率平滑的归纳偏置以解决表格数据的目标函数通常非常不规则的问题。【表格任务】【表格数据集】【分类准确率】【一些MLP】

23. **Scaling MLPs: A Tale of Inductive Bias** [NIPS2023] [[paper link](https://papers.nips.cc/paper_files/paper/2023/file/bf2a5ce85aea9ff40d9bf8b2c2561cae-Paper-Conference.pdf)]

     探索MLP在视觉任务上随着规模增长的极限，评估在无 inductive bias的条件下，性能是否能被计算资源代偿。论文核心反复强调：MLP不具备视觉偏置，即完全依赖平铺像素信息处理，没有空间结构inductive bias；然而结果表明，通过规模（compute）可以弥补这一缺陷，验证了“scale beats bias”这一命题。【图像分类】【ImageNet‑21k】【分类准确率】【一些MLP】

24. **Mars: Situated Inductive Reasoning in an Open‑World Environment** [NIPS2024] [[paper link](https://papers.nips.cc/paper_files/paper/2024/file/1fb6d0b52f5e41b11392841a66dbfe7d-Paper-Datasets_and_Benchmarks_Track.pdf)]

     当前LLM和RL模型依赖大量“预先存储的知识”，但在新环境中难以灵活应对。作者提出“情境归纳推理（situated inductive reasoning）”：模型需要在开放世界中通过交互从零开始归纳出规则，并在决策中灵活应用这些新知识。【开放世界任务】【Mars】【Reward,Success Rate】【LLM】

25. **How Far Can Transformers Reason? The Globality Barrier and Inductive Scratchpad** [NIPS2024] [[paper link](https://papers.nips.cc/paper_files/paper/2024/file/3107e4bdb658c79053d7ef59cbc804dd-Paper-Conference.pdf)]

     通过类比Scratchpad技术实现LLM的长OOD任务泛化。【token序列合成任务】【Cycle,Parity与Addition】【训练效率和长度泛化性】【GPT2-style】

26. **Amortized Active Causal Induction with DeepReinforcement Learning** [NIPS2024] [[paper link](https://papers.nips.cc/paper_files/paper/2024/file/4e2c6423d724370b36c3a7612f25b78c-Paper-Conference.pdf)]

     当前的因果结构学习（causal structure learning）通常依赖：对每个数据集进行单独图结构推断（通常需慢速似然或复杂后验算法）；基于推断出的图再贪婪选择干预实验，效率低、对分布变更敏感。论文提出CAASL方法，使用更少干预获得更准确的因果图，适配不同图结构分布、干预类型，甚至更高维环境。【干预设计因果学习】【Gaussian SCM】【Returns,结构指标】【Random（随机干预）,Observational（继续采集观测数据）,DiffCBED等】

27. **On the Inductive Bias of Stacking Towards Improving Reasoning** [NIPS2024] [[paper link](https://papers.nips.cc/paper_files/paper/2024/file/837bc5db12f3d394d220815a7687340c-Paper-Conference.pdf)]

     高效训练的stacking策略（如渐进式层级增长）已被用于加速大规模语言模型结构训练，但这类方法除了提高训练效率外，对模型的归纳偏置影响尚未充分研究本文目标除了探索stacking的效率提升外，更聚焦于其是否能内隐地增强模型的推理能力。（本文偏FLOPS和perplexity等底层）【UL2 objective】【开放式阅读理解,数学等】【准确率】【LLM】

28. **Diffusion Model with Cross Attention as an Inductive Bias for Disentanglement** [NIPS2024] [[paper link](https://papers.nips.cc/paper_files/paper/2024/file/9647157086adf5aa2c0217fb7f82bb19-Paper-Conference.pdf)]

     利用扩散模型（Diffusion Models）结合交叉注意力（Cross Attention），作为一种inductive bias，提高模型在特定任务中的解耦能力。【生成任务】【CIFAR-10等】【FID,IS】【扩散模型】
    
29. **Explicit Inductive Bias for Transfer Learning with Convolutional Networks** [ICML2018] [[paper link](https://arxiv.org/abs/1802.01483)]

     预训练之后finetune也会有所遗忘，通过显式的正则化机制，在 fine‑tuning 过程中保持与预训练模型的相似性，从而增强迁移性能并减少遗忘。【分类任务】【ImageNet、Places‑365等】【准确率】【CV模型】
    
30. **Fast and Sample Efficient Inductive Matrix Completion via Multi-Phase Procrustes Flow** [ICML2018] [[paper link](https://proceedings.mlr.press/v80/zhang18b/zhang18b.pdf)]

     多阶段非凸梯度优化做矩阵补全。【矩阵补全】【多标签学习，基因-疾病预测】【相对误差】【矩阵补全模型】

31. **Inductive Two-layer Modeling with Parametric Bregman Transfer** [ICML2018] [[paper link](https://proceedings.mlr.press/v80/ganapathiraman18a/ganapathiraman18a.pdf)]

     实现带有理论保证的全局最优或近似最优两层网络学习。 模型学习的是参数𝑊,𝑈，不需要访问训练样本进行推断。【分类任务】【G241N等】【ACC】【两层网络模型】

32. **Inductive Relation Prediction by Subgraph Reasoning** [ICML2020] [[paper link](https://proceedings.mlr.press/v119/teru20a/teru20a.pdf)]

     现有实体嵌入的方法无法处理新的实体，本文能够从局部子图结构中归纳出关系规则，并推广到未见实体和新图结构。【实体预测】【WN18RR,FB15k-237,NELL-995】【AUC,hit】【GNN模型】
    
33. **ConViT: Improving Vision Transformers with Soft Convolutional Inductive Biases** [ICML2021] [[paper link](http://proceedings.mlr.press/v139/d-ascoli21a/d-ascoli21a.pdf)]

    CNN拥有硬编码的局部性和权重共享等归纳偏置，在小数据集上样本效率非常高，却因表达局限而在大数据上表现逐渐成为性能瓶颈。ViT放弃卷积硬偏置，依赖全局自注意力来捕捉视觉特征，在大规模预训练下效果卓越，但在中小规模数据时容易欠拟合或者过拟合。本文使用了Gated Positional Self-Attention（GPSA）方法，提出ConViT架构解决这一类问题。【图像分类】【ImageNet-1k】【分类准确率】【ConViT】

34. **LIME: Learning Inductive Bias for Primitives of Mathematical Reasoning** [ICML2021] [[paper link](http://proceedings.mlr.press/v139/wu21c/wu21c.pdf)]

    提出通过设计专门的合成任务（synthetic tasks），用于给模型注入“数学推理”的 inductive bias，而非通过改变架构，形成一种新型的数学预训练范式——LIME。【数学推理】【IsarStep等】【top1 top10】【Transformers】

35. **Towards Open-World Recommendation: An Inductive Model-based Collaborative Filtering Approach** [ICML2021] [[paper link](http://proceedings.mlr.press/v139/wu21j/wu21j.pdf)]

    传统协同过滤（Collaborative Filtering）通过矩阵分解学习用户和物品的latent embedding，但这是典型的transductive方法，无法处理训练中未见的新用户，也无法即时推荐（on‑the‑fly）新来访用户。现实推荐场景存在大量的few‑shot用户（极少评分）或zero‑shot用户，传统方法难以应对。本文提出Relation‑learning模块归纳计算用户query特征。【推荐系统】【 MovieLens‑1M,MovieLens‑10M等】【RMSE等推荐指标】【推荐模型】

36. **Cycle Representation Learning for Inductive Relation Prediction** [ICML2022] [[paper link](https://proceedings.mlr.press/v162/yan22a/yan22a.pdf)]

    训练集与测试集实体不重叠，模型不能借助训练期间看到的实体embedding，仅能通过关系模式（rules）来泛化至测试图中全新实体；方法采用 entity-agnostic learning，重点学习循环结构（cycles）及其组合，而不是具体实体embedding。【关系预测】【FB15k‑237, NELL‑995, WN18RR等】【AUC‑PR, Hits@10】【GNN】

37. **Inductive Matrix Completion: No Bad Local Minima and a Fast Algorithm** [ICML2022] [[paper link](https://proceedings.mlr.press/v162/zilber22a/zilber22a.pdf)]

    一种基于优化的矩阵补全方法。【矩阵补全】【相关数据集】【rel‑RMSE】【相关基线】

38. **Neuro-Symbolic Hierarchical Rule Induction** [ICML2022] [[paper link](https://proceedings.mlr.press/v162/glanois22a/glanois22a.pdf)]

    该论文聚焦于 Inductive Logic Programming (ILP) 问题——从一组正负样本和背景知识中自动学习一阶逻辑规则。传统ILP方法依赖于符号组合搜索，效率低、难以扩展；而现有神经符号方法虽然可微分，但通常缺乏通用而高效的结构。作者提出HRI模型，结合元规则（meta-rules）结构化假设与可学习嵌入，旨在获得高效、可解释、且具组合泛化能力的规则归纳方法。【ILP】【相关数据集】【成功率】【相关基线】

39. **PAC-Net: A Model Pruning Approach to Inductive Transfer Learning** [ICML2022] [[paper link](https://proceedings.mlr.press/v162/myung22a/myung22a.pdf)]

      fine‑tune容易在目标任务中过拟合，遗忘源任务核心知识（例如物理规律）；当模型高度过参数化时，修剪后仍能保留源任务性能，剪枝提供了inductive bias这为 transfer learning 提供新的思路；以同时保留源知识并适应目标任务。【分类与回归任务】【Friedman和CelebA等】【RMSE和ACC等】【相关基线】
    
40. **Parametric Visual Program Induction with Function Modularization** [ICML2022] [[paper link](https://proceedings.mlr.press/v162/duan22c/duan22c.pdf)]

      视觉程序归纳（Visual Program Induction）旨在从图像或视觉场景生成可执行程序，但现有方法大多只能应对非参数化的原始函数（无参数或实例极少），难以处理复杂视觉场景中具有大量参数和多变属性的原始函数。作者发现：对于parametric primitive functions，即具有丰富且异构参数的函数，其变体数量极多（一个函数可能超过 10⁴ 种变体），使得动作空间爆炸，模型难以有效学习与归纳。因此论文提出Parametric Visual Program Induction的新任务，并提出Function Modularization 的方法，以应对动作空间庞大与函数间复杂相关性挑战。【VPI】【Pixel‑Grid dataset等】【ACC】【三个模块叠加的模型】

41. **Understanding Contrastive Learning Requires Incorporating Inductive Biases** [ICML2022] [[paper link](https://proceedings.mlr.press/v162/saunshi22a/saunshi22a.pdf)]

      为对比学习引入归纳偏置。【分类任务】【CIFAR-100, ImageNet】【ACC】【图像对比学习模型】
    
42. **Graph Inductive Biases in Transformers without Message Passing** [ICML2023] [[paper link](https://openreview.net/pdf?id=HjMdlNgybR)]

      文章提出了一种新方法，在Transformer中引入图的归纳偏置，具体来说，利用位置编码（Positional Encoding）和图结构编码来捕捉图中的节点关系，而不依赖于传统的消息传递机制。【图表示学习】【Cora,Citeseer,PubMed等】【分类准确率】【Transformers,GNN】
    
43. **INGRAM: Inductive Knowledge Graph Embedding via Relation Graphs** [ICML2023] [[paper link](https://openreview.net/pdf?id=OoOpO0u4Xd)]

      文章提出了INGRAM方法，它通过引入关系图来为每种关系构建一个独立的图结构，并通过该图来嵌入知识图谱中的实体和关系。通过提出一种inductive方法，使得模型能够在遇到新关系或实体时，无需重新训练整个模型，而是能够快速适应新信息。【知识图谱嵌入】【FB15k,WN18等】【Hits@K】【INGRAM模型】

44. **Meta-Learning the Inductive Bias of Simple Neural Circuits** [ICML2023] [[paper link](https://openreview.net/pdf?id=757L5dtuah)]

      文章提出了一种基于元学习的框架来自动学习神经网络的归纳偏置。具体来说，通过设计一个简单的神经电路模型，并通过元学习算法，使得网络能够根据不同的任务自动调整其归纳偏置。【元学习】【Omniglot,Mini-ImageNet】【ACC】【神经电路模型】

45. **SLOG: An Inductive Spectral Graph Neural Network Beyond Polynomial Filter** [ICML2024] [[paper link](https://openreview.net/pdf?id=0SrNCSklZx)]

      通过对子图进行采样并仅在子图上应用实值阶滤波器，避免对整图进行谱分解，使模型能够处理图中未见过的新节点。这种设计使 SLOG 具备真正的归纳式推理能力。【图节点分类】【图数据集】【ACC】【SLOG模型】

46. **Tripod: Three Complementary Inductive Biases for Disentangled Representation Learning** [ICML2024] [[paper link](https://openreview.net/pdf?id=0iXp5P77ho)]

      论文关注为什么无监督表示学习难以实现因子化disentanglement。前人已有多种 inductive bias，如 latent quantization、latent independence（total correlation）和decoder的Hessian正则化，单独使用时都有助益，但组合时往往难以训练、性能没有实质提升。动机即是：能否将三种互补的 inductive bias 有效融合在一个autoencoder中，借此精确限定latent空间结构，从而实现更可靠的disentangled表征学习。 inductive bias来引导模型disentanglement。三条腿分别作用于：latent空间压缩（量化）、latent变量集体独立性、decoder function中latent相互影响最小化，分别对应encoder、latent空间、decoder的inductive bias体现。【无监督的disentangled表征学习】【四个图像disentanglement数据集】【InfoMEC】【Tripod】

47. **Confronting Reward Overoptimization for Diffusion Models: A Perspective of Inductive and Primacy Biases** [ICML2024] [[paper link](https://openreview.net/pdf?id=v2o9rRJcEv)]

      利用diffusion模型的temporal inductive bias：确保reward优化与模型多步生成过程对齐，避免仅关注最终图像评分的偏差。【文生图】【Stable Diffusion v1.4】【sample efficiency】【TDPO】

48. **Inductive Moment Matching** [ICML2025] [[paper link](https://openreview.net/pdf?id=pwNSUo7yUb)]

      现有的扩散模型（Diffusion）和流匹配模型（Flow Matching）虽然能生成高质量图像，但推理时需要大量采样步骤，导致推理慢。模型通过自身生成的样本来匹配目标分布，类似数学归纳法自我引导学习。【文生图】【ImageNet‑256×256和CIFAR‑10】【FID】【IMM】

49. **Customizing the Inductive Biases of Softmax Attention using Structured Matrices** [ICML2025] [[paper link](https://openreview.net/pdf?id=Roc5O1ECEt)]

      如何定制attention的归纳偏好，既能处理高维输入，又能显式编码邻近依赖信息，从而提升性能。本文实现了BTT与MLR分别提供对输入中高维依赖结构和距离依赖结构的inductive bias。【in‑context回归任务】【高维输入回归数据集】【MSE】【Transformer】

50. **iN2V: Bringing Transductive Node Embeddings to Inductive Graphs** [ICML2025] [[paper link](https://openreview.net/pdf?id=BYakLzKJDz)]

      传统的图节点嵌入方法，如 Node2Vec（N2V），通常依赖于图的整体结构进行训练，因此属于传递性（transductive）方法，即在训练期间需要访问整个图，包括测试节点。然而，在实际应用中，图结构可能会发生变化，出现新的节点和边，这些新的节点在训练期间是不可见的。因此，如何将传递性节点嵌入方法扩展到归纳性（inductive）设置，使其能够为训练期间未见过的节点生成有效的嵌入。【图节点分类】【Cora,Citeseer和PubMed等等】【ACC】【GNN】

51. **GenZSL: Generative Zero-Shot Learning Via Inductive Variational Autoencoder** [ICML2025] [[paper link](https://openreview.net/pdf?id=AYxiZfJN9V)]

      生成式零样本学习（Generative ZSL）常借助GAN、VAE 等生成视觉特征，但多数方法 直接从强语义向量生成样本，对新类别泛化能力有限。本文目标是通过从相似已见类“归纳”出新类样本。本文提出GenZSL：一类具有归纳能力的变分自编码器模型。它不从零生成目标类样本，而是通过从相似已见类中“归纳（induct）”合成新类样本，模拟人类概念迁移。【图零样本分类】【AwA2等等】【ACC】【GenZSL模型】

52. **Deep Gaussian Embedding of Graphs: Unsupervised Inductive Learning via Ranking** [ICLR2018] [[paper link](https://openreview.net/pdf?id=r1ZdKJ-0W)]

      传统图嵌入方法把每个节点表示为低维向量，但这忽略了“表示的不确定性” —— 即当节点信息有冲突或多样性时，单一点向量难以表达这一不确定程度。此外，现有大多数方法为transductive（传导式），训练时不能自然泛化到新的、未见过的节点，需要重新训练或依赖其结构信息。作者因此提出一种将节点嵌入为高斯分布的方法，并结合属性信息，实现不依赖已有图结构也能表示新节点。【链接预测，节点分类】【Cora,DBLP等等】【AUC,F1】【G2G模型】

53. **DEEP REINFORCEMENT LEARNING WITH RELATIONAL INDUCTIVE BIASES** [ICLR2019] [[paper link](https://openreview.net/pdf?id=HkxaFoC9KQ)]

      传统的model‑free深度强化学习（如 CNN+A2C/DQN）在样本效率、泛化能力以及可解释性方面存在缺陷，尤其难以在组合性变化的环境中迁移和泛化。本文将图像输入编码为一组实体向量，然后通过多头点积自注意力模块进行迭代推理，学习实体间的关系。这相当于一个图神经网络或Transformer风格的关系推理层。生成关系感知的表示后，再由actor‑critic模型输出策略与价值估计。【Box‑World，星际2】【这俩数据集】【游戏中得分】【自己训练的Relational Agent】

54. **An Inductive Bias for Distances: Neural Nets that Respect the Triangle Inequality** [ICLR2020] [[paper link](https://arxiv.org/abs/2002.05825)]

      距离度量在机器学习中无处不在——用于相似度、损失函数、学习目标等。三角不等式既是理论收敛与最优性的基础，也是很有用的归纳偏置。然而，大多数深度度量学习方法仅通过欧氏距离在潜在空间中满足三角不等式，但很多实际场景中的距离（如图中最短路径、RL 中的状态距离）是非对称或无法嵌入欧氏空间的，普通方法无法建模。本文因此提出新的神经网络架构，在结构上就保证满足三角不等式，以更好地刻画这些复杂距离。【图距离建模】【图数据集,RL环境】【各种距离函数】【作者自己提出的三个模型】

55. **Are Pre-trained Language Models Aware of Phrases? Simple but Strong Baselines for Grammar Induction** [ICLR2020] [[paper link](https://arxiv.org/abs/2002.00737)]

      不修改模型结构、不微调，只使用预训练语言模型的隐表示（hidden states）来进行语法归纳任务。【无监督语法归纳】【WSJ,multiNLI等】【F1】【Bert等】

56. **Inductive Matrix Completion Based on Graph Neural Networks** [ICLR2020] [[paper link](https://arxiv.org/pdf/1904.12058)]

      矩阵补全（Matrix completion）方法（如传统的矩阵分解或 GNN-based 推断）多为 transductive：它们依赖学习特定用户／物品的潜在嵌入，因此无法推广到训练中未见过的新用户、新物品，且常需使用侧信息（例如用户年龄或电影类型）以实现inductive性能。通过纯粹从评分矩阵构建的二部图中提取local enclosing subgraph（以特定(user, item)为中心的局部子图），并用GNN直接学习子图 → rating的映射，从而让模型具备对新用户／新物品或新评分矩阵的直接迁移能力。【矩阵补全】【Flixster,DOUBAN,MovieLens等等】【RMSE】【IGMC】

57. **Inductive representation learning on temporal graphs** [ICLR2020] [[paper link](https://arxiv.org/abs/2002.07962)]

      现实世界中大量图结构数据具有连续时间变化特性（例如社交网络、用户–商品交互、人–物项购买等），同时随着节点与边的不断新增、删除、特征变化，图结构也会随之演化。已有的大多数图嵌入方法仅能处理静态图或离散快照，缺乏处理连续时间演化与节点新增的能力。文章强调，在工业大规模动态图下，模型需要具备 Inductive inference（新节点/新时间点的嵌入推断能力）和 time-feature interactions 排列。故提出新的模型架构来解决：对时间编码与邻域聚合一体化设计，实现平滑连接到 GraphSage／GAT 思路，但扩展到 时序图，并且支持 Inductive 嵌入生成。【Future Link Prediction】【Reddit,维基等等】【AUC】【TGAT各种变体】

58. **Synthesizing Programmatic Policies that Inductively Generalize** [ICLR2020] [[paper link](https://openreview.net/pdf?id=S1l8oANFDH)]

      深度强化学习虽在多个控制任务上取得进展，但其策略通常“过拟合”训练环境，难以应对诸如样本大小变化、目标数量变化、地点变化等在测试时才遇到的情况，尤其是需要反复某种子行为才能达成的任务；作者将此类能力称为 “归纳泛化（inductive generalization）” —— 能够对任意次数的重复行为（例如多次绕行、拉杆上山等）自动扩展策略；他们发现，程序化的有限状态机(policy as state machine) 天然支持这种行为的循环与分支，从而具有更强的泛化能力；但此类策略很难通过传统梯度网络直接学习，因为其兼具离散控制结构与连续参数部分；故论文提出一种学习范式：基于program synthesis + teacher‑student imitation 的“自适应教学”方法，用有限规则描述policy结构，让策略学到可泛化的 “程序”，而不是绑定到特定范围数据的神经网络。【归纳泛化】【六个归纳泛化场景】【成功率】【一些RL模型】

59. **GraphSAINT: Graph Sampling Based Inductive Learning Method** [ICLR2020] [[paper link](https://arxiv.org/pdf/1907.04931)]

      当下的 GCN 结构在大图上训练时面临**“邻域指数增长”（neighbor explosion）**问题：随着网络层数增加，每个节点的多跳邻居数量迅速膨胀。现有的图像层采样（layer sampling）方法（如 GraphSAGE、FastGCN、S‑GCN、AS‑GCN 等）虽有一定减轻邻域扩展的效果，但仍面临准确率下降、训练开销大、架构兼容性差等问题。因此，论文提出：从“采样图”而非“采样层”入手，改为先抽取图子集，再构建完整的 GCN 并进行训练，从根本上解决扩展性与准确性之间的冲突。【节点分类】【六个节点分类数据集】【F1】【GraphSAINT】

60. **Inductive and Unsupervised Representation Learning on Graph Structured Objects** [ICLR2020] [[paper link](https://openreview.net/pdf?id=rkem91rtDB)]

      许多图结构任务（比如图分类、检索、异常检测）缺少标签或难以获取标签，因此迫切需要一种方法能够在没有监督信号（unsupervised）且能处理未见图（inductive） 的情况下生成图的向量表示。【图分类图聚类】【七个数据集】【ACC】【自己的模型】

61. **Learn to Explain Efficiently via Neural Logic Inductive Learning** [ICLR2020] [[paper link](https://arxiv.org/pdf/1910.02481)]

      在接受噪声和大规模 KB 的同时，用可学习且高效的方法生成更长、更丰富、且具有全局一致性的符号 FOL 规则作为解释。【KG补全】【ILP benchmark等】【MRR,Hit@10】【NLIL模型】
    
62. **Implementing Inductive bias for different navigation tasks through diverse RNN attractors** [ICLR2020] [[paper link](https://arxiv.org/pdf/2002.02496)]

      动物／人工智能在导航任务中需要某种内部表示（cognitive map），通常假设是欧几里得 metric 地图；但这种“地图”形式在不同导航任务中并非最优。PosNet 的 RNN 形成 “plane/continuous attractor”，便于位置积分与 metric 推理；MemNet 则形成 “discrete attractors”，易于编码地标记忆与 topological 推断。【grid路径任务】【15×15离散grid arena】【Trial-level score】【RNN LSTM各种net】

63. **Inductive Representation Learning in Temporal Networks via Causal Anonymous Walks** [ICLR2021] [[paper link](https://arxiv.org/pdf/2101.05974)]

      现实世界中的temporal networks（社交互动、通信日志等）遵循诸如三角闭合、前馈控制环路等动态演化规律，而这些规律通常独立于节点身份（node identity），是系统的结构性laws。要对新网络泛化，仅靠记忆节点编号是不够的。因此，论文的核心动机是设计一种能够捕捉网络动态规律（motifs）、同时对节点身份保持匿名、还能对新网络实现 归纳式泛化的representation learning方法。【Temporal link prediction】【Reddit, Wikipedia等】【AUC】【CAW系列】

64. **Neural Structured Prediction for Inductive Node Classification** [ICLR2022] [[paper link](https://arxiv.org/pdf/2204.07524)]

      结合 GNN 的高容量与效率，以及 CRF 的结构输出建模能力，来改进归纳节点分类任务。【inductive节点分类】【Cora等】【ACC】【GNN+CRF】

65. **Inductive Relation Prediction Using Analogy Subgraph Embeddings** [ICLR2022] [[paper link](https://openreview.net/pdf?id=PTRo58zPt3P)]

      传统基于嵌入的知识图谱链接预测方法依赖于固定实体与关系的训练集，因此无法处理测试时出现的全新关系类型（即只在推理时才出现的关系）。作者提出利用子图结构与类比模式，在归纳设置中支持新关系的预测，同时带来更好的泛化与可解释性。【归纳关系预测任务】【对应数据集】【MRR/Hits@K】【GraphANGEL模型】

66. **On Incorporating Inductive Biases into VAEs** [ICLR2022] [[paper link](https://arxiv.org/pdf/2106.13746)]

      在标准 VAE 中通过替换先验分布（prior）来引入 inductive bias（归纳偏好）往往效果不佳，论文提出了用 Intermediary Latent Space VAEs（InteL‑VAEs）进行改善。【图像生成】【VAE对应数据集】【ELBO】【VAE系列】

67. **Embedded-model flows: Combining the inductive biases of model-free deep learning and explicit probabilistic modeling** [ICLR2022] [[paper link](https://arxiv.org/pdf/2110.06021)]

      继承领域 inductive bias（如多模态、层级耦合、连续性）而保持流模型训练的灵活性。【结构化推断】【合成数据集】【对数似然, ELBO】【多EMF结构】

68. **Learning Language Representations with Logical Inductive Bias** [ICLR2023] [[paper link](https://arxiv.org/abs/2302.09458)]

      Transformer 在大型预训练语言模型中表现优越，这部分归因于其固有的 relational inductive bias（如 pairwise attention），但模型缺乏 逻辑推理层次的结构偏好。作者希望引入一种新的 “逻辑归纳偏好（logical inductive bias）”，使模型不仅能建模分布式语义表征，还能具备形式化的逻辑推理能力。将一阶逻辑 Horn 子句作为可学习的 神经逻辑操作符，并通过 forward chaining（前向连锁推理） 构建一个全可微的逻辑推理网络。【文本分类, NIL等】【GLUE等】【ACC, F1】【FOLNet模型】

69. **LogicDP: Creating Labels for Graph Data via Inductive Logic Programming** [ICLR2023] [[paper link](https://openreview.net/pdf?id=2b2s9vd7wYv)]

      现实中的图数据（如场景图和知识图）往往不完整，但图推理模型（如知识图补全、场景图补全）都需要大量训练数据才能取得好效果。人工标注成本高。现有的 Data Programming（DP）方法主要面向非结构化数据，不适用于图结构数据，也依赖专家手动编写 labeling functions（标注函数）。论文动机在于：能否自动生成图结构的标注函数，减少专家工作，并更高效地构建训练集？因此提出 LogicDP 框架。【图推理任务】【场景图数据集】【数据效率】【GNN等图推模型】

70. **Graph Signal Sampling for Inductive One‑Bit Matrix Completion: a Closed‑Form Solution** [ICLR2023] [[paper link](https://arxiv.org/pdf/2302.03933)]

      现代推荐系统中，经常在线上出现 新用户，他们在测试阶段可能只有正反馈（“喜欢”即1），而没有负反馈。传统的 one‑bit matrix completion 无法处理这种 inductive 设置（测试时出现新列只有正例）。作者动机是提出一个 可推广的新用户预测框架，能够在仅获取部分正反馈的情形下，准确推断一个新用户对所有物品的兴趣倾向。【Inductive Top‑N推荐】【Netflix】【HR@50等】【GS】

71. **Phenomenal Yet Puzzling: Testing Inductive Reasoning Capabilities of Language Models with Hypothesis Refinement** [ICLR2024] [[paper link](https://arxiv.org/pdf/2310.08559)]

      论文提出了一种模拟人类归纳推理过程的 三步迭代假设精炼方法：Hypothesis Proposing：LM 根据少量示例生成多个候选规则或假设；Selection：使用 task-specific 符号解释器（symbolic interpreter）检测每个假设能覆盖多少已知例子，挑选覆盖度高者；Refinement：LM 基于反馈进一步修改所选假设，迭代数轮直至收敛。最终得到一个符合多数示例并具有泛化潜在能力的规则，并用它预测 unseen instances。【inductive任务】【因果关系归纳（causal induction）,语言式组合指令归纳（如 MiniSCAN）,符号操作归纳（Rule）,视觉概念归纳（ARC mini versions）】【预测准确率】【GPT‑3.5, GPT‑4,Claude-2】

72. **Abstractors and relational cross-attention: An inductive bias for explicit relational reasoning in Transformers** [ICLR2024] [[paper link](https://arxiv.org/pdf/2304.00195)]

      传统 Transformer 建模物体之间的关系时，关系信息往往与对象的视觉或属性特征混合表示，导致模型无法显式地进行关系推理。作者认为，为支持从少量数据中进行归纳推理，需要一类结构性inductive bias，即把关系信息与对象特征解耦，使模型能够专注于关系信息进行抽象和泛化。 【判别性关系任务】【合成 relational reasoning benchmark】【ACC】【Transformer+Abstractor】

73. **Geometrically Aligned Transfer Encoder for Inductive Transfer in Regression Tasks** [ICLR2024] [[paper link](https://arxiv.org/pdf/2310.06369)]

      当前大多数迁移学习方法聚焦于图像或语言分类任务，而 回归任务（特别是分子性质预测）鲜有能有效迁移的方法；回归任务中，即使源任务相关但任务定义不同，目标数据样本稀缺也带来挑战；标准迁移学习方法在处理 latent 表示几何结构差异时往往无视几何对齐，难以实现知识跨任务流动；为此，作者提出了一种基于黎曼几何的迁移方法，针对回归任务设计 inductive transfer 框架。 【分子性质回归任务】【PubChem,Ochem,CCCB】【RMSE】【GATE模型】

74. **A 2‑Dimensional State Space Layer for Spatial Inductive Bias** [ICLR2024] [[paper link](https://openreview.net/pdf?id=BGkqypmGvm)]

      计算机视觉模型通常需要具备合适的 二维空间归纳偏好（2‑D inductive bias），如位置感知、空间局部性、平移与排列不变性。传统 CNN 本身具有强局部空间偏好；但 Transformer 通常作为一维序列处理图像并借助 positional encoding，其归纳偏好较弱。本文旨在设计可嵌入 Transformer 的新层，弥补其在视觉场景中的空间结构弱偏好。 【分类】【ImageNet‑1K等】【ACC】【ViT等】

75. **Conformal Inductive Graph Neural Networks** [ICLR2024] [[paper link](https://arxiv.org/pdf/2407.09173)]

      虽然 Conformal Prediction（CP） 为传统模型提供了无分布假设下的覆盖保证，适用于 transductive 节点分类，但其要求的 exchangeability（可交换性） 在 inductive（测试阶段出现新节点）场景中破坏，主要原因是 message passing 导致 calibration 分数分布 shift。因此，现有 CP 方法无法在 inductive setting（例如 新节点加入图结构后预测）保证覆盖率。作者动机在于构建一种适用于 inductive GNN 设置 的 CP 方法，既可满足 new node/edge 到来时的覆盖保证，又不损失统计效率。 【节点分类】【多个经典图分类数据集】【真实标签覆盖率】【NodeEx CP+GNN】

76. **Hypothesis Search: Inductive Reasoning with Language Models** [ICLR2024] [[paper link](https://arxiv.org/pdf/2309.05660)]

      Abstract Hypothesis Proposal：让 LLM 生成多个自然语言层面的抽象假设；Hypothesis Filtering / Summarization：通过 LLM 或 minimal 人工筛选，缩小假设集；Concrete Program Implementation：将每个假设转化为可执行的 Python 程序，并验证其是否能正确解释已知样本。 【ARC与列表变换】【对应数据集】【ACC】【GPT3.5和4】
    
77. **Label-Focused Inductive Bias over Latent Object Features in Visual Classification** [ICLR2024] [[paper link](https://openreview.net/pdf?id=cH3oufN8Pl)]

      输入域偏置问题：现有的视觉分类模型通常依赖于输入图像中的视觉相似性来学习特征，这种方法可能引入与人类标注者基于世界知识所定义的隐式输出域之间的冲突。这种冲突可能限制模型在推理阶段的泛化能力。目标：提出一种方法，通过构建仅由输出标签区分的特征，来减少输入域偏置对模型推理的影响，从而提高模型的泛化能力。【分类任务】【CIFAR-10等等】【ACC】【ViT】

78. **Integrating Planning and Deep Reinforcement Learning via Automatic Induction of Task Substructures** [ICLR2024] [[paper link](https://openreview.net/pdf?id=PR6RMsxuW7)]

      尽管深度学习在高维决策任务中取得了显著进展，但在稀疏奖励和目标导向任务中仍面临学习效率低和泛化能力差的问题。经典规划的优势与局限：经典规划方法擅长处理具有层次结构的任务，通过符号知识进行高层次规划，但大多数方法依赖于预定义的子任务假设，限制了其在未知环境中的应用。提出一种框架，将 DRL 与经典规划相结合，通过从少量示范中自动诱导任务结构和子结构，克服上述挑战。【稀疏奖励和目标导向的任务】【对应数据集】【对应性能】【多种深度学习方法】

79. **LVSM: A Large View Synthesis Model with Minimal 3D Inductive Bias** [ICLR2025] [[paper link](https://arxiv.org/pdf/2410.17242)]

      传统的视图合成方法（如 NeRF、3DGS）依赖于固定的 3D 表示和渲染方程，限制了模型的泛化能力和可扩展性。挑战：如何在不依赖传统 3D 偏置的情况下，实现高质量的视图合成。【Novel View Synthesis】【多个数据集】【信噪比】【LVSM模型】

80. **Decision Tree Induction Through LLMs via Semantically-Aware Evolution** [ICLR2025] [[paper link](https://arxiv.org/pdf/2503.14217)]

      决策树具有较强的可解释性和适用性，但传统生成方法（如 CART）容易陷入贪心子优化；优秀的全局搜索算法（如 exact methods）计算复杂度高且受限于小问题规模。遗传编程（GP）虽能寻找更全局最优解，却缺乏语义引导，搜索效率低、易陷入无意义变化。因此作者提出将大语言模型（LLM）中蕴含的语义先验知识纳入 GP 操作中，以提升决策树结构搜索的效率和泛化能力。【分类与回归任务】【对应数据集】【MSE】【LLEGO】

81. **Neuron‑based Personality Trait Induction in Large Language Models** [ICLR2025] [[paper link](https://arxiv.org/pdf/2410.12327)]

      目前 LLM 刚性表达 personality traits（如 Big Five），但主流方法依赖 prompt engineering（稳定性差）或 fine-tuning（资源消耗高）。作者希望探索一个更稳定、高效且可解释的方法：直接通过 操控 LLM 中的具体神经元 实现个性特质调整，而无需微调或重训练整个模型。【LLM人格】【PERSONALITYBENCH】【自动打分】【LLaMA】

82. **Fully‑inductive Node Classification on Arbitrary Graphs** [ICLR2025] [[paper link](https://arxiv.org/pdf/2405.20445)]

      传统的图机器学习模型只能在训练所见图上泛化，无法推广到拥有全新结构、节点特征与标签空间的图。现有 Inductive GNN 方法仍假设测试图与训练图共享特征/标签空间，限制其在不同域间迁移能力。作者提出更广泛、更实用的 “fully‑inductive” 设定：模型需在任意图（结构、feature、label 均不依赖训练图）上执行分类，无需重新训练或微调。【节点分类】【30个不同图domain数据集】【ACC】【GraphAny】

83. **Differentiable Rule Induction from Raw Sequence Inputs** [ICLR2025] [[paper link](https://openreview.net/pdf?id=zDjHOsSQxd)]

      传统可微分归纳逻辑编程（Differentiable ILP）方法通常依赖符号化输入，即从预训练网络或手工特征里获得离散符号标签，再学习规则。这会造成 标签泄漏（label leakage）：模型过度依赖输入中特征标签的监督，不能直接从原始连续输入（如时间序列或图像）中归纳规则。因此，作者希望构建一个 端到端可微分 pipeline，实现从 原始序列或图像输入 学习符号规则的能力，同时避免标签泄漏。【时间序列分类, 图像归纳】【UCR, MNIST】【准确率】【NeurRL】

84. **Selective Induction Heads: How Transformers Select Causal Structures in Context** [ICLR2025] [[paper link](https://openreview.net/pdf?id=bnJgzAQjWf)]

      Transformer 中的 induction heads 已被证明是 in‑context learning 的关键机制，它们能根据上下文复制先前出现的 tokens，实现基于因果依赖的 token 预测。以往研究使用的设置假定因果结构（如 Markov 链滞后）是固定的，无法解释自然语言和实际任务中动态变化的因果关系。构建了一种 交错的 Markov 链（Interleaved Markov Chains），在同一序列中混入多个不同滞后（lag）结构，但保持 transition probabilities 不变。训练 attention-only 的 Transformer 在每个 context 中识别当前有效的滞后结构，并且通过复制相应滞后的 token 进行预测。构建了一个简化的 三层 Transformer 架构，第 1 层估计不同滞后结构的 transition probabilities，第 2 层对这些概率进行 aggregated，最后第 3 层引入 Selective Induction Head 来选择正确滞后并复制对应 token。【交错 Markov Chain生成的synthetic序列上进行next‑token prediction】【合成数据集】【对应方法】【Attention‑only Transformer】

85. **Generative Event Schema Induction with Entity Disambiguation** [ACL2015] [[paper link](https://aclanthology.org/P15-1019.pdf)]

      引入实体属性关系（如修饰词）和触发关系（如动词与实体的语法关系），改进事件模式的归纳效果。方法是使用概率主题分布表示实体及其上下文信息，通过Gibbs采样进行参数估计，利用Dirichlet先验生成分布。
【无监督的事件模式归纳】【MUC-4语料库】【精确率、召回率、F-score】【提出的生成模型】

86. **Environment-Driven Lexicon Induction for High-Level Instructions** [ACL2015] [[paper link](https://aclanthology.org/P15-1096.pdf)]

      在机器人执行指令任务中，训练时学习的词汇表在测试时无法覆盖新动词，提出利用环境信息生成新的逻辑形式，动态扩展词汇表。联合建模文本、逻辑形式和环境，通过特征函数评分逻辑形式。
【将自然语言指令映射为机器人动作序列】【自建的众包数据集】【IED（编辑距离）、END（Jaccard指数）】【提出的混合模型（训练时词汇归纳+测试时环境驱动搜索）】

87. **Aconvex and feature-rich discriminative approach to  dependency grammar induction** [ACL2015] [[paper link](https://aclanthology.org/P15-1133.pdf)]

      无监督依存句法分析方法（从无标注语料中归纳出通用的依存语法规则）要基于生成模型（如DMV），涉及非凸优化问题，初始化敏感且易陷入局部最优。提出一种凸优化框架，支持丰富的特征表示和非投影依存结构生成。
【无监督依存句法分析】【Universal Treebanks v2.0】【有向依存准确率】【提出的凸判别式模型】

88. **Probing the Linguistic Strengths and Limitations  of Unsupervised Grammar Induction** [ACL2015] [[paper link](https://aclanthology.org/P15-1135.pdf)]

      无监督语法归纳生成的依存关系通常是无标记的。通过带标记的依存关系评估（CCGbank标注），分析无监督CCG解析器的能力边界，尤其关注非局部依赖等复杂结构的处理缺陷，为未来引入语义信号或弱监督提供依据。
【无监督组合范畴语法（CCG）归纳与解析】【CCGbank】【带标记依存F1（LF1）、无标记依存F1（UF1）、Supertagging准确率】【在HDP-CCG模型基础上改进】

89. **Bilingual Word Embeddings from Non-Parallel Document-Aligned Data  Applied to Bilingual Lexicon Induction** [ACL2015] [[paper link](https://aclanthology.org/P15-2118.pdf)]

      从仅文档对齐的数据中学习双语词嵌入，并将其应用于双语词典归纳（BLI）任务。提出了BWESG，将双语文档合并、随机打乱，确保每个词的上下文包含两种语言的词汇，使用Skip-Gram训练双语词嵌入。
【双语词典归纳（BLI）】【三种语言对的文档对齐维基百科数据】【测试集中源语言词的正确翻译在目标语言中排名第一的比例】【BWESG】

90. **Labeled Grammar Induction with Minimal Supervision** [ACL2015] [[paper link](https://aclanthology.org/P15-2143.pdf)]

      无监督语法归纳依赖黄金词性标注（gold POS tags）。提出通过少量人工监督，从词聚类中归纳出依存结构。为每个聚类标注3个高频词的词性，通过多数投票确定聚类标签，利用HDP-CCG模型生成依存句法结构。
【无监督的带标签语法归纳】【英语和汉语的CCGbank、PASCAL语法归纳挑战赛的10种语言依赖树库】【词聚类质量：Many-to-one (M-1)、V-Measure (VM)、名词/动词/其他召回率（NV/O Recall）；句法分析性能：定向带标签F1（LF1）、无向无标签F1（UF1）】【HDP-CCG】

91. **Liberal Event Extraction and Event Schema Induction** [ACL2016] [[paper link](https://aclanthology.org/P16-1025.pdf)]

      传统事件抽取方法依赖预定义事件模式，提出直接从语料中自动发现事件模式并抽取事件。先通过约束聚类将触发词和论元分别聚类为事件类型和角色，基于聚类中心触发词命名事件类型，并利用AMR/FrameNet映射论元角色名称。
【事件模式发现与事件抽取】【ERE语料、ACE2005、PubMed摘要及全文】【模式发现：覆盖度（与ACE/ERE人工模式的对比）、类型/角色数量；事件抽取：触发词/论元的识别（Precision/Recall/F1）与分类准确率】【聚类+AMR/FrameNet】

92. **Extracting token-level signals of syntactic processing from fMRI- with an  application to PoS induction** [ACL2016] [[paper link](https://aclanthology.org/P16-1071.pdf)]

      本文提出从fMRI数据中归纳词性信号的方法，基于高斯滑动窗口提取单词级fMRI特征，结合类型约束的二阶HMM进行弱监督词性归纳。
【弱监督词性标注】【8名受试者阅读《哈利·波特与魔法石》第9章的fMRI数据】【词性标注准确率（Accuracy）、F1值（按词性类别细分）】【融合fMRI向量的HMM】

93. **ALTO: Active Learning with Topic Overviews for Speeding Label Induction and Document Labeling** [ACL2016] [[paper link](https://aclanthology.org/P16-1110.pdf)]

      通过结合主题模型（全局归纳标签）和主动学习（局部优化标注），解决文本分类中标签归纳和高效标注的问题。提出ALTO框架利用主题模型提供全局视角，并借助主动学习指导用户标注关键文档。
【文本分类中的标签归纳和文档标注】【US Congressional Bills（美国国会法案）和20 Newsgroups】【Purity（纯度）、Rand Index（兰德指数）、Normalized Mutual Information（标准化互信息）】【逻辑回归分类器（用于主动学习）和LDA主题模型（用于生成主题概览）】

94. **Joint Word Segmentation and Phonetic Category Induction** [ACL2016] [[paper link](https://aclanthology.org/P16-2010.pdf)]

      通过理想化数据下的联合建模，验证无监督方法能否同时归纳词汇和语音类别，揭示了真实语音识别中上下文变异是主要挑战。方法是分层贝叶斯框架的联合模型，通过Dirichlet过程和高斯分布建模词汇与声学特征，利用Gibbs采样进行推断。
【联合词汇分割和元音类别归纳】【基于Brent (1999)的儿童导向语音语料库，添加模拟共振峰数据（来自Hillenbrand et al. 1995的实验室元音数据）】【分割性能：词边界检测的精确率（P）、召回率（R）、F1值；元音聚类：配对F1值（衡量同类元音是否被正确聚类）】【分层贝叶斯模型（Dirichlet过程 + 高斯混合），基于Gibbs采样的推断方法】

95. **Multiplicative Representations for Unsupervised Semantic Role Induction** [ACL2016] [[paper link](https://aclanthology.org/P16-2020.pdf)]

      通过显式建模句法关系提升嵌入的语义角色归纳能力，解决了无监督语义角色标注（SRL）中依赖关系与词汇语义解耦的问题。方法是基于神经网络的乘法依赖变换，通过上下文预测和层次聚类实现语义角色归纳。
【无监督语义角色归纳】【North American News Text Corpus（训练）、CoNLL 2008（评估）】【纯度（PU）、共现率（CO）、F1值；SimLex999的词相似性】【基于CBOW框架】

96. **Program Induction by Rationale Generation:  Learning to Solve and Explain Algebraic Word Problems** [ACL2017] [[paper link](https://aclanthology.org/P17-1015.pdf)]

      解决代数应用题需要生成一系列算术操作来得到最终答案，但直接从问题-答案对中归纳程序极具挑战性。提出通过生成答案解释（由自然语言和数学表达式组成的中间步骤）来间接监督程序学习。
【代数应用题的求解与解释生成】【自建的100,000条问题-解释对数据集】【困惑度（Perplexity）、BLEU-4（解释质量）、答案准确率（Accuracy）】【LSTM支持数学操作和指针网络】

97. **Watset: Automatic Induction of Synsets from a Graph of Synonyms** [ACL2017] [[paper link](https://aclanthology.org/P17-1145.pdf)]

      通过归纳方法从同义词词典中自动构建无歧义的词集，解决资源匮乏语言的词汇资源问题。提出Watset通过局部词义消歧和全局图聚类，从同义词图中归纳出词集。
【词集归纳】【英语：WordNet、BabelNet；俄语：RuWordNet、YARN】【精确率（Precision）、召回率（Recall）、F-score（Paired F-score）】【Watset（基于局部-全局聚类）】

98. **Adversarial Training for Unsupervised Bilingual Lexicon Induction** [ACL2017] [[paper link](https://aclanthology.org/P17-1179.pdf)]

      通过对抗训练从单语词嵌入中无监督地归纳出跨语言映射关系，解决双语词典构建中的监督依赖问题。通过生成器与判别器的对抗训练学习跨语言线性映射，结合正交约束和重构损失提升性能。
【无监督双语词典归纳】【Wikipedia可比语料及Gigaword大规模语料】【Top-1和Top-5准确率】【提出的三种对抗训练模型（单向、双向、对抗自编码器）】

99. **Zara Returns: Improved Personality Induction and Adaptation by an  Empathetic Virtual Agent** [ACL2017] [[paper link](https://aclanthology.org/P17-4021.pdf)]

      通过多模态人格识别和动态个性适配，提升虚拟代理的共情能力，其方法从用户数据中归纳出人格特征与交互偏好之间的关系。
【人格识别与虚拟代理的个性化适配】【音频：ChaLearn First Impressions数据集、文本：WCPR的Facebook和YouTube数据集】【F-score、准确率、精确率、召回率】【CNN】

100. **A La Carte Embedding:  Cheap but Effective Induction of Semantic Feature Vectors**  [ACL2018] [[paper link](https://aclanthology.org/P18-1002.pdf)]

      现有词嵌入方法在小规模语料或稀疏特征（如罕见词、n-gram、同义词集）场景下性能下降，提出"a la carte embedding"，基于预训练词向量和线性回归学习上下文到嵌入的映射矩阵，支持动态生成新特征的嵌入。
【罕见词嵌入学习；同义词集嵌入与词义消歧；n-gram嵌入与文档分类】【自建的Contextual Rare Words (CRW) 数据集；非词任务（nonce）和合成词（chimera）数据集；SemCor（用于WSD）和多个文档分类数据集】【罕见词：Spearman相关系数（与人类评分的一致性）；非词/合成词：平均倒数排名（MRR）和Spearman相关系数；WSD：准确率；文档分类：准确率】【a la carte embedding】

101. **On the Limitations of Unsupervised Bilingual Dictionary Induction**  [ACL2018] [[paper link](https://aclanthology.org/P18-1072.pdf)]

      文章通过实验归纳发现无监督双语词典归纳的缺陷（如语言形态和领域的影响），提出用同形词弱监督和图相似性度量来改进。结合对抗训练和弱监督对齐词嵌入，并用拉普拉斯特征值量化跨语言词嵌入的相似性。
【双语词典归纳】【Polyglot Wikipedia、EuroParl、EMEA医学语料库、Finnish WaC】【Precision@1】【基于fastText的词嵌入，结合对抗训练】

102. **Embedding Learning Through Multilingual Concept Induction**  [ACL2018] [[paper link](https://aclanthology.org/P18-1141.pdf)]

      研究通过多语言概念归纳学习跨语言的词向量表示，以解决低资源语言中缺乏平行语料的问题，并提升跨语言任务的性能。方法是基于词典图提取概念，利用这些概念训练跨语言词嵌入。
【跨语言词相似度、情感分析、往返翻译】【Parallel Bible Corpus】【往返翻译的准确率、情感分析的F1分数】【基于word2vec的skip-gram模型】

103. **Higher-order Relation Schema Induction using Tensor Factorization with  Back-off and Aggregation** [ACL2018] [[paper link](https://aclanthology.org/P18-1146.pdf)]

      从无标注文本中归纳高阶关系模式，解决了知识图谱构建中多元关系缺失的问题。提出TFBA，通过分解低阶张量并聚合二元模式，构建高阶关系模式。
【高阶关系模式归纳（HRSI）】【Shootings（美国枪击事件文档）、NYT Sports（纽约时报体育新闻）、MUC（拉丁美洲恐怖事件新闻）】【人工评估（三位评审员验证模式的准确性），使用AvgFIT（平均拟合分数）选择超参数】【TFBA】

104. **End-to-End Reinforcement Learning for Automatic Taxonomy Induction** [ACL2018] [[paper link](https://aclanthology.org/P18-1229.pdf)]

      提出一种端到端强化学习方法（TaxoRL），通过联合学习术语关系表示和分类法构建，解决传统两阶段方法在自动归纳层次分类法时的错误传播和局部优化问题。用强化学习策略网络逐步构建分类法，通过全局奖励（如祖先F1）优化整体结构。
【自动分类法归纳】【WordNet、SemEval-2016 Task 13的TExEval-2数据集】【祖先F1、边F1】【TaxoRL】

105. **Unsupervised Semantic Frame Induction using Triclustering**  [ACL2018] [[paper link](https://aclanthology.org/P18-2010.pdf)]

      提出无监督方法Triframes，通过三聚类从大规模三元组数据中自动归纳语义框架。将SVO三元组嵌入后聚类，利用图算法（如Watset）同时发现框架、动词及其角色。
【无监督语义框架归纳】【FrameNet 1.7、DepCC、多义动词聚类数据集】【归一化修正纯度、归一化逆纯度、综合F1值】【Triframes】

106. **Orthographic Features for Bilingual Lexicon Induction** [ACL2018] [[paper link](https://aclanthology.org/P18-2062.pdf)]

      通过融合拼写特征与词嵌入，提升低资源相关语言对的双语词典归纳性能。方法是，扩展词嵌入的拼写信息，或直接调整相似性得分以结合编辑距离与嵌入相似性。
【无监督双语词典归纳】【英语-意大利语、英语-德语、英语-芬兰语】【翻译准确率】【提出的方法】

107. **Connecting Distant Entities with Induction through Conditional  Random Fields for Named Entity Recognition: Precursor-Induced  CRF**  [ACL2018] [[paper link](https://aclanthology.org/W18-2402.pdf)] 

      CRF在命名实体识别中，当实体被多个非实体词分隔时，局部转移信息会丢失，无法捕捉远距离依赖关系。提出了前导诱导CRF，将非实体标签作为传递媒介，利用归纳方法将远距离依赖关系编码到一阶CRF中。
【命名实体识别】【i2b2 2012临床文本、SNUH风湿病患者出院摘要、JNLPBA 2004生物医学文献】【精确率（P）、召回率（R）、F1值（F）】【Precursor-induced CRF】

108. **Symbolic inductive bias for visually grounded learning of spoken language** [ACL2019] [[paper link](https://aclanthology.org/P19-1647.pdf)] 

      通过多任务学习结合转录语音数据，可以在端到端的视觉-语音学习框架中引入符号化的归纳偏置（symbolic inductive bias），从而提升模型性能。
【语音/图像匹配、语音/文本匹配、文本/图像匹配】【Flickr8K Audio Caption Corpus：每张图像配5条语音描述、LibriSpeech用于Speech/Text任务】【Recall@10、Median Rank、说话人识别准确率、表征相似性分析（RSA）、音素解码准确率】【GRU、VGG-16】

109. **Bilingual Lexicon Induction with Semi-supervision  in Non-Isometric Embedding Spaces**  [ACL2019] [[paper link](https://aclanthology.org/P19-1018.pdf)] 

      文章提出了一种半监督方法BLISS，用于从少量对齐词典和大量未对齐词嵌入中学习两种语言的词嵌入映射，解决了传统双语词典归纳方法对等距假设的依赖问题。
【双语词典归纳】【MUSE数据集和VecMap数据集】【词对齐的准确率】【BLISS】

110. **Compound Probabilistic Context-Free Grammars  for Grammar Induction**  [ACL2019] [[paper link](https://aclanthology.org/P19-1228.pdf)] 

      提出了一种增强版的概率上下文无关文法（PCFG），通过神经网络和隐变量提升模型的表达能力，从而更有效地从无标注文本中归纳语法结构。
【无监督语法归纳】【英文Penn Treebank（PTB）和中文Penn Treebank（CTB）】【无标记F1分数】【PCFG】

111. **Variance of average surprisal: a better predictor for quality of grammar from unsupervised PCFG induction**  [ACL2019] [[paper link](https://aclanthology.org/P19-1235.pdf)]
     
      提出了指标VAS，用于评估和选择无监督语法归纳模型。通过计算句子平均惊讶度的方差（VAS），捕捉语法模型对功能词和内容词的区分能力，替代传统的数据似然作为模型选择标准。
【无监督语法归纳】【多语言数据集（包括Penn Treebank、Universal Dependencies等）】【VAS、数据似然（LL）、右分支得分（RBS）、规则复杂度等】【基于贝叶斯PCFG的语法归纳模型】

112. **Domain Adaptation of Neural Machine Translation by Lexicon Induction**  [ACL2019] [[paper link](https://aclanthology.org/P19-1286.pdf)]  

      为解决神经机器翻译（NMT）跨领域时词汇缺失问题，提出无监督方法DALI，从单语数据中归纳领域词汇表并生成伪数据来微调模型。方法是用词嵌入映射和最近邻搜索提取领域词汇，构造伪平行语料训练NMT模型。
【德语到英语的领域适应机器翻译】【Medical、IT、Law、Subtitles、Koran五个领域的数据集】【BLEU分数】【基于LSTM和Transformer的NMT模型】

113. **MAAM:A Morphology-Aware Alignment Model for Unsupervised  Bilingual Lexicon Induction**  [ACL2019] [[paper link](https://aclanthology.org/P19-1308.pdf)] 

      为解决无监督双语词典归纳中形态学差异导致的错误对齐，提出了一种结合语法规则的方法。方法是用线性变换做词对齐，并通过去噪自编码器和语言模型引入语法信息来优化对齐结果。
【无监督双语词典归纳】【基于Wikipedia训练的300维fastText词向量】【最近邻检索的准确率】【线性变换（SGD优化）+ 去噪评估器】

114. **A Multilingual BPE Embedding Space  for Universal Sentiment Lexicon Induction**  [ACL2019] [[paper link](https://aclanthology.org/P19-1341.pdf)] 

      为了解决低资源语言缺乏情感词典的问题，提出了一种通用方法，通过BPE分词和多语言嵌入空间，从英语归纳出1593种语言的情感词典。方法是用BPE分词构建多语言嵌入空间，通过零样本迁移和领域适应生成情感词典。
【跨语言情感词典归纳】【Parallel Bible Corpus+、Twitter数据集】【F1分数、Kendall’s 、分类准确率】【word2vec-skipgram】

115. **Hubless Nearest Neighbor Search for Bilingual Lexicon Induction**  [ACL2019] [[paper link](https://aclanthology.org/P19-1399.pdf)] 

      为了解决BLI任务中hubness（某些目标词被过度检索为“中心点”）导致的检索偏差，文章提出HNN方法，通过均衡偏好假设优化词对齐。方法是用均衡偏好约束构建优化问题，并通过高效对偶求解器减少目标词的过度检索。
【双语词典归纳】【MUSE库中的6种语言的词嵌入和词典】【Top-1准确率、k-occurrence】【HNN】

116. **Duality of Link Prediction and Entailment Graph Induction**  [ACL2019] [[paper link](https://aclanthology.org/P19-1468.pdf)] 

      通过结合链接预测和蕴含图归纳，利用已知事实归纳出更全面的关系和规则，从而提升两个任务的性能。方法是使用链接预测模型预测缺失关系，构建马尔可夫链计算蕴含分数，再用这些分数优化链接预测结果。
【链接预测和蕴含关系检测】【NewsSpike文本语料库（用于链接预测），Levy/Holt数据集（用于蕴含关系评估）】【蕴含任务：AUC；链接预测任务：Hits@1、Hits@10、MR、MRR】【ConvE（链接预测模型）】

117. **Bilingual Lexicon Induction through Unsupervised Machine Translation**  [ACL2019] [[paper link](https://aclanthology.org/P19-1494.pdf)] 

      双语词典归纳（BLI）依赖于跨语言词嵌入的直接检索，但这些存在“中心性”问题。提出通过无监督机器翻译从单语数据中归纳出双语词典，避免了直接检索。
【双语词典归纳】【MUSE数据集】【Precision at 1】【词嵌入模型：fastText、基于短语的统计机器翻译】

118. **Unsupervised Induction of Ukrainian Morphological Paradigms for the  NewLexicon: Extending Coverage for Named Entities and Neologisms  Using Inflection Tables and Unannotated Corpora**  [ACL2019] [[paper link](https://aclanthology.org/W19-3701.pdf)] 

      通过无监督方法从语料中归纳出新词的形态变化规则，动态扩展词典，解决了静态资源覆盖不足的问题。方法是利用屈折表拆分词干和后缀，通过语料验证生成完整词形变化范式。
【无监督生成乌克兰语新词的形态学范式】【乌克兰语未标注语料及静态词典】【词汇覆盖率】【基于规则的范式生成算法，依赖屈折表和语料验证】

119. **Every Document Owns Its Structure: Inductive Text Classification via  Graph Neural Networks** [ACL2020] [[paper link](https://aclanthology.org/2020.acl-main.31.pdf)] 

      提出文本分类方法TextING，为每个文档构建局部图，节点为词，通过门控机制聚合邻居信息。实现归纳式文本分类，模型可泛化到未见过的新词和新文档。同时可以通过局部图建模词与词的细粒度关系。
【文本分类（情感分析、新闻分类、医学摘要分类）】【MR（电影评论情感分析）、MR（电影评论情感分析）、Ohsumed（医学摘要分类，23类）】【准确率】【TextING】

120. **Dynamic Memory Induction Networks for Few-Shot Text Classification** [ACL2020] [[paper link](https://aclanthology.org/2020.acl-main.102.pdf)] 

      通过动态记忆和查询增强，让模型从少量样本中归纳出鲁棒的类别表示，显著提升小样本分类性能。具体方法是结合动态路由调整记忆权重，利用查询信息筛选支持集样本，生成判别性类别向量。
【小样本文本分类】【miniRCV1（新闻分类）和ODIC（开放域意图分类）】【分类准确率】【BERT-base、动态记忆模块（DMM）、查询增强归纳模块（QIM）】

121. **A Graph-based Coarse-to-fine Method for Unsupervised  Bilingual Lexicon Induction** [ACL2020] [[paper link](https://aclanthology.org/2020.acl-main.318.pdf)] 

      提出了一种基于图的粗到细方法，通过从单词中归纳出词团级别的语义信息，生成更准确的初始词典，从而提升无监督双语词典归纳的性能。
【无监督双语词典归纳】【MUSE数据集】【Precision@1】【提出方法】

122. **Classification-Based Self-Learning for Weakly Supervised Bilingual Lexicon Induction** [ACL2020] [[paper link](https://aclanthology.org/2020.acl-main.618.pdf)] 

      提出ClassyMap，通过分类器从少量种子词对中归纳翻译规律，结合多特征优化，提升双语词典归纳的准确性。方法是分类器整合词形、语义等特征筛选高质量翻译对，迭代优化跨语言词向量并重排序候选词。
【弱监督双语词典归纳】【MUSE数据集】【Precision@1】【ClassyMap】

123. **The Importance of Category Labels in Grammar Induction with  Child-directed Utterances** [ACL2020] [[paper link](https://aclanthology.org/2020.iwpt-1.15.pdf)] 

      无监督语法归纳通常忽略短语标签的评估，仅依赖无标签评估导致模型仅学习到表面的分支倾向，无法捕捉人类语法的稀疏性和类别分布特性。提出带标签评估RH，从儿童语料中归纳更真实的语法结构。方法是用贝叶斯PCFG模型和RH指标，结合深度限制，从无监督数据中学习符合语言学特性的语法。
【无监督语法归纳】【CHILDES多语言语料、WSJ20Dev】【无标签F1、带标签RH和RVM】【贝叶斯PCFG模型】

124. **Script Induction as Association Rule Mining** [ACL2020] [[paper link](https://aclanthology.org/2020.nuse-1.7.pdf)] 

      将脚本归纳问题转化为关联规则挖掘，从叙事链中归纳高阶事件模式，提升缺失事件预测的准确性和可解释性。方法是用FP-growth挖掘频繁事件集，结合加权集合覆盖和后验概率优化预测缺失事件。
【脚本归纳】【Annotated Gigaword的纽约时报部分】【Recall@50和MRR】【FP-growth】

125. **Improving Bilingual Lexicon Induction with Unsupervised  Post-Processing of Monolingual Word Vector Spaces** [ACL2020] [[paper link](https://aclanthology.org/2020.repl4nlp-1.7.pdf)]
     
      跨语言词嵌入主要关注改进投影机制，而忽略了输入单语词向量空间的质量对跨语言对齐的影响。提出对单语词向量空间进行简单的后处理，可以显著提升双语词典归纳的性能。
【双语词典归纳】【PanLex数据集】【MRR】【基于投影的跨语言词嵌入方法（如VecMap和RCSLS）】

126. **Inductively Representing Out-of-Knowledge-Graph Entities by  Optimal Estimation Under Translational Assumptions** [ACL2021] [[paper link](https://aclanthology.org/2021.repl4nlp-1.10.pdf)] 

      文章解决知识图谱中未见过实体(OOKG）的表示问题，提出一种高效且无需额外训练的归纳方法，利用翻译模型的假设直接估计OOKG实体的嵌入。
【链接预测、三元组分类】【FB15k、WN11】【链接预测：MRR、Hits@1/10；三元组分类：准确率】【本文方法InvTransE、InvRotatE】

127. **Bilingual Lexicon Induction  via Unsupervised Bitext Construction and Word Alignment** [ACL2021] [[paper link](https://aclanthology.org/2021.acl-long.67.pdf)]

      提出结合无监督平行语料挖掘和词对齐，通过归纳数据中的统计规律生成高质量双语词典。方法是使用CRISS挖掘平行语料，SimAlign对齐词，再通过统计特征或MLP过滤噪声，生成最终词典。
【双语词典归纳】【BUCC 2020共享任务数据集、MUSE数据集、WikiMatrix平行语料】【F1分数、Precision@1】【CRISS、SimAlign、MLP】

128. **Neural Bi-Lexicalized PCFG Induction** [ACL2021] [[paper link](https://aclanthology.org/2021.acl-long.209.pdf)]

      提出神经双词汇化PCFG模型，通过潜在变量和分解技术从数据中归纳出句法规则，提升无监督句法分析性能。方法是使用规范多线性分解和“展开-折叠”技术优化词汇化PCFG的参数化和计算效率。
【无监督句法分析】【华尔街日报（WSJ）语料库（Penn Treebank）】【句子级F1分数、无标记定向附着分数（UDAS）、无标记无向附着分数（UUAS）】【神经双词汇化PCFG】

129. **Knowledge-Enriched Event Causality Identification via Latent Structure  Induction Networks** [ACL2021] [[paper link](https://aclanthology.org/2021.acl-long.376v2.pdf)]

      提出了归纳学习潜在推理结构方法（LSIN），通过结合外部知识，解决事件因果关系识别任务中数据稀缺和隐式因果线索的问题。LSIN利用图神经网络和潜在结构归纳模块，从外部知识中学习并优化推理路径。
【事件因果关系识别】【EventStoryLine和Causal-TimeBank】【精确率、召回率和F1分数】【LSIN】

130. **StructFormer: Joint Unsupervised Induction of Dependency and  Constituency Structure from Masked Language Modeling** [ACL2021] [[paper link](https://aclanthology.org/2021.acl-long.559.pdf)] 

      提出StructFormer，通过无监督学习从文本中同时归纳依存和成分结构，并利用这些结构提升语言模型的性能。
方法是通过句法距离和高度预测模块，结合依存约束的自注意力机制，实现了语言结构的联合归纳和语言建模。
【无监督依存解析、无监督成分解析、掩码语言建模】【Penn TreeBank (PTB)、BLLIP】【成分解析：未标记F1分数（UF1）；依存解析：未标记附着分数（UAS）和无向未标记附着分数（UUAS）；MLM：困惑度】【StructFormer】

131. **Semantic Frame Induction using  Masked Word Embeddings and Two-Step Clustering** [ACL2021] [[paper link](https://aclanthology.org/2021.acl-short.102.pdf)]

      提出一种无监督方法，通过掩码词嵌入和两步聚类从文本中归纳语义框架，解决现有方法过度依赖动词表面信息和聚类过度分割的问题。方法总结：结合BERT掩码嵌入减少表面信息干扰，通过两步聚类（先动词内聚类，再跨动词合并）实现更准确的语义框架归纳。
【无监督语义框架归纳】【英文FrameNet（Berkeley FrameNet 1.7）】【B-cubed Precision/Recall/F1（BCP/BCR/BCF）、Purity/Inverse Purity/F1】【BERT、聚类】

132. **Combining Static Word Embeddings and Contextual Representations for  Bilingual Lexicon Induction** [ACL2021] [[paper link](https://aclanthology.org/2021.findings-acl.260.pdf)]

      提出结合静态词嵌入和上下文表示的机制，通过弹簧网络和相似性插值，从单语数据中归纳更准确的双语词典。
通过弹簧网络调整静态词嵌入位置，结合上下文的语义信息，最终加权插值两种相似性以提升翻译匹配精度。
【双语词典归纳】【Wikipedia多语言语料、WaCKy语料】【Precision@1】【静态词嵌入：fastText、上下文表示：XLM/mBART】

133. **Verb Sense Clustering using Contextualized Word Representations  for Semantic Frame Induction** [ACL2021] [[paper link](https://aclanthology.org/2021.findings-acl.381.pdf)]

      研究如何用BERT等模型自动归纳动词的语义框架，减少人工标注工作。方法是用上下文词表示对动词聚类，区分不同语义框架，并用调整的BIC估计框架数量。
【语义框架归纳】【FrameNet和PropBank】【聚类匹配率、Spearman相关系数、准确率、均方根误差】【Transformer】

134. **Simple induction of (deterministic) probabilistic finite-state automata for  phonotactics by stochastic gradient descent** [ACL2021] [[paper link](https://aclanthology.org/2021.sigmorphon-1.19.pdf)]

      提出用梯度下降从数据中归纳PFA（概率有限状态自动机），自动学习音系规则。方法是通过优化可微分的PFA参数，支持无限制和受限子正则语言类的归纳。
【音系规则建模与PFA归纳】【Quechua和Navajo的词典词形数据】【保留数据的负对数似然（NLL）、合法与非合法非词的似然差异】【PFA】

135. **Probing as Quantifying Inductive Bias** [ACL2022] [[paper link](https://aclanthology.org/2022.acl-long.129.pdf)]  

      提出通过量化预训练表示对特定任务的归纳偏置（inductive bias）来改进探测方法。将表示和探测模型视为一个整体，用贝叶斯证据量化表示-探测模型对在特定任务中的归纳偏置，通过最大化证据，自动选择探测模型架构。
【词级别任务、依存弧标注任务、句子级别任务】【词级别和依存弧任务：Universal Dependencies (UD) v2.5树库、UniMorph模式；句子级别任务：MultiNLI、BoolQ、Commitment Bank、RTE】【对数证据，用于衡量表示-探测模型对的归纳偏置】【表示模型：m-BERT、fastText、随机表示（Rand.）、ALBERT、RoBERTa、XLNet、T5；探测模型：线性模型、MLP】

136. **Speaker Information Can Guide Models to Better Inductive Biases:  ACase Study On Predicting Code-Switching** [ACL2022] [[paper link](https://aclanthology.org/2022.acl-long.267.pdf)] 

      NLP模型在处理用户生成数据时可能不可靠，提出为模型提供说话者信息，可以引导模型学习更有用的归纳偏置（inductive biases）。在预测英语-西班牙语双语对话中的code-switching任务中进行了验证。
【预测英语-西班牙语双语对话中的语码转换点】【Bangor Miami数据集，包含56个英语-西班牙语对话，附带说话者的社会语言学特征】【准确率、F1分数、精确率、召回率】【在XLM-RoBERTa基础上预置说话者提示】

137. **Deep Inductive Logic Reasoning for Multi-Hop Reading Comprehension**  [ACL2022] [[paper link](https://aclanthology.org/2022.acl-long.343.pdf)] 

      针对多跳阅读理解任务，提出深度归纳逻辑推理模型DILR，通过逻辑规则生成和评估，实现可解释且高效的多跳推理。先从文档中筛选与查询相关的信息，递归生成逻辑子句，再通过逻辑运算符评估子句的真值概率。
【多跳阅读理解】【WikiHop、MedHop】【准确率】【DILR】

138. **Fire Burns, Sword Cuts: Commonsense Inductive Bias for  Exploration in Text-based Games**  [ACL2022] [[paper link](https://aclanthology.org/2022.acl-short.56.pdf)] 

      强化学习代理在探索大规模动作空间时效率低下，引入常识知识作为归纳偏置（Inductive Bias），帮助代理在训练中更好地泛化。使用预训练的语言模型（如COMET）基于当前观察生成常识知识图。
【文本游戏中的强化学习探索】【来自Jericho游戏套件的9个游戏】【游戏分数、生成动作的语言流畅性】【基于知识图的强化学习代理KG-A2C + CoMMEXPL(提出的结合常识的探索方法)】

139. **Hierarchical Inductive Transfer for Continual Dialogue Learning**  [ACL2022] [[paper link](https://aclanthology.org/2022.findings-acl.57.pdf)] 

      对话系统需要持续学习新的对话技能，提出分层归纳迁移框架AdaHIT。分层：基础适配器：从多任务中归纳通用对话模式（如语法、流畅性）；任务适配器：在通用知识基础上，通过微调归纳任务特定模式（如共情表达）。
【持续对话学习】【ConvAI2（个性化）、WoW（知识）、ED（共情）、BST（混合技能）】【Hits@1/K】【Reddit数据预训练的Poly-encoder，进行微调】

140. **Skill Induction and Planning with Latent Language** [ACL2022] [[paper link](https://aclanthology.org/2022.acl-long.120.pdf)]

      提出一种用少量语言标注从演示数据中自动归纳分层策略的方法，通过语言描述实现可解释的任务规划。方法是结合分段、标注和参数更新的迭代优化，利用预训练语言模型从稀疏标注中学习技能库和分层策略。
【分层策略学习与任务规划】【ALFRED（家庭机器人模拟环境）】【子任务完成率、端到端任务成功率】【基于T5-small的控制器和执行器】

141. **Discrete Opinion Tree Induction for Aspect-based Sentiment Analysis** [ACL2022] [[paper link](https://aclanthology.org/2022.acl-long.145.pdf)]

      提出一种无需依赖外部解析器的方法dotGCN，通过归纳学习自动生成针对特定方面的意见树结构，用于方面级情感分析，解决了依赖树模型的局限性。基于注意力分数和强化学习诱导树结构，结合GCN进行分类
【方面级情感分析】【六个英文基准数据集（如MAMS、SemEval）、一个中文酒店评论数据集和一个韩文汽车评论数据集】【 准确率和宏平均F1分数】【提出的dotGCN模型】

142. **Hierarchical Sketch Induction for Paraphrase Generation** [ACL2022] [[paper link](https://aclanthology.org/2022.acl-long.178.pdf)]

      提出一种通过归纳学习分层句法草图的方法（HRQ-VAE），用于生成高质量且多样化的复述，解决了传统方法需要完全指定句法结构的局限性。方法: 使用分层离散潜在变量逐步细化句法结构，结合编码-解码框架生成复述。
【复述生成】【Paralex（问题复述数据集）、Quora Question Pairs（QQP）、MSCOCO 2017（图像描述数据集）】【 iBLEU（平衡复述质量和多样性）、BLEU（复述质量）、Self-BLEU（复述与输入的差异）、P-BLEU（生成复述之间的多样性）】【HRQ-VAE】

143. **Large Scale Substitution-based Word Sense Induction** [ACL2022] [[paper link](https://aclanthology.org/2022.acl-long.325.pdf)]

      提出一种从大规模语料中自动归纳词义的方法，解决了传统词义消歧依赖人工清单的问题，并生成可解释的词义标注和嵌入。方法：用MLM生成替代词，通过图聚类动态归纳词义，再标注语料并训练静态嵌入。
【词义归纳（WSI）、词义标注、词义感知静态嵌入生成】【English Wikipedia、PubMed Abstracts、SemEval 2010/2013、自建大规模人工标注数据集】【F-Score、V-Measure、FNMI、FBC、分类F1、OPP】【BERT-large、SciBERT、word2vec（生成静态嵌入）】

144. **Query Structure Modeling for Inductive Logical Reasoning  Over Knowledge Graphs**  [ACL2023] [[paper link](https://aclanthology.org/2023.acl-long.259.pdf)]  

      提出“结构建模的文本编码框架”（SILR），解决知识图谱上复杂逻辑查询的归纳推理问题。将逻辑查询结构转换为文本序列，设计逐步指令，指示PLMs在查询结构中执行几何操作的顺序。通过显式建模查询的逻辑结构，使其能够泛化到训练时未见过的新实体、关系甚至新的知识图谱。
【复杂逻辑查询的归纳推理】【FB15k-237-V2、NELL-V3】【Hits@K（K=3,10）】【BERT-large-cased】

145. **Contrastive Learning with Generated Representations for Inductive  Knowledge Graph Embedding**  [ACL2023] [[paper link](https://aclanthology.org/2023.findings-acl.900.pdf)] 

      提出一种归纳式方法，能够从已有的知识图谱中捕获结构模式，并将其迁移到新的知识图谱中。设计了两种对比学习目标，分别在实体内部和元知识图谱之间进行对比，以显式模拟迁移模式。
【知识图谱的归纳式表示学习和链接预测】【F1-F4、N1-N4】【MRR、Hits@1、Hits@10】【VMCL及其变体（基于TransE和RotatE的KGE模型）】

146. **Learning Query Adaptive Anchor Representation for Inductive Relation Prediction** [ACL2023] [[paper link](https://aclanthology.org/2023.findings-acl.882.pdf)] 

      知识图谱中现有的归纳式关系预测方法（如GraIL）需要为每个候选三元组提取一个封闭子图并进行多次推理，效率低下。提出QAAR模型为查询实体提取一个开放子图，覆盖所有候选实体，避免重复提取。同时引入实体无关的锚点和多类特征，提升模型对未见实体的泛化能力。
【归纳式关系预测】【WN18RR、FB15k-237、NELL-995】【Hits@10】【QAAR】

147. **I2D2: Inductive Knowledge Distillation with  NeuroLogic and Self-Imitation**  [ACL2023] [[paper link](https://aclanthology.org/2023.acl-long.535.pdf)] 

      提出蒸馏算法，通过约束解码和自模仿学习显著提升GPT-2的常识生成质量。自模仿学习使模型从自身生成的样本中学习，逐步归纳（inductive）出更高质量的常识知识。
【生成日常概念的常识性陈述】【种子概念来自GenericsKB、ConceptNet、ProScript和ATOMIC，扩展概念使用GPT-3生成】【准确率、PR曲线】【GPT-2】

148. **Non-Sequential Graph Script Induction via Multimedia Grounding** [ACL2023] [[paper link](https://aclanthology.org/2023.acl-long.303.pdf)]

      通过视频数据自动归纳出更灵活的任务步骤图脚本（像流程图一样），而不仅仅是固定的线性步骤。方法是用视频和文本对齐训练模型，生成包含可选和可互换步骤的图脚本。
【非顺序图脚本归纳】【CrossTask、Howto100M、wikiHow】【Next Step Prediction（Acc@1, Acc@3, Rec@3, F1@3）、Partial Sequence Completion（Acc@1, Edit Distance）、人工评估（正确性和表达性）】【BART-base，结合对比学习】

149. **Open-Domain Hierarchical Event Schema Induction by Incremental  Prompting and Verification** [ACL2023] [[paper link](https://aclanthology.org/2023.acl-long.312.pdf)]

      利用大语言模型的常识，自动归纳出更灵活、层次化的事件流程图（比如“疫情爆发”包含“病例激增”“医院超负荷”等子事件）。方法：通过分阶段提问LLM（先列主干事件，再扩展细节，最后验证关系）构建事件模式图。
【开放领域层次化事件模式归纳】【ODIN（自建新闻场景库）、RESIN-11（11类新闻场景）、ProScript（日常任务）】【事件匹配F1、时序关系F1、层次关系F1；人工评估】【基于GPT-3的增量提示框架】

150. **Using Domain Knowledge to Guide Dialog  Structure Induction via Neural Probabilistic Soft Logic** [ACL2023] [[paper link](https://aclanthology.org/2023.acl-long.422.pdf)]

      文章提出了一种结合符号知识和神经网络的对话结构归纳方法，通过注入领域规则提升模型在数据稀缺时的表现。方法是用概率软逻辑规则指导神经网络的训练，联合优化符号约束和生成模型。
【对话结构归纳】【MultiWoZ 2.1 synthetic、SGD-synthetic、SGD-real】【调整互信息（AMI）、纯度（Purity）、隐藏表示学习的分类准确率】【神经概率软逻辑对话结构归纳】

151. **Limitations of Language Models in Arithmetic and Symbolic Induction** [ACL2023] [[paper link](https://aclanthology.org/2023.acl-long.516.pdf)]

      揭示了LLMs在简单符号操作和长数字运算的归纳局限性，提出通过逐步教学和显式定位提升模型性能。方法：用动作序列模拟人类教学，将复杂任务分解为原子操作（如移动、复制），确保模型逐步正确执行。
【复制、反转、加法】【自定义生成的数字序列和符号列表】【准确率，分内分布和OOD测试】【LLMs】

152. **Human-in-the-Loop Schema Induction** [ACL2023] [[paper link](https://aclanthology.org/2023.acl-demo.1.pdf)]

      提出一种人机协同的事件模式归纳方法，利用GPT-3生成候选模式并通过人工干预提升质量，解决了纯自动化方法的领域迁移和语义一致性问题。方法：四阶段流水线（生成→抽取→建图→grounding），结合大模型生成与人工编辑。
【事件模式归纳、图构建、节点 grounding】【自建五个场景（如“网络攻击”“医疗救治”）】【评估基于人工标注的步骤/节点准确率、图编辑距离、grounding成功率】【GPT-3（生成步骤/节点/关系）、AllenNLP SRL模型（节点抽取）、BART（entailment评分）、GloVe（相似度计算）】

153. **Knowledge Base Question Answering for Space Debris Queries** [ACL2023] [[paper link](https://aclanthology.org/2023.acl-industry.47.pdf)]

      开发了一个透明、可验证的空间碎片问答系统，通过程序归纳和迁移学习，让模型从少量标注数据中归纳出复杂查询的逻辑，解决了领域数据稀缺问题。方法：分阶段生成查询程序（草图→参数填充），结合领域预训练和GPT-3数据增强提升泛化能力。
【复杂知识库问答，支持多跳查询】【KQA Pro、DISCOS-Questions-Programs (DQP)】【各组件（函数、实体、关系等）预测准确率，整体程序生成准确率】【LLMs】

154. **Categorial Grammar Induction from Raw Data** [ACL2023] [[paper link](https://aclanthology.org/2023.findings-acl.149.pdf)]

      研究如何从儿童语言数据中无监督地归纳出基本范畴语法规则，验证了语法结构的可学习性，并通过引入分支偏置提升了性能。方法：扩展了现有的PCFG神经网络模型，通过约束语法范畴的组合方式学习更高效的语法规则。
【无监督的语法归纳】【CHILDES中的英语儿童导向语料库】【召回-同质性和未标记F1分数】【基于神经网络的范畴语法归纳模型，扩展自PCFG模型】

155. **Improving Diachronic Word Sense Induction with a Nonparametric  Bayesian method** [ACL2023] [[paper link](https://aclanthology.org/2023.findings-acl.567.pdf)]

      通过非参数贝叶斯和动态嵌入模型，从生物医学文本中自动归纳词义的动态演变，解决了参数化模型依赖预设词义数量的局限性。方法：结合HDP的无限聚类能力和DETM的语义嵌入，实现了更准确的词义推断和演变建模。
【历时词义归纳（DWSI）,即从时间标注的文本中推断词义的动态变化】【生物医学领域的PubMed和MeSH时间标注数据集】【全局匹配（Global Matching）、V-measure（同质性和完整性）、词义涌现年份误差（MAE）】【分层狄利克雷过程HDP】

156. **Acquiring Frame Element Knowledge with Deep Metric Learning  for Semantic Frame Induction** [ACL2023] [[paper link](https://aclanthology.org/2023.findings-acl.596.pdf)]

      通过深度度量学习优化预训练模型的嵌入空间，解决了语义框架归纳中论元角色区分的问题，显著提升了聚类性能。方法：结合Triplet和ArcFace损失微调BERT，并提出了框架内聚类策略以更好地捕捉角色特异性。
【论元聚类（argument clustering），即根据语义角色对论元进行分组】【FrameNet 1.7】【纯度（PU）、逆纯度（IPU）、F-SCORE（PIF）、B-CUBED精确度（BCP）、召回率（BCR）和F-SCORE（BCF）】【BERT】

157. **Few-shot Dialogue Strategy Learning  for Motivational Interviewing via Inductive Reasoning**  [ACL2024] [[paper link](https://aclanthology.org/2024.findings-acl.782.pdf)]

      提出了一种归纳推理框架DIIR，从专家对话中归纳出有效的自然语言策略，在数据稀缺时提升对话系统的表现。DIIR通过LLM从有限数据生成潜在策略，并通过生成-验证循环优化这些策略。
【动机性访谈对话生成】【AnnoMI】【MI不一致行为比例（%MI-i）、复杂反思比例（C/S）、主动倾听行为比例（%AL）】【GPT-3.5和GPT-4】

158. **SIP: Injecting a Structural Inductive Bias into a Seq2Seq Model by Simulation**  [ACL2024] [[paper link](https://aclanthology.org/2024.acl-long.355.pdf)]

      让seq2seq模型模拟有限状态转换器FSTs的行为，可以为模型注入结构化的归纳偏置，提升模型的泛化和小样本学习能力。
【合成FST任务、自然语言任务】【合成数据：自动生成的FST输入/输出对；自然数据：Wikipron（音素转换）、SyGuS竞赛数据（文本编辑）】【准确率、编辑距离、音素错误率】【seq2seq模型】

159. **LLM as Prompter: Low-resource Inductive Reasoning on Arbitrary  Knowledge Graphs** [ACL2024] [[paper link](https://aclanthology.org/2024.findings-acl.224.pdf)]

      通过LLMs生成提示图增强GNN推理器，提升模型在零样本、少样本场景下的归纳推理能力，保持对未见知识图谱的泛化性。prompt graph：利用LLM通过简洁的关系描述推断实体类型，构建关系间的交互边。
【知识图谱归纳推理、零样本、单样本和三样本场景】【基于FB15k237、Wikidata68K、NELL-995构建】【MRR和Hits@N】【Llama2-7B/13B、Mistral-7B、GPT-3.5、GPT-4】

160. **DM-BLI: Dynamic Multiple Subspaces Alignment for Unsupervised  Bilingual Lexicon Induction** [ACL2024] [[paper link](https://aclanthology.org/2024.acl-long.112.pdf )]

      提出动态多子空间对齐方法（DM-BLI），通过无监督聚类和对比学习，从词嵌入中归纳出子空间结构并优化映射，显著提升了远距离和低资源语言对的双语词典归纳性能。方法总结：DM-BLI通过聚类发现子空间，结合对比学习和动态更新，为每个子空间对学习定制化的映射矩阵。
【无监督双语词典归纳】【MUSE双语词典，使用fastText在Wikipedia上训练的词向量】【Precision@1和Precision@5】【DM-BLI】

161. **ItD: Large Language Models Can Teach Themselves  Induction through Deduction** [ACL2024] [[paper link](https://aclanthology.org/2024.acl-long.150.pdf)]

      提出ItD框架，利用大语言模型的演绎能力生成数据并优化归纳推理，显著提升了模型从少量样本中学习通用规则的能力。方法总结：通过演绎生成数据，再用朴素贝叶斯方法优化模型对样本的利用，实现更高效的归纳推理。
【归纳推理任务，包括语义归纳和符号归纳】【Instruction Induction和List Function】【执行分数，即模型生成的变换规则在测试样本上的正确率】【LLMs】

162. **Temporal Knowledge Question Answering  via Abstract Reasoning Induction** [ACL2024] [[paper link](https://aclanthology.org/2024.acl-long.267.pdf)]

      提出 ARI 框架，让 LLM 从历史推理链中“归纳”出抽象方法，再把事实查询与策略决策解耦，提升了时间知识问答的准确率。方法：把问答拆成“归纳式策略选择 + 事实执行”两阶段循环，直到得出答案。
【Temporal Knowledge Graph Question Answering（TKGQA）】【MULTITQ、CRONQUESTIONS】【Overall Accuracy】【ARI】

163. **Domain Adaptation for Subjective Induction Questions Answering on  Products by Adversarial Disentangled Learning** [ACL2024] [[paper link](https://aclanthology.org/2024.acl-long.491.pdf)]
     
      提出领域自适应模型，通过解耦领域无关和特定知识，解决低资源领域主观问答的数据不均衡问题，生成融合事实与多视角观点的归纳性答案。方法总结：基于对抗解耦学习分离跨领域共享模式，结合对比学习和强化学习优化答案生成。
【主观归纳问答（SunPQA）】【SupQA】【BLEU、ROUGE（评估生成质量），人工评估】【BART】

164. **Structural Optimization Ambiguity and Simplicity Bias  in Unsupervised Neural Grammar Induction** [ACL2024] [[paper link](https://aclanthology.org/2024.findings-acl.898.pdf)]

      研究无监督神经语法归纳（UNGI）中的两个问题：结构优化模糊性（SOA）和结构简单性偏差（SSB）。这些导致模型随机选择语法结构（高方差）或生成过于简单的解析树（低表达能力），影响性能。通过预训练解析器筛选高质量解析树作为训练偏置，减少语法归纳中的模糊性和简单性偏差
【无监督语法归纳】【Penn Treebank (PTB)、Chinese Penn Treebank (CTB)、SPMRL多语言数据集】【未标记句子F1分数、负对数似然、规则利用率】【PCFG】

165. **Improving Word Usage Graphs with Edge Induction** [ACL2024] [[paper link](https://aclanthology.org/2024.lchange-1.9.pdf)]

      通过预测缺失的边来增强稀疏的词用法图（WUGs），从而更高效地发现词义，减少人工标注需求。其方法利用了图中已有的结构规律和上下文语义信息，通过归纳学习补全缺失的边。方法：结合图结构特征和预训练语言模型预测缺失的边，再用聚类算法分析增强后的图以发现词义。
【词义聚类和词义变化检测】【DWUG_DE、resampled dataset】【加权平均Spearman相关系数、调整兰德指数ARI】【基于逻辑回归的边预测模型、聚类算法】

166. **Towards more complete solutions for Lexical Semantic Change:  an extension to multiple time periods and  diachronic word sense induction** [ACL2024] [[paper link](https://aclanthology.org/2024.lchange-1.10.pdf)]  
      扩展词汇语义变化研究，从简单的两时间段建模升级到多时间段的动态分析，通过归纳已有数据中的词义规律来预测和追踪语义演变。方法：提出多种动态聚类和评估策略，结合时间序列分析，从已有词义中归纳规律以建模多时间段的语义变化。
【多时间段的词汇语义变化检测（LSC）和历时词义归纳】【LSC基准】【聚类质量（如对齐一致性）和语义变化显著性】【上下文嵌入模型、聚类】

167. **Towards an Onomasiological Study of Lexical Semantic Change through  the Induction of Concepts** [ACL2024] [[paper link](https://aclanthology.org/2024.lchange-1.15.pdf)]

      词汇语义变化（LSC）研究主要从词到概念的视角出发，而忽略了概念到词的视角。后者能揭示词汇命名方式的演变。提出通过自动归纳概念来填补这一空白，方法是用XLM-R嵌入和层次聚类从词例中归纳概念簇，支持词义和命名演变的双重分析。
【历时概念归纳与语义变化分析】【法语历时语料库Presto Corpus】【人工评估概念簇质量，JSD量化词义变化】【XLM-R（提取词例嵌入） + 层次聚类】

168. **The Role of Deductive and Inductive Reasoning in Large Language Models**  [ACL2025] [[paper link](https://aclanthology.org/2025.acl-long.820.pdf)]

      针对LLMs静态推理的局限性，提出了De-In-Ductive（DID）方法，通过动态结合归纳和演绎推理，利用Littlestone维度和信息熵评估任务复杂度，并逐步分解问题，引导模型从简单到复杂逐步解决任务。
【逻辑推理、数学推理和时序推理】【AIW、MR-GSM8K、Holiday Puzzle】【准确率、计算成本】【GPT-3.5 Turbo、GPT-4o、Claude 3.5 Sonnet】

169. **Measuring What Matters: Evaluating Ensemble LLMs with Label  Refinement in Inductive Coding**  [ACL2025] [[paper link](https://aclanthology.org/2025.findings-acl.563.pdf)]

      针对单一LLM在归纳编码中的不一致性，文章通过集成学习模拟“多专家共识”，结合标签精炼优化归纳结果。方法：用多个小型LLM生成候选编码，通过moderator机制和相似性合并实现精炼，最终以复合指标评估。
【自动化归纳编码】【1,000个“文本-编码”对（600条社会科学研究数据 + 400条SemEval-2014评论数据），另用100条ChatGPT用户评论作为独立测试集】【复合评分（核心指标）、BERTScore、ROUGE、覆盖度、新颖性】【Llama3-8B、Falcon-7B、Mistral-7B、Vicuna-7B等】

170.**Patterns Over Principles: The Fragility of Inductive Reasoning in LLMs  under Noisy Observations**  [ACL2025] [[paper link](https://aclanthology.org/2025.findings-acl.1006.pdf)]

      针对LLM在噪声数据中归纳规则时的脆弱性，通过多样化假设和迭代修正来增强推理稳定性。提出Sample-steered Rule Refinement (SRR)，通过生成多样规则候选并基于执行反馈迭代优化。
【Robust Rule Induction（从含噪声的输入-输出对中推断潜在规则）】【Arithmetic（非十进制加法）；Cryptography（替换密码）；List Functions（列表操作）】【整体正确率、噪声与无噪声条件下推理一致性】【SRR】

171.**Inductive Linguistic Reasoning with Large Language Models**  [ACL2025] [[paper link](https://aclanthology.org/2025.findings-acl.1171.pdf)]

      针对低资源语言缺乏标注，通过类比提示让模型从少量示例中归纳语言规则，并利用同语系语言的相似性生成辅助示例，增强跨语言推理能力。方法：首先生成同语系类比示例，再结合原始示例进行上下文学习。
【语言学谜题】【model_ing和LINGOLY】【精确匹配、ChrF2和BLEU分数】【LLMs】

172.**Theorem-of-Thought: A Multi-Agent Framework for Abductive, Deductive,  and Inductive Reasoning in Language Models**  [ACL2025] [[paper link](https://aclanthology.org/2025.knowllm-1.10.pdf)]

      针对LLMs推理缺乏逻辑严谨性的问题，通过模拟人类多模态推理（溯因、演绎、归纳），结合贝叶斯验证，提升复杂任务的可靠性和可解释性。方法：三代理（溯因/演绎/归纳）生成结构化推理图，经NLI验证后选择最优解。
【符号推理和数值推理】【WebOfLies、MultiArith】【答案准确率】【本文提出的Theorem-of-Thought (ToTh)框架】

173.**Inductive Learning on Heterogeneous Graphs Enhanced by LLMs for  Software Mention Detection** [ACL2025] [[paper link](https://aclanthology.org/2025.sdp-1.16.pdf)]

      针对多语言NER/RE任务中结构化知识融合的难题，通过异构图谱归纳学习与LLM验证协同，提升模型泛化性。方法：异构图谱编码+归纳式GraphSAGE分类+LLM逻辑验证。
【多语言命名实体识别（NER）和关系抽取（RE），聚焦软件提及检测】【SOMD 2025竞赛数据集】【Macro F1、Precision、Recall】【基础模型：GraphSAGE；LLM验证层：DeepSeek v3】

174.**Learn to Memorize: Scalable Continual Learning in Semiparametric  Models with Mixture-of-Neighbors Induction Memory**  [ACL2025] [[paper link](https://aclanthology.org/2025.acl-long.1385.pdf)] 

      针对半参数化模型记忆效率低的问题，提出MoNIM，通过结合注意力头的归纳能力和前馈网络的记忆机制，实现动态、可扩展的持续学习。方法：将非参数化记忆改造为可学习的类前馈网络旁路层。
【语言建模和下游任务】【News Crawl-20H1、WikiEvent-20H1、ACL论文数据集】【困惑度、记忆率、准确率】【MoNIM（基于kNN-LM改进的可学习记忆模块）】

175.**Programming by Examples Meets Historical Linguistics: A Large  Language Model Based Approach to Sound Law Induction** [ACL2025] [[paper link](https://aclanthology.org/2025.acl-long.1432.pdf)] 
      
      提出利用LLMs的“示例编程”（Programming by Examples, PBE）能力来自动生成音变规则，并通过研究“结构”与“实质”在数据分布中的平衡，优化模型的归纳性能。
【音变规律归纳】【包括Proto-Polynesian（Pol）和Proto-Tangkhulic（Ptk）等低资源语言的真实数据，以及生成的合成数据】【编辑距离奖励、通过率】【LLMs】

176.**Semantic Frame Induction from a Real-World Corpus** [ACL2025] [[paper link](https://aclanthology.org/2025.acl-srw.72.pdf)] 

      语义框架归纳依赖FrameNet等人工标注资源，在真实语言覆盖上存在局限，通过深度度量学习和真实语料（C4）的结合，验证了语义框架归纳方法的泛化能力。方法：基于BERT嵌入和深度度量学习的聚类方法，通过掩码技术和多阶段聚类优化框架归纳效果。
【语义框架归纳】【Colossal Clean Crawled Corpus（C4）作为真实语料，FrameNet 1.7作为评估基准】【B-cubed F1（BCF）、Purity与Inverse Purity的调和平均】【基于BERT的上下文嵌入模型】

177.**Improve Rule Retrieval and Reasoning with Self-Induction and Relevance  ReEstimate** [ACL2025] [[paper link](https://aclanthology.org/2025.findings-acl.286.pdf)] 

      针对规则检索中查询与规则的语义不对齐问题，利用LLM的归纳能力从查询中抽象出潜在规则（Self-Induction Augmented Retrieval ，SIAR），并通过相关性重估优化检索结果，从而提升推理性能。
【规则检索与推理】【Clutrr、ULogic、CAIL2018】【检索性能（Recall@1/5/10）、推理性能（Match）】【SIAR】

178.**IDEA: Enhancing the Rule Learning Ability of Large Language Model  Agent through Induction, Deduction, and Abduction** [ACL2025] [[paper link](https://aclanthology.org/2025.findings-acl.698.pdf)]

      针对LLM在交互式规则学习中的不足，文章提出IDEA框架，通过模拟人类“假设生成（溯因）-验证（演绎）-修正（归纳）”的循环，提升模型动态学习能力。
【在交互式环境中学习隐藏规则并解决问题】【RULEARN基准，包含三种手动设计的谜题类型】【任务成功率、重复动作次数、有效归纳率】【IDEA】

179.**In the LLMera, Word Sense Induction remains unsolved** [ACL2025] [[paper link](https://aclanthology.org/2025.findings-acl.882.pdf)] 

      针对词义归纳（WSI）评估中多义词分布不自然的问题，提出基于自然分布的评估框架，并通过数据增强（如LLM生成、语料库和词典）和半监督学习（如Wiktionary）提升词义归纳的性能。
【词义归纳】【SemCor-WSI（基于SemCor构建）、SemEval 2010 Task 14、SemEval 2013 Task 13】【F-B³、NMI、V-measure、Paired F-score等】【基于BERT和Wiktionary的半监督模型】


## Others
   
1. **Inductive Representation Learning on Large Graphs** [NIPS2017] [[paper link](https://arxiv.org/pdf/1706.02216)]

   GraphSAGE是一个通用的归纳式框架，它利用节点的特征信息，可以高效地为以前未见过的数据生成节点embedding表示。

2. **Inductive Quantum Embedding** [NIPS2020] [[paper link](https://proceedings.neurips.cc/paper_files/paper/2020/file/b87039703fe79778e9f140b78621d7fb-Paper.pdf)]

   原始的 Quantum Embedding (QE)方法只能用于transductive设置，现在在QE损失中引入inductive特征映射项。

3. **Grounding inductive biases in natural images: invariance stems from variations in data** [NIPS2021] [[paper link](https://arxiv.org/pdf/2106.05121)]

   传统观点认为，CNN中的空间平移不变性来自网络结构本身的归纳偏置（例如卷积和池化操作），但这篇论文质疑了这个观点，提出了一个新的假设：不变性并不主要来自模型结构中的归纳偏置，而是来自训练数据中天然存在的变换多样性（variations in natural images）。

4. **The Inductive Bias of Quantum Kernels** [NIPS2021] [[paper link](https://arxiv.org/pdf/2106.03747)]

   揭示quantum kernel中inductive bias与泛化的关系，没有归纳偏置的指数空间”会导致泛化困难，而偏置引入又伴随测量成本的指数级增长。

5. **A Closer Look at Learned Optimization: Stability, Robustness, and Inductive Biases** [NIPS2022] [[paper link](https://papers.nips.cc/paper_files/paper/2022/file/184c1e18d00d7752805324da48ad25be-Paper-Conference.pdf)]

   借助动力系统理论分析优化器动态，从中提炼出有助于稳定与泛化的归纳偏置，以优化训练。

6. **SHINE: SubHypergraph Inductive Neural nEtwork** [NIPS2022] [[paper link](https://papers.nips.cc/paper_files/paper/2022/file/7721f1fea280e9ffae528dc78c732576-Paper-Conference.pdf)]

   有关超图预测与类比。

7. **Maximum Class Separation as Inductive Bias in One Matrix** [NIPS2022] [[paper link](https://arxiv.org/abs/2206.08704)]

   最大类别间隔（maximum class separation）是传统机器学习（例如 SVM）中的重要归纳偏置。本文试图将将“最大类别间隔”以结构级别的归纳偏置嵌入网络架构中。

8. **The Inductive Bias of Flatness Regularization for Deep Matrix Factorization** [NIPS2023] [[paper link](https://papers.nips.cc/paper_files/paper/2023/file/5927edd18c5dd83aa8936a4610c72029-Paper-Conference.pdf)]

   核心问题：深度神经网络在过参数化（参数远多于样本数）情况下仍能良好泛化，这与传统统计学习理论相矛盾。研究空白：平坦正则化（如L2正则化、SGD隐式偏好）如何影响深度矩阵分解（DMF）模型的优化动态？深度（层数）如何改变模型对低秩解的偏好？

9. **CAT-Walk: Inductive Hypergraph Learning via Set Walks** [NIPS2023] [[paper link](https://papers.nips.cc/paper_files/paper/2023/file/6739d8df16b5bce3587ca5f18662a6aa-Paper-Conference.pdf)]

   同样与超图有关。
   
10. **PAC-Bayes Generalization Certificates for Learned Inductive Conformal Prediction** [NIPS2023] [[paper link](https://papers.nips.cc/paper_files/paper/2023/file/9235c376df778f1aaf486a882afb7471-Paper-Conference.pdf)]

    在Inductive Conformal Prediction (ICP)：一种后验式、不要求数据交换性假设的保序预测方法，属于归纳学习范式中给出泛化界的inductive bias。

11. **PID‑Inspired Inductive Biases for Deep Reinforcement Learning in Partially Observable Control Tasks** [NIPS2023] [[paper link](https://papers.nips.cc/paper_files/paper/2023/file/ba1c5356d9164bb64c446a4b690226b0-Paper-Conference.pdf)]

    以PID控制为启发，设计一种既能有效编码历史信息又具备强鲁棒性的inductive bias。

12. **MOTIVE: A Drug-Target Interaction Graph For Inductive Link Prediction** [NIPS2024] [[paper link](https://papers.nips.cc/paper_files/paper/2024/file/fdb3fa770c2e0ecbb4b7dc7083ef5be9-Paper-Datasets_and_Benchmarks_Track.pdf)]

    靶向药。
    
13. **Theoretical Analysis of the Inductive Biases in Deep Convolutional Networks** [NIPS2024] [[paper link](https://papers.nips.cc/paper_files/paper/2023/file/eb1bad7a84ef68a64f1afd6577725d45-Paper-Conference.pdf)]

    系统性地解析这些结构形成的归纳偏置，以在理论上解释CNN的高效学习能力。

14. **Inductive-bias-driven Reinforcement Learning for Efficient Schedules in Heterogeneous Clusters** [ICML2020] [[paper link](https://proceedings.mlr.press/v119/banerjee20a/banerjee20a.pdf)]

    通过系统拓扑与性能计数器定义的架构依赖，提供inductive bias，引导RL agent（异构集群调度）学习有效状态表示。

15. **Provable Guarantees for Decision Tree Induction: The Agnostic Setting** [ICML2020] [[paper link](https://proceedings.mlr.press/v119/blanc20a/blanc20a.pdf)]

    与决策树。
    
16. **ModLaNets: Learning Generalisable Dynamics via Modularity and Physical Inductive Bias** [ICML2022] [[paper link](https://proceedings.mlr.press/v162/lu22c/lu22c.pdf)]

    与动力单元。

17. **Inductive Gradient Adjustment for Spectral Bias in Implicit Neural Representations** [ICML2025] [[paper link](https://openreview.net/pdf?id=pYMZQtkp3F)]

    从训练动力学视角出发，设计不依赖模型架构变化的 梯度调整策略，使MLP能有效学习高频分量。

18. **Map Induction: Compositional spatial submap learning for efficient exploration in novel environments** [ICLR2022] [[paper link](https://arxiv.org/pdf/2110.12301)]

    论文假设人类在探索未知环境时，并非一片空白地随机探索，而是会根据此前看到过的相似结构来归纳新环境的未观测区域，从而更加高效地规划路线和搜寻目标。这一认知机制可以用分层贝叶斯与程序归纳模型来模拟。

19. **Enhancing the Inductive Biases of Graph Neural ODE for Modeling Physical Systems** [ICLR2023] [[paper link](https://arxiv.org/pdf/2209.10740)]

    引入 Graph Neural ODE（GNODE）：对粒子系统建模时，利用 GNN 构造连续时间动力学方程，作为 NODE 执行积分预测。相比传统输入位置 + 速度，GNODE 仅将 位置作为输入 且对加速度进行预测，为 second-order bias 做准备。inductive bias 通过将物理约束与系统特性（energy conservation、Newton’s law）编码为模型架构的一部分，被强制注入 GNODE。

20. **SEGNO: Generalizing Equivariant Graph Neural Networks with Physical Inductive Biases** [ICLR2024] [[paper link](https://arxiv.org/pdf/2308.13212)]

    虽然等变图神经网络（Equivariant GNNs）在模拟多对象物理系统中广泛使用，但其泛化能力仍受限，因为未充分融入关键的物理归纳偏好。

21. **Interpretable Vision‑Language Survival Analysis with Ordinal Inductive Bias for Computational Pathology** [ICLR2025] [[paper link](https://arxiv.org/pdf/2409.09369)]

    在计算病理学中，对全切片影像（WSI）进行预后生存分析（Survival Analysis，SA）通常面临两大挑战：病患数据稀缺（通常少于千人）和仅有粗粒度（病人级别）的监督标签。多实例学习（MIL）框架下，模型难以从海量切片图像中学习有效的预后表示。作者提出利用 Vision‑Language Foundation Models（如病理 VL 模型） 引入语言中的预后先验知识，以补强弱监督信号，提高数据效率与可解释性。
    
