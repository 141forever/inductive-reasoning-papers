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

5.  **Code-Driven Inductive Synthesis: Enhancing Reasoning Abilities of Large Language Models with Sequences** [Arxiv2025] [[paper link](https://arxiv.org/abs/2503.13109)]
   
      提出了一种基于数列的类比推理合成数据管线，以code为呈现形式构建了一批SFT合成数据，有效的提高了LLMs的类比推理和code推理能力。
   
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
   
## Evaluations

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

   对于模型优化过程神经切线核（NTK）的inductive bias的探索，本文给出了一种基于核函数的提高方法。【图像分类】【CIFAR-10，MNIST】【准确率】【CNN模型】
   
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
