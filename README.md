# The Paper Collection of Inductive Reasoning

## Benchmarks, Datasets and Tasks

1.  **On the Transfer of Inductive Bias from Simulation to the Real World: a New Disentanglement Dataset** [NIPS2019] [[paper link](https://papers.nips.cc/paper_files/paper/2019/file/d97d404b6119214e4a7018391195240a-Paper.pdf)]

      提出了一个数据集，通过真实机械臂采样而来的，包含超过一百万张物理三维物体的图像，拥有三个子集，以提升模型的迁移效果和inductive bias。【MPI3D】【disentanglement metrics】【各类VAE模型】
    
2.  **Learning abstract structure for drawing by efficient motor program induction** [NIPS2020] [[paper link](https://papers.nips.cc/paper_files/paper/2020/file/1c104b9c0accfca52ef21728eaf01453-Paper.pdf)]

     研究人类如何几次演练后便构建出抽象的、可复用的程序性先验知识，供模型学习。揭示两大元学习原则：abstraction（抽象）和compositionality（组合）是构成人类快速学习结构化表示的关键，同时强调motor efficiency的先验在真实行为再现中必不可少。【手绘风格图形】【stroke order, motor trajectory, 模型重现度】【PI,Hybrid等】

3.  **Code-Driven Inductive Synthesis: Enhancing Reasoning Abilities of Large Language Models with Sequences** [Arxiv2025] [[paper link](https://arxiv.org/abs/2503.13109)]
   
      提出了一种基于数列的类比推理合成数据管线，以code为呈现形式构建了一批SFT合成数据，有效的提高了LLMs的类比推理和code推理能力。
   
      
   
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

   提出了一种结构化变分自编码器（Structured Variational Autoencoder）模型，利用连续松弛的条件随机场（CRF）推理机制，自动从文本数据中归纳出控制句子生成结构的潜在模板。【文本生成】【数据到文本生成R4R和无监督同义句生成ParaNMT】【BLEU，ROUGE，Success@1】【CRF模型】

9. **Fine-grained Generalization Analysis of Inductive Matrix Completion** [NIPS2021] [[paper link](https://proceedings.neurips.cc/paper_files/paper/2021/file/d6428eecbe0f7dff83fc607c5044b2b9-Paper.pdf)]

   旨在缩小归纳矩阵补全在理论分析方面与标准矩阵补全之间的差距：此前在无分布假设条件下，IMC 的样本复杂度最高达 $O(rd^2)$，作者努力证明更优的边界，并希望引入更高效的“带权迹范数”正则策略。【矩阵补全】【推荐数据】【理论界与实证loss】【IMC/ATR】

10. **Leveraging the Inductive Bias of Large Language Models for Abstract Textual Reasoning** [NIPS2021] [[paper link](https://arxiv.org/abs/2110.02370)]

     预训练的大型语言模型（如T5、GPT-3）是否具备对抽象文本推理任务（如容器操作、导航路径推断）的归纳偏置？微调 T5，设计 container/navigation/composite 任务，对比 tabula rasa 和英语 vs 猫语模板。【NLP任务泛化】【每个任务构造成训练集、插值和外推测试集，用于各类泛化测试（基数、符号、组合）】【Exact match,BLEU】【T5】

11. **Tailoring: encoding inductive biases by optimizing unsupervised objectives at prediction time** [NIPS2021] [[paper link](https://arxiv.org/abs/2009.10623)]

     监督学习中，辅助损失（auxiliary loss，如物理守恒、对比学习约束等）只在训练阶段使用，会带来泛化缺口，并且训练优化的是合并目标而非关注的任务损失。通过在inference时执行unsupervised优化，让inductive bias可对每个输入样本直接生效。【多任务】【多数据】【多指标】【多模型】

12. **Open Rule Induction** [NIPS2021] [[paper link](https://arxiv.org/pdf/2110.13577)]

     传统基于知识库（KB）的规则归纳只能从已有实体和关系中挖掘模式，表达能力有限；而当前基于语言模型（LM）的规则生成，如 Comet，依赖人工标注的规则，缺乏真正“归纳”能力，生成结果受限于训练样本，难以创造真实通用规则。提出 Open Rule Induction（ORI）问题：给定前提句子如 (x, rp, y)，从 LM 中挖掘 top‑k 个有效的结论 (x, rh, y) 规则，自动诱导的规则。【Open Rule Induction, 关系抽取】【自动生成开放规则与公开关系数据】【质量,F1】【BART】

13. **ViTAE: Vision Transformer Advanced by Exploring Intrinsic Inductive Bias** [NIPS2021] [[paper link](https://arxiv.org/pdf/2106.03348)]

     ViT将图像拆成1D token序列，缺乏CNN的内在归纳偏置（intrinsic inductive bias），特别是在局部结构建模与多尺度变化上的能力。结果它需要极大规模数据和长训练才能“间接”学会这些偏置。本文将CNN的 locality和scale‑invariance偏置直接引入ViT。【图像分类和下游任务】【ImageNet-1K和下游数据集】【top1等】【ViT系列】
    
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

21. **** [NIPS2023] [[paper link]()]

     【知识图谱补全】【WN18RR-Ind,FB15k-237-Ind】【MRR（平均倒数排名）, Hit@1/3/10】【直推式：TransE,RotatE,ComplEx。归纳式：GraIL,CoMPILE,Meta-KGC】

   
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
