
# [Proceedings of Machine Learning Research](https://proceedings.mlr.press/v250/)

## Medical Imaging with Deep Learning, 3-5 July 2024, Paris, France

---

## 1. A Comprehensive Benchmark of Supervised and Self-supervised Pre-training on Multi-view Chest X-ray Classification
- **任务**：研究多视图胸部X光图像分类任务中的预训练策略，特别是在低数据量场景下的性能表现。
- **数据集**：PadChest 数据集，包含160,868张胸部X光图像，涵盖多种病理标签。
- **方法**：通过对比自然图像和医学图像预训练的监督学习和自监督学习方法，评估其在多视图胸部X光分类任务中的效果。提出了一个四阶段的预训练策略，包括监督学习、自监督学习、医学图像监督学习和自监督学习，并在不同数据量（1%、10%、100%）下进行微调，验证其在低数据量场景中的优势。
- **论文链接**：[A Comprehensive Benchmark of Supervised and Self-supervised Pre-training on Multi-view Chest X-ray Classification ](https://raw.githubusercontent.com/mlresearch/v250/main/assets/afzal24a/afzal24a.pdf)

---

## 2. Interpretable Uncertainty-Aware Deep Regression with Cohort Saliency Analysis for Three-Slice CT Imaging Studies
- **任务**：开发一种用于三切面CT图像的不确定性感知深度回归方法，用于量化肝脏、内脏脂肪组织和大腿肌肉的横截面积。
- **数据集**：SCAPIS 和 IGT 研究中的2,724名受试者的CT图像数据。
- **方法**：提出了一种基于ResNet-50的深度回归网络，通过预测均值和方差来量化目标区域的面积，并结合Grad-CAM生成队列显著性图，用于解释模型预测。通过图像配准技术将显著性图对齐到公共模板空间，实现群体级别的可视化分析。
- **论文链接**：[Interpretable Uncertainty-Aware Deep Regression with Cohort Saliency Analysis for Three-Slice CT Imaging Studies](https://raw.githubusercontent.com/mlresearch/v250/main/assets/ahmad24a/ahmad24a.pdf)

---

## 3. Distance-Aware Non-IID Federated Learning for Generalization and Personalization in Medical Imaging Segmentation
- **任务**：提出一种基于距离感知的非独立同分布（non-IID）联邦学习方法，用于医学图像分割任务，优化模型的泛化和个性化能力。
- **数据集**：FeTS、Prostate 和 Fed-KITS2019 数据集，涵盖多种放射学成像场景。
- **方法**：结合医学图像嵌入空间的距离测量和元数据的统计距离，通过降低最远客户端的贡献来优化模型泛化能力，并通过基于距离的聚类实现客户端的个性化。验证了该方法在多个公共数据集上的有效性。
- **论文链接**：[Distance-Aware Non-IID Federated Learning for Generalization and Personalization in Medical Imaging Segmentation](https://raw.githubusercontent.com/mlresearch/v250/main/assets/alekseenko24a/alekseenko24a.pdf)

---

## 4. FluidRegNet: Longitudinal registration of retinal OCT images with new pathological fluids
- **任务**：开发一种用于视网膜光学相干断层扫描（OCT）图像的纵向配准方法，专门处理新病理液体的出现和消失。
- **数据集**：包含33名CSCR患者的61只眼睛的369张OCT图像。
- **方法**：提出FluidRegNet，通过预测液体起源的位置（以稀疏强度偏移形式）并将其配准到后续图像中的受影响区域，生成更准确的变形场。结合基于区域的正则化策略，该方法能够处理新出现液体导致的组织变形，并用于无监督的液体分割。
- **论文链接**：[FluidRegNet: Longitudinal registration of retinal OCT images with new pathological fluids](https://raw.githubusercontent.com/mlresearch/v250/main/assets/andresen24a/andresen24a.pdf)

---

## 5. HoVer-NeXt: A Fast Nuclei Segmentation and Classification Pipeline for Next Generation Histopathology
- **任务**：开发一种快速、准确的基于H&E染色的细胞核分割和分类模型，用于大规模结直肠癌队列研究。
- **数据集**：扩展的Lizard CRC细胞核数据集，包含6种细胞类型，并新增了有丝分裂类。
- **方法**：提出HoVer-NeXt模型，基于ConvNeXt-v2编码器和U-Net架构，结合类平衡采样和焦点损失优化性能。通过高效的WSI推理流程，该方法在多个数据集上实现了快速推理和高准确率，同时提供了额外的验证数据集。
- **论文链接**：[HoVer-NeXt: A Fast Nuclei Segmentation and Classification Pipeline for Next Generation Histopathology](https://raw.githubusercontent.com/mlresearch/v250/main/assets/baumann24a/baumann24a.pdf)

---

## 6. Combining Reconstruction-based Unsupervised Anomaly Detection with Supervised Segmentation for Brain MRIs
- **任务**：结合重建型无监督异常检测（UAD）和自监督分割方法，提高脑部MRI异常检测的分割性能和泛化能力。
- **数据集**：IXI数据集用于训练扩散模型，BRATS和ATLAS数据集用于弱监督学习和评估。
- **方法**：提出SADM框架，结合扩散模型生成伪健康重建和基于残差的U-Net分割网络。通过将监督预测与无监督异常图融合，该方法在已知和未知病理类型上均表现出色。
- **论文链接**：[Combining Reconstruction-based Unsupervised Anomaly Detection with Supervised Segmentation for Brain MRIs](https://raw.githubusercontent.com/mlresearch/v250/main/assets/behrendt24a/behrendt24a.pdf)

---

## 7. GazeDiff: A radiologist visual attention guided diffusion model for zero-shot disease classification
- **任务**：利用放射科医生的眼动模式作为控制信号，改进扩散模型在胸部X光图像生成和零样本分类中的性能。
- **数据集**：公开的胸部X光眼动数据集（EGD-CXR），包含1083张图像及其转录文本。
- **方法**：提出GazeDiff模型，将眼动模式作为额外控制信号，结合放射科医生的转录文本，生成具有疾病特征的医学图像，并用于零样本分类任务。通过密度估计，该方法在肺炎和结核病分类上优于基线模型。
- **论文链接**：[GazeDiff: A radiologist visual attention guided diffusion model for zero-shot disease classification](https://raw.githubusercontent.com/mlresearch/v250/main/assets/bhattacharya24a/bhattacharya24a.pdf)

---

## 8. Network conditioning for synergistic learning on partial annotations
- **任务**：提出一种用于部分标注区域分割的条件网络框架，优化多器官分割任务中的数据利用效率。
- **数据集**：包含289个胎儿MRI扫描的内部数据集，部分标注了5个区域。
- **方法**：提出CoNeMOS框架，通过特征线性调制（FiLM）层实现条件网络，动态调整网络以适应不同标签。该方法在胎儿MRI数据上表现出色，优于现有的部分监督学习方法。
- **论文链接**：[Network conditioning for synergistic learning on partial annotations](https://raw.githubusercontent.com/mlresearch/v250/main/assets/billot24a/billot24a.pdf)

---

## 9. There Are No Shortcuts to Anywhere Worth Going: Identifying Shortcuts in Deep Learning Models for Medical Image Analysis
- **任务**：研究深度学习模型中的“捷径学习”现象，提出一种检测和定位模型中捷径的方法。
- **数据集**：Waterbirds、CheXpert 和 ISIC 2017 数据集，涵盖自然图像和医学图像任务。
- **方法**：结合预测深度（PD）和KL散度，定位模型中捷径特征出现的具体层，并分析捷径复杂性、深度和对模型性能的影响。实验表明，更复杂的捷径通常出现在模型的深层，而简单的捷径对性能的负面影响更大。
- **论文链接**：[There Are No Shortcuts to Anywhere Worth Going: Identifying Shortcuts in Deep Learning Models for Medical Image Analysis](https://raw.githubusercontent.com/mlresearch/v250/main/assets/boland24a/boland24a.pdf)

---

## 10. Video-CT MAE: Self-supervised Video-CT Domain Adaptation for Vertebral Fracture Diagnosis
- **任务**：提出一种结合视频预训练和自监督领域适应的方法，用于3D CT图像中的椎体骨折检测。
- **数据集**：包含27,776个未标注椎体的预训练数据集，以及457名患者的6,245个标注椎体的下游任务数据集。
- **方法**：提出Video-CT MAE方法，通过视频MAE预训练初始化，然后在未标注的椎体数据上进行自监督预训练，最后在标注数据上进行微调。该方法在椎体骨折检测任务中优于现有的CNN方法，并展示了Transformer在3D医学图像中的潜力。
- **论文链接**：[Video-CT MAE: Self-supervised Video-CT Domain Adaptation for Vertebral Fracture Diagnosis](https://raw.githubusercontent.com/mlresearch/v250/main/assets/buess24a/buess24a.pdf)

---

## 11. Evaluating ChatGPT’s Performance in Generating and Assessing Dutch Radiology Report Impressions
- **任务**：评估ChatGPT在生成和评估荷兰语放射学报告“印象”部分的能力。
- **数据集**：荷兰奈梅亨大学医学中心（Radboudumc）的胸部CT放射学报告数据集，包含200份报告，分为训练集和测试集。
- **方法**：使用OpenAI的GPT-3.5-turbo-0613模型对报告的“发现”部分进行微调，生成“印象”部分，并通过两名放射科医生和GPT-4对生成的印象进行评估，比较其与原始印象的质量差异。
- **论文链接**：[Evaluating ChatGPT’s Performance](https://raw.githubusercontent.com/mlresearch/v250/main/assets/builtjes24a/builtjes24a.pdf)

---

## 12. Predicting Age-related Macular Degeneration Progression from Retinal Optical Coherence Tomography with Intra-Subject Temporal Consistency
- **任务**：从视网膜光学相干断层扫描（OCT）图像中预测年龄相关性黄斑变性（AMD）的进展。
- **数据集**：维也纳医科大学的235只眼（3534张OCT扫描图像），包含40个转换为晚期干性AMD的病例。
- **方法**：提出一种结合AMD阶段分类器和神经常微分方程（N-ODE）的方法，通过建模疾病进展的未来轨迹，并利用同一眼的纵向扫描图像确保时间一致性，预测AMD的转换风险。
- **论文链接**：[Predicting AMD Progression](https://raw.githubusercontent.com/mlresearch/v250/main/assets/chakravarty24a/chakravarty24a.pdf)

---

## 13. Hyperparameter-Free Medical Image Synthesis for Sharing Data and Improving Site-Specific Segmentation
- **任务**：提出一种无需手动调整超参数的医学图像合成方法，用于数据共享和分割性能提升。
- **数据集**：包括盆腔MRI、肺部X光和息肉照片的三个分割任务数据集。
- **方法**：引入Hyperparameter-Free distributed learning method for automatic medical image Synthesis, Sharing, and Segmentation（HyFree-S3），结合StyleGAN2和nnU-Net，自动调整生成模型和分割模型的超参数，实现跨站点的合成数据共享和分割性能提升。
- **论文链接**：[Hyperparameter-Free Medical Image Synthesis](https://raw.githubusercontent.com/mlresearch/v250/main/assets/chebykin24a/chebykin24a.pdf)

---

## 14. Learned morphological features guide cell type assignment of deconvolved spatial transcriptomics
- **任务**：利用形态学特征指导空间转录组学中细胞类型的重新分配。
- **数据集**：包括模拟数据、合成数据和Visium数据集（使用Tangram方法）。
- **方法**：提出MHAST（Morphology-guided Hierarchical reAssignment of cell types in Spatial Transcriptomics），通过分层排列方法和自监督深度学习特征，将细胞类型重新分配到空间转录组学的每个点，提高细胞注释的准确性。
- **论文链接**：[Learned morphological features](https://raw.githubusercontent.com/mlresearch/v250/main/assets/chelebian24a/chelebian24a.pdf)

---

## 15. FedFDD: Federated Learning with Frequency Domain Decomposition for Low-Dose CT Denoising
- **任务**：在保护隐私的前提下，通过联邦学习（FL）方法对低剂量CT（LDCT）图像进行去噪。
- **数据集**：包含腹部、胸部和头部的LDCT和全剂量CT（NDCT）图像数据集。
- **方法**：提出FedFDD（Federated Learning with Frequency Domain Decomposition），通过离散余弦变换（DCT）将图像分解为高频和低频成分，并仅在FL中更新高频成分，同时保留每个客户端的低频成分，以改善LDCT去噪性能。
- **论文链接**：[FedFDD](https://raw.githubusercontent.com/mlresearch/v250/main/assets/chen24a/chen24a.pdf)

---

## 16. A Multi-Focal Image Fusion Network for Implantation Outcome Prediction of Blastocyst
- **任务**：预测囊胚移植结果，通过融合多个焦平面图像。
- **数据集**：包含643个人类胚胎的显微镜图像，分为成功植入和植入失败两类。
- **方法**：提出MFIF-Net（Multi-Focal Image Fusion Network），包含核心图像生成网络（CI-Gen）和关键特征融合网络（KFFNet），通过像素级加权融合多个焦平面图像，并提取每个焦平面的关键特征，以提高囊胚移植结果的预测性能。
- **论文链接**：[Multi-Focal Image Fusion Network](https://raw.githubusercontent.com/mlresearch/v250/main/assets/cheng24a/cheng24a.pdf)

---

## 17. Pretraining Vision-Language Model for Difference Visual Question Answering in Longitudinal Chest X-rays
- **任务**：在纵向胸部X光图像中进行差异视觉问答（diff-VQA）任务。
- **数据集**：MIMIC-CXR数据集（包含377,110张胸部X光图像和227,827份报告）和MIMIC-Diff-VQA数据集（包含700,703对纵向胸部X光图像的问答对）。
- **方法**：提出PLURAL模型，基于Transformer架构，先在自然图像和文本上进行预训练，然后在纵向胸部X光数据上进行预训练，最后在diff-VQA数据上进行微调，以提高模型在纵向图像差异问答任务中的性能。
- **论文链接**：[Pretraining Vision-Language Model](https://raw.githubusercontent.com/mlresearch/v250/main/assets/cho24a/cho24a.pdf)

---

## 18. Finite Volume Informed Graph Neural Network for Myocardial Perfusion Simulation
- **任务**：模拟心肌灌注，解决Darcy方程。
- **数据集**：合成的简化心肌形状的3D网格数据集（2000个训练样本和400个验证样本），以及从400名患者的CT图像中提取的真实心肌网格数据。
- **方法**：提出FVINN（Finite Volume Informed Graph Neural Network），将有限体积法（FVM）离散化的PDE作为“物理信息”损失函数，通过图神经网络（GNN）加速数值求解器，无需真实标签数据即可在新几何形状上进行预测。
- **论文链接**：[Finite Volume Informed Graph Neural Network](https://raw.githubusercontent.com/mlresearch/v250/main/assets/chou24a/chou24a.pdf)

---

## 19. The Multiscale Surface Vision Transformer
- **任务**：在人类皮层表面进行高分辨率的深度学习分析，用于新生儿表型预测和皮层分割。
- **数据集**：Developing Human Connectome Project（dHCP）数据集（包含580名新生儿的皮层表面网格和MRI衍生的皮层特征）；MindBoggle-101数据集（88个手动标记的成人大脑）和UK Biobank数据集（4000个大脑的FreeSurfer分割）。
- **方法**：提出MS-SiT（Multiscale Surface Vision Transformer），在局部网格窗口内应用自注意力机制，并通过移位窗口策略改善信息共享，逐步合并邻近补丁以学习层次化表示，适用于高分辨率采样和密集预测任务。
- **论文链接**：[The Multiscale Surface Vision Transformer](https://raw.githubusercontent.com/mlresearch/v250/main/assets/dahan24a/dahan24a.pdf)

---

## 20. Spatio-Temporal Encoding of Brain Dynamics with Surface Masked Autoencoders
- **任务**：开发用于人类大脑活动时空编码的深度学习模型，以提高神经科学发现的鲁棒性和泛化能力。
- **数据集**：dHCP（发育性人类连接组项目）、UKB（英国生物银行）、HCP（人类连接组项目）的fMRI数据。
- **方法**：提出表面掩码自编码器（sMAE）和视频表面掩码自编码器（vsMAE），通过自监督学习重建大脑皮层信号，增强个体表型预测和迁移学习能力。
- **论文链接**：[Spatio-Temporal Encoding of Brain Dynamics](https://raw.githubusercontent.com/mlresearch/v250/main/assets/dahan24b/dahan24b.pdf)

---

## 21. Video Polyp Segmentation using Implicit Networks
- **任务**：提高内窥镜视频中息肉分割的精度和时间一致性。
- **数据集**：SUN-SEG视频息肉分割数据集、KvasirCapsule-SEG胶囊内窥镜数据集。
- **方法**：结合隐式网络和光流损失函数，通过时空约束优化视频息肉分割，显著提升分割精度。
- **论文链接**：[Video Polyp Segmentation](https://raw.githubusercontent.com/mlresearch/v250/main/assets/dahan24c/dahan24c.pdf)

---

## 22. An unexpected confounder: how brain shape can be used to classify MRI scans?
- **任务**：评估大脑形状作为MRI扫描分类中的混杂因素的影响。
- **数据集**：IXI、HCP、MPI、kirby、IBC、OFSEP、BraTS、ADNI等T1加权MRI数据集。
- **方法**：通过两步法验证大脑形状是否为混杂因素，并利用可变形配准消除其影响，提高分类模型的解释性。
- **论文链接**：[An unexpected confounder](https://raw.githubusercontent.com/mlresearch/v250/main/assets/dauchelle24a/dauchelle24a.pdf)

---

## 23. Multi-scale Stochastic Generation of Labelled Microscopy Images for Neuron Segmentation
- **任务**：生成用于神经元追踪模型训练的多样化、高分辨率显微镜图像。
- **数据集**：果蝇神经元显微镜图像数据集。
- **方法**：提出多尺度级联的条件生成对抗网络（cGAN），结合模式寻求损失函数生成逼真的显微镜图像，提升神经元分割性能。
- **论文链接**：[Multi-scale Stochastic Generation](https://raw.githubusercontent.com/mlresearch/v250/main/assets/decroocq24a/decroocq24a.pdf)

---

## 24. Multimodal Image Registration Guided by Few Segmentations from One Modality
- **任务**：在仅有一个模态提供少量分割标注的情况下，实现多模态医学图像配准。
- **数据集**：膝关节DXA和X光图像。
- **方法**：通过数据增强、无监督领域适应和基于分割的配准，利用少量标注训练分割网络并迁移到目标模态，实现高质量的多模态配准。
- **论文链接**：[Multimodal Image Registration](https://raw.githubusercontent.com/mlresearch/v250/main/assets/demir24a/demir24a.pdf)

---

## 25. Auto-Generating Weak Labels for Real & Synthetic Data to Improve Label-Scarce Medical Image Segmentation
- **任务**：解决医学图像分割中标注稀缺问题，通过自动生成弱标签增强数据集。
- **数据集**：BUSI（乳腺超声图像）、ISIC（皮肤病变图像）、CANDID-PTX（胸部X光图像）。
- **方法**：利用少量金标准标注训练初始模型，生成粗标签并选择输入提示，通过MedSAM生成高质量弱标签，提升分割性能。
- **论文链接**：[Auto-Generating Weak Labels](https://raw.githubusercontent.com/mlresearch/v250/main/assets/deshpande24a/deshpande24a.pdf)

---

## 26. Parameter-Efficient Fine-Tuning for Medical Image Analysis: The Missed Opportunity
- **任务**：评估参数高效微调（PEFT）在医学图像分析中的有效性，特别是在低数据量场景下。
- **数据集**：包括HAMD10000、BreastUS、Fitzpatrick17K、SMDG、RSNA肺炎检测等医学图像数据集。
- **方法**：对17种PEFT算法进行基准测试，比较不同算法在CNN和Transformer架构下的性能，发现LoRA和SSF等方法在低数据量任务中表现优异。
- **论文链接**：[Parameter-Efficient Fine-Tuning](https://raw.githubusercontent.com/mlresearch/v250/main/assets/dutt24a/dutt24a.pdf)

---

## 27. Predicting DNA Content Abnormalities in Barrett’s Esophagus: A Weakly Supervised Learning Paradigm
- **任务**：预测Barrett食管中的DNA含量异常（非整倍性），辅助癌症风险评估。
- **数据集**：BEAR项目提供的H&E染色WSI数据集。
- **方法**：利用多实例学习（MIL）框架和弱监督学习，结合图像增强策略，训练深度学习模型预测DNA含量状态，显著提升预测性能。
- **论文链接**：[Predicting DNA Content Abnormalities](https://raw.githubusercontent.com/mlresearch/v250/main/assets/ercan24a/ercan24a.pdf)

---

## 28. DeCoDEx: Confounder Detector Guidance for Improved Diffusion-based Counterfactual Explanations
- **任务**：通过去偏增强基于扩散模型的反事实解释，提高模型的可解释性和泛化能力。
- **数据集**：CheXpert胸部X光图像数据集。
- **方法**：提出DeCoDEx框架，利用预训练的伪影检测器指导反事实图像生成，忽略数据中的虚假相关性，提升模型对因果病理标记的解释能力。
- **论文链接**：[DeCoDEx](https://raw.githubusercontent.com/mlresearch/v250/main/assets/fathi24a/fathi24a.pdf)

---

## 29. Improving CNN-Based Mitosis Detection through Rescanning Annotated Glass Slides and Atypical Mitosis Subtyping
- **任务**：通过重新扫描玻片和多任务学习改进CNN在有丝分裂检测中的性能。
- **数据集**：犬乳腺癌（CMC）数据集、多肿瘤WSI数据集、MIDOG22挑战数据集。
- **方法**：提出重新扫描玻片的训练范式，结合多任务学习对有丝分裂进行亚型分类，显著提升模型的鲁棒性和检测性能。
- **论文链接**：[Improving CNN-Based Mitosis Detection](https://raw.githubusercontent.com/mlresearch/v250/main/assets/fick24a/fick24a.pdf)

---

## 30. Active Learning for Efficient Medical Image Segmentation
- **任务**：使用主动学习技术减少医学图像分割任务中的标注成本，同时保持模型性能。
- **数据集**：使用医学分割十项全能（Medical Segmentation Decathlon）中的三个数据集，包括脾脏、肝脏和海马数据集，涉及CT和MRI模态。
- **方法**：提出了一种新的样本选择策略USIM，结合预测不确定性和基于次模函数的样本代表性，通过蒙特卡洛Dropout估计不确定性，并利用扩散模型生成的激活图选择多样化的样本批次。
- **论文链接**：[Active Learning for Efficient Medical Image Segmentation](https://raw.githubusercontent.com/mlresearch/v250/main/assets/fuchs24a/fuchs24a.pdf)

---

## 31. HARP: Histological Artifact Restoration Pipeline
- **任务**：开发一种无监督的组织病理学图像伪影修复流程，以提高图像质量和诊断可靠性。
- **数据集**：使用包含真实和合成伪影的组织病理学图像数据集。
- **方法**：提出HARP（Histological Artifact Restoration Pipeline），整合伪影检测、定位和修复三个步骤，使用FastFlow检测伪影，结合SAM和DBSCAN生成定位掩码，并利用条件扩散模型进行修复。
- **论文链接**：[HARP](https://raw.githubusercontent.com/mlresearch/v250/main/assets/follmer24a/follmer24a.pdf)

---

## 32. Confounder Correction in Medical Image Segmentation Quality Prediction
- **任务**：研究结构大小作为混杂因素对基于不确定性的医学图像分割质量预测的影响。
- **数据集**：使用德国国家队列研究的MRI图像数据集，包含全身MRI扫描和手动标注的解剖结构掩码。
- **方法**：提出使用偏斯皮尔曼秩相关系数来校正结构大小的影响，从而更准确地评估不确定性度量与分割质量之间的关系。
- **论文链接**：[Confounder Correction](https://raw.githubusercontent.com/mlresearch/v250/main/assets/geissler24a/geissler24a.pdf)

---

## 33. Unpaired Super-Resolution for Axial Spine MRI
- **任务**：开发一种无配对的超分辨率算法，用于提升轴向脊柱MRI图像的分辨率，以实现自动化的脊柱分割。
- **数据集**：使用包含多发性硬化症患者的轴向和矢状面T2加权MRI扫描数据集。
- **方法**：提出一种基于扩散超分辨率模型的方法，通过模拟退化函数生成合成训练对，并训练模型以提升轴向图像的z轴分辨率。
- **论文链接**：[Unpaired Super-Resolution](https://raw.githubusercontent.com/mlresearch/v250/main/assets/graf24a/graf24a.pdf)

---

## 34. Multi-Objective Learning for Deformable Image Registration
- **任务**：提出一种基于深度学习的多目标学习方法，用于可变形图像配准（DIR）。
- **数据集**：使用宫颈癌患者的盆腔MRI扫描数据集，包含手动标注的器官轮廓。
- **方法**：结合VoxelMorph网络和多目标学习框架，通过最大化超体积（HV）来优化多个冲突目标，并生成多种配准结果供临床选择。
- **论文链接**：[Multi-Objective Learning](https://raw.githubusercontent.com/mlresearch/v250/main/assets/grewal24a/grewal24a.pdf)

---

## 35. Predicting 3D Forearm Fracture Angles from Biplane X-rays
- **任务**：从双平面X光图像中预测3D前臂骨折角度。
- **数据集**：使用杜克大学健康系统的前臂X光图像数据集，包含AP和LAT视图。
- **方法**：提出一种深度学习方法，结合骨骼分割、姿态估计、2D骨折角度检测和3D重建，通过模拟退化函数生成合成数据进行训练。
- **论文链接**：[Predicting 3D Forearm Fracture Angles](https://raw.githubusercontent.com/mlresearch/v250/main/assets/gu24a/gu24a.pdf)

---

## 36. REINDIR: Accelerating Implicit Neural Representations for Deformable Image Registration
- **任务**：加速隐式神经表示（INR）在可变形图像配准中的优化过程，同时保持对域偏移的鲁棒性。
- **数据集**：使用DIR-LAB、NLST和Learn2Reg挑战赛提供的肺部CT和CBCT数据集。
- **方法**：提出REINDIR方法，通过图像编码器生成嵌入表示，并将其注入到模板INR中，以改善优化的初始化。
- **论文链接**：[REINDIR](https://raw.githubusercontent.com/mlresearch/v250/main/assets/harten24a/harten24a.pdf)

---

## 37. Neural Obfuscation for Privacy Protection in Medical Imaging
- **任务**：开发一种隐私保护方法，用于在共享医学图像时保护患者隐私。
- **数据集**：使用Kaggle RANZCR CLiP挑战赛的胸部X光图像数据集。
- **方法**：提出隐式神经混淆（Neural Obfuscation）方法，通过神经网络的隐式表示和压缩技术，对图像进行处理以减少可识别信息，同时保留图像的相关特征。
- **论文链接**：[Neural Obfuscation](https://raw.githubusercontent.com/mlresearch/v250/mainassets/heinrich24a/heinrich24a.pdf)

---

## 38. Prediction Bias in Chest X-ray Classification Models
- **任务**：研究不同数据集训练的胸部X光分类模型在图像级别上的预测倾向差异。
- **数据集**：使用CheXpert（CXP）和MIMIC-CXR（MMC）两个胸部X光数据集。
- **方法**：提出“预测倾向”概念，通过比较不同数据集训练模型的预测差异，并训练比较数据集模型（CDMs）来识别这些倾向。
- **论文链接**：[Prediction Bias](https://raw.githubusercontent.com/mlresearch/v250/main/assets/hoebel24a/hoebel24a.pdf)

---

## 39. ICL-SAM: Combining In-Context Learning and Segment Anything Model for Medical Image Segmentation
- **任务**：结合In-Context Learning（ICL）模型和Segment Anything Model（SAM），提高医学图像分割的性能。
- **数据集**：使用眼底、脑部MRI和肾脏CT图像的多个数据集。
- **方法**：提出ICL-SAM方法，通过SAM细化ICL模型的分割结果，并利用ICL模型为SAM生成提示，同时引入语义置信度图以进一步提高分割精度。
- **论文链接**：[ICL-SAM](https://raw.githubusercontent.com/mlresearch/v250/main/assets/hu24a/hu24a.pdf)

---

## 40. AttLLSTM: Recurrent Network for Thrombus Segmentation in Brain MRI
- **任务**：开发一种循环神经网络模型，用于超急性缺血性中风患者的脑MRI图像中血栓的分割。
- **数据集**：CHSF（近端闭塞）和MATAR（远端闭塞）数据集，包含188个MRI样本，涵盖DWI和SWAN模态。
- **方法**：提出AttLLSTM模型，结合交叉注意力模块将DWI和SWAN模态融合，并通过改进的卷积长短期记忆网络（LLSTM）进行血栓分割，最后通过病变分割和后处理模块减少假阳性预测。
- **论文链接**：[AttLLSTM](https://raw.githubusercontent.com/mlresearch/v250/main/assets/ibarra24a/ibarra24a.pdf)

---

## 41. Uncertainty-aware Retinal Layer Segmentation in OCT
- **任务**：提出一种不确定性感知的视网膜层分割方法，用于光学相干断层扫描（OCT）图像。
- **数据集**：内部数据集（AMD和正常参与者）和外部验证数据集（Rotterdam Study），包含458个B扫描。
- **方法**：基于符号距离函数（SDF）和高斯分布的概率建模，通过深度对比学习优化模型，以提高视网膜层分割的准确性和鲁棒性。
- **论文链接**：[Uncertainty-aware Retinal Layer Segmentation](https://raw.githubusercontent.com/mlresearch/v250/main/assets/islam24a/islam24a.pdf)

---

## 42. Reducing Uncertainty in 3D Medical Image Segmentation under Limited Annotations
- **任务**：减少在有限标注数据下3D医学图像分割中的不确定性。
- **数据集**：左心房（LA）和胰腺（Pancreas）数据集，包含MRI和CT体积。
- **方法**：提出一种半监督对比学习方法，通过两个子网络（不确定性预测网络和不确定性感知描述符网络）纠正错误预测，并通过深度对比学习优化模型。
- **论文链接**：[Reducing Uncertainty](https://raw.githubusercontent.com/mlresearch/v250/main/assets/jarimijafarbigloo24a/jarimijafarbigloo24a.pdf)

---

## 43. Edge-Guided Single-Source Domain Generalization for Medical Image Segmentation
- **任务**：开发一种单源领域泛化方法，用于医学图像分割，以实现“一次训练，随处部署”。
- **数据集**：BraTS’19（脑肿瘤分割）、前列腺数据集（多中心MRI）和MMWHS（心脏结构分割）。
- **方法**：提出边缘引导的单源领域泛化（EGSDG）方法，通过引入图像边缘信息作为输入，并结合Bézier曲线数据增强，提高模型在未知目标域上的泛化能力。
- **论文链接**：[Edge-Guided Single-Source Domain Generalization](https://raw.githubusercontent.com/mlresearch/v250/main/assets/jiang24b/jiang24b.pdf)

---

## 44. Self-supervised Pretraining in the Wild for Medical Image Transformers
- **任务**：比较自监督预训练（SSL）在自然图像数据集（wild-pretraining）和任务相关数据集（self-pretraining）对医学图像分割的影响。
- **数据集**：包含10,412个3D CT扫描的公共数据集，以及用于微调的NSCLC患者数据集。
- **方法**：使用Swin Transformer和Vision Transformer（ViT）进行实验，通过对比学习、掩码图像预测等任务进行预训练，并评估模型在不同成像条件下的鲁棒性和微调效率。
- **论文链接**：[Self-supervised Pretraining](https://raw.githubusercontent.com/mlresearch/v250/main/assets/jiang24a/jiang24a.pdf)

---

## 45. Comparing Radiation Oncologists and Deep Learning Dose Predictors
- **任务**：比较放射肿瘤学家与深度学习剂量预测模型在评估分割变化对剂量学影响方面的表现。
- **数据集**：包含100名胶质母细胞瘤患者的MRI和CT图像，以及用于测试的54个分割变体。
- **方法**：训练一个级联3D U-Net剂量预测模型，通过计算分割变化对OARs剂量的影响，评估其在剂量学评估中的准确性和效率。
- **论文链接**：[Comparing Radiation Oncologists and Deep Learning Dose Predictors](https://raw.githubusercontent.com/mlresearch/v250/main/assets/kamath24a/kamath24a.pdf)

---

## 46. Efficiently Correcting Patch-based Segmentation Errors in Retinal Images
- **任务**：提出一种结合质量控制和错误校正的框架，用于视网膜图像的血管分割任务，以控制每张图像的分割质量。
- **数据集**：FIVES数据集，包含800张眼底图像，涵盖健康个体和患有AMD、DR、青光眼的患者。
- **方法**：通过不确定性图选择局部补丁进行人工审核，并使用DSC估计器预测校正后的分割质量，以最小化人工审核工作量。
- **论文链接**：[Efficiently Correcting Patch-based Segmentation Errors](https://raw.githubusercontent.com/mlresearch/v250/main/assets/konstantin24a/konstantin24a.pdf)

---

## 47. ASMR: Angular Support for Malfunctioning Client Resilience in Federated Learning
- **任务**：提出一种新的联邦学习方法，用于动态排除故障客户端，提高全局模型的鲁棒性。
- **数据集**：CRC（结直肠癌）数据集，包含100,000张病理图像。
- **方法**：基于“角度客户端支持”概念，通过计算客户端更新之间的余弦距离，动态排除故障客户端，无需知道故障客户端数量。
- **论文链接**：[ASMR](https://raw.githubusercontent.com/mlresearch/v250/main/assets/krusen24a/krusen24a.pdf)

---

## 48. Real-time MR-based 3D Motion Monitoring using Raw k-space Data
- **任务**：开发一种基于原始k空间数据的实时3D运动监测方法，用于磁共振引导的放疗。
- **数据集**：4D XCAT幻影生成的腹部MRI数据，模拟呼吸和心脏运动。
- **方法**：提出一种基于RNN的架构，直接从k空间线估计目标运动，通过Kooshball轨迹采样k空间，并使用简单的移动平均滤波器平滑输出。
- **论文链接**：[Real-time MR-based 3D Motion Monitoring](https://raw.githubusercontent.com/mlresearch/v250/main/assets/kuipers24a/kuipers24a.pdf)

---

## 49. Conditional Set-Diffusion for Cerebral Vessel Tree Generation
- **任务**：提出一种基于条件集扩散的生成模型，用于生成急性缺血性中风患者的脑血管树。
- **数据集**：MR CLEAN Registry数据集，包含110名M1动脉闭塞患者的MRI图像。
- **方法**：使用条件集扩散模型生成血管树中心线，并通过后处理算法对生成的无序中心线进行排序和清理，以用于下游任务。
- **论文链接**：[Conditional Set-Diffusion](https://raw.githubusercontent.com/mlresearch/v250/main/assets/kulkarni24a/kulkarni24a.pdf)

---

## 50. Hidden Adversarial Bias Attacks on Vulnerable Patient Populations
- **任务**：研究如何通过数据中毒攻击在医学影像中注入不可检测的偏见，导致模型对特定脆弱人群产生误诊。
- **数据集**：RSNA肺炎检测挑战赛数据集（胸部X光）、CheXpert和MIMIC-CXR-JPG数据集。
- **方法**：通过在训练数据中注入针对特定人群的标签噪声（即降低肺炎标签的置信度），训练深度学习模型以引入误诊偏见。研究发现，这种攻击可以在不降低整体模型性能的情况下，有针对性地降低特定人群的模型性能，并且这种偏见可以传播到外部数据集。
- **论文链接**：[Hidden Adversarial Bias Attacks](https://raw.githubusercontent.com/mlresearch/v250/main/assets/kulkarni24b/kulkarni24b.pdf)

---

## 51. Registration Quality Evaluation Metric with Self-Supervised Siamese Networks
- **任务**：开发一种新的医学图像配准质量评估指标，以解决传统方法的局限性。
- **数据集**：Nissl染色小鼠脑组织切片数据集、IXI数据集（人类大脑MRI）。
- **方法**：提出了一种基于自监督学习的Siamese网络（SiamRegQC），通过学习图像对的语义相似性来评估配准质量。该方法使用余弦相似性作为评估指标，并通过对比学习损失函数优化网络，以提高对小误差的敏感性和对局部最小值的鲁棒性。
- **论文链接**：[Registration Quality Evaluation Metric](https://raw.githubusercontent.com/mlresearch/v250/main/assets/kohler24a/kohler24a.pdf)

---

## 52. Multi-Source StyleGAN for Heterogeneous Medical Data Integration
- **任务**：解决医学数据稀缺和异构性问题，通过多源数据生成高质量的医学图像。
- **数据集**：手写数字图像（MorphoMNIST）、视网膜眼底图像（M2CAI）、大脑MRI图像（UKB和ADNI）。
- **方法**：提出了一种多源StyleGAN（MSSG），通过联合学习多个数据源的潜在空间，生成控制所有潜在因素的新图像。该方法通过建模不同数据源之间的条件分布，实现从不同数据源中学习并生成高质量图像。
- **论文链接**：[Multi-Source StyleGAN](https://raw.githubusercontent.com/mlresearch/v250/main/assets/lai24a/lai24a.pdf)

---

## 53. Triplet Training for Dementia Diagnosis with Limited Data
- **任务**：在有限数据的情况下，提高痴呆症差异诊断的性能。
- **数据集**：UK Biobank、ADNI和NIFD（用于阿尔茨海默病和额颞叶痴呆的数据集）。
- **方法**：提出了一种“Triplet Training”方法，结合自监督预训练（Barlow Twins）、自蒸馏和目标数据集的微调，通过逐步优化模型，显著提高了在有限数据情况下的诊断性能。
- **论文链接**：[Triplet Training](https://raw.githubusercontent.com/mlresearch/v250/main/assets/li24a/li24a.pdf)

---

## 54. Detecting Brain Anomalies with β-VAE in Clinical Routine
- **任务**：在临床实践中检测脑部异常（如与年龄相关的白质高信号）。
- **数据集**：UK Biobank（健康队列）、巴黎临床数据仓库（CDW，包含多个医院的FLAIR MRI）。
- **方法**：使用β-VAE在健康队列上预训练，并在CDW中微调，通过比较重建图像和真实图像的差异来检测异常。研究发现，模型能够检测到与Fazekas评分相关的病变体积，但在图像质量较差时可能失败。
- **论文链接**：[Detecting Brain Anomalies](https://raw.githubusercontent.com/mlresearch/v250/main/assets/loizillon24a/loizillon24a.pdf)

---

## 55. SepVAE: Contrastive VAE to Separate Pathological Patterns from Healthy Ones
- **任务**：从健康人群中分离病理模式。
- **数据集**：包括健康对照组和患有精神分裂症或自闭症的患者的结构化MRI数据。
- **方法**：提出了一种对比分析变分自编码器（SepVAE），通过引入解耦项和分类项，优化了潜在空间的分离，使得病理特征和常见特征能够被更好地分离。实验表明，该方法在多个医学应用中优于现有方法。
- **论文链接**：[SepVAE](https://raw.githubusercontent.com/mlresearch/v250/main/assets/louiset24a/louiset24a.pdf)

---

## 56. Efficient Anatomy Segmentation in Laparoscopic Surgery using Multi-Teacher Knowledge Distillation
- **任务**：提高腹腔镜手术中解剖结构分割的效率和准确性。
- **数据集**：Dresden Surgical Anatomy Dataset（包含多种解剖结构的腹腔镜图像）。
- **方法**：提出了一种多教师知识蒸馏（MT-KD）方法，通过多个高精度的解剖特定教师网络指导一个高效的学生网络，显著提高了小规模网络的分割性能，同时保持了实时性。
- **论文链接**：[Efficient Anatomy Segmentation](https://raw.githubusercontent.com/mlresearch/v250/main/assets/maack24a/maack24a.pdf)

---

## 57. Automated Ranking of Chest X-ray Radiological Findings Severity
- **任务**：在只有二元标签的情况下，从胸部X光中自动评估异常发现的严重程度。
- **数据集**：包含190万张胸部X光的专有数据集，以及手动标注的测试集。
- **方法**：通过分析二元分类器的原始输出与放射科医生对严重程度的排名之间的相关性，研究了在没有直接严重程度标签的情况下，模型是否能够隐式捕获异常严重程度信息。此外，通过结合少量完全监督的排名数据和大量二元标签数据，进一步提高了模型性能。
- **论文链接**：[Automated Ranking](https://raw.githubusercontent.com/mlresearch/v250/main/assets/macpherson24a/macpherson24a.pdf)

---

## 58. Training-free Prompt Placement for SAM Predictions in 3D Bone CT Scans
- **任务**：减少Segment Anything Model（SAM）在3D骨CT扫描中应用时所需的用户交互。
- **数据集**：包含肩关节、膝关节和髋关节CT扫描的内部数据集和公开数据集。
- **方法**：提出了一种无需训练的提示放置方法，通过从单个初始框提示开始，利用相邻切片的预测信息传播新的框提示，显著减少了所需的用户交互和标注像素数量。
- **论文链接**：[Training-free Prompt Placement](https://raw.githubusercontent.com/mlresearch/v250/main/assets/magg24a/magg24a.pdf)

---

## 59. Laparoflow-SSL: Image Analysis from a Tiny Dataset through Self-Supervised Transformers
- **任务**：利用少量标注数据和大量未标注的腹腔镜手术视频，进行图像分析。
- **数据集**：M2CAI 2016挑战赛数据集（腹腔镜视频）、RARP-45数据集（机器人手术视频）、CholecSeg8k数据集（胆囊切除术的语义分割）。
- **方法**：提出了一种基于自监督学习的Laparoflow-SSL方法，通过光流引导的像素级对比学习损失函数，训练了一个强大的表示骨干网络。实验表明，即使在只有少量标注数据的情况下，基于该骨干网络的下游任务模型也能取得与现有方法相当的性能。
- **论文链接**：[Laparoflow-SSL](https://raw.githubusercontent.com/mlresearch/v250/main/assets/moens24a/moens24a.pdf)

---

## 60. IHCScoreGAN: Unsupervised Deep Learning Framework for Breast Cancer Ki67 Scoring
- **任务**：开发无监督深度学习框架IHCScoreGAN，用于乳腺癌Ki67评分的自动化和端到端分析。
- **数据集**：Mayo Clinic的2,126张Ki67染色切片图像，以及未配对的公共H&E染色图像数据集用于合成掩码生成。
- **方法**：提出一种基于生成对抗网络（GAN）的框架，通过域转移策略将Ki67图像转换为合成细胞分割掩码，同时预测细胞中心点和生物标志物表达，实现无需标注数据的Ki67评分。
- **论文链接**：[IHCScoreGAN](https://raw.githubusercontent.com/mlresearch/v250/main/assets/molnar24a/molnar24a.pdf)

---

## 61. RADR: Robust Domain Adversarial Framework for Diabetic Retinopathy Classification
- **任务**：开发一种鲁棒的域对抗框架RADR，用于糖尿病视网膜病变（DR）严重程度的自动化分类。
- **数据集**：EyePACS数据集（成人眼底图像）和多个外部数据集（Messidor、APTOS等）。
- **方法**：结合域对抗训练和数据增强策略，通过多相机训练和伪标签生成，提高模型在未见数据集上的泛化能力。
- **论文链接**：[RADR](https://raw.githubusercontent.com/mlresearch/v250/main/assets/monedero24a/monedero24a.pdf)

---

## 62. ADAPT: Multimodal Learning Framework for Detecting Physiological Changes with Missing Modalities
- **任务**：开发一种多模态学习框架ADAPT，用于在缺失模态数据的情况下检测生理变化。
- **数据集**：StressID（压力检测）和LOC（飞行员意识丧失检测）数据集，包含视频、音频和生物医学信号。
- **方法**：通过模态对齐和掩码多模态Transformer，将所有模态对齐到锚点模态空间，并处理缺失模态，提高模型的鲁棒性。
- **论文链接**：[ADAPT](https://raw.githubusercontent.com/mlresearch/v250/main/assets/mordacq24a/mordacq24a.pdf)

---

## 63. Noisy Student for OCT Segmentation
- **任务**：提出一种基于Noisy Student框架的半监督学习方法，用于视网膜OCT图像中视神经盘和视神经杯的分割。
- **数据集**：DRISHTI、REFUGE、RIGA（成人眼底图像）和AIROGS（未标记图像）。
- **方法**：通过教师模型生成伪标签，训练学生模型，结合数据增强策略，提高模型在新领域的泛化能力。
- **论文链接**：[Noisy Student for OCT Segmentation](https://raw.githubusercontent.com/mlresearch/v250/main/assets/moris24a/moris24a.pdf)

---

## 64. Unsupervised Domain Adaptation for MRI Skull Stripping
- **任务**：开发一种无监督域适应方法，用于将成人脑部MRI的颅骨剥离模型迁移到新生儿数据上。
- **数据集**：Calgary-Campinas（成人脑部MRI）、GMM合成数据集和新生儿MRI数据集。
- **方法**：结合域对抗模型和GMM生成的合成数据，通过数据增强策略，训练模型以适应新生儿MRI数据。
- **论文链接**：[Unsupervised Domain Adaptation](https://raw.githubusercontent.com/mlresearch/v250/main/assets/omidi24a/omidi24a.pdf)

---

## 65. Resolution and Field of View Invariant Generative Modelling
- **任务**：提出一种基于潜在扩散模型（LDM）的生成建模方法，用于在不同分辨率和视野条件下生成全身CT图像。
- **数据集**：AutoPET数据集（全身CT扫描）。
- **方法**：通过空间条件机制控制样本几何属性，结合数据增强策略，实现多分辨率和多视野的图像生成。
- **论文链接**：[Resolution and Field of View Invariant Generative Modelling](https://raw.githubusercontent.com/mlresearch/v250/main/assets/patel24a/patel24a.pdf)

---

## 66. Unsupervised Deep Learning Method for MRI Bias Correction
- **任务**：开发一种无监督深度学习方法UBC，用于MRI图像的偏置场校正。
- **数据集**：OASIS和IXI（T1加权MRI图像）。
- **方法**：通过最小化基于图像熵和偏置场导数的成本函数，训练网络以估计偏置校正后的图像。
- **论文链接**：[Unsupervised Deep Learning Method](https://raw.githubusercontent.com/mlresearch/v250/main/assets/perez-caballero24a/perez-caballero24a.pdf)

---

## 67. Annotation-Efficient Strategy for Segmentation of 3D Body Composition
- **任务**：提出一种高效的标注策略，用于3D全身成分分析的医学图像分割。
- **数据集**：Mayo Clinic的CT扫描数据集（腹部和盆腔区域）。
- **方法**：通过迭代自学习方法和稀疏标注，结合2D和3D神经网络，减少手动标注需求，提高分割精度。
- **论文链接**：[Annotation-Efficient Strategy](https://raw.githubusercontent.com/mlresearch/v250/main/assets/philipp24a/philipp24a.pdf)

---

## 68. Cell-DETR: Efficient Cell Detection and Classification for Whole Slide Images
- **任务**：开发一种高效的细胞检测和分类方法Cell-DETR，用于全切片图像（WSIs）分析。
- **数据集**：PanNuke、CoNSeP和Camelyon16（细胞分割和分类）。
- **方法**：基于检测变换器（DETR）模型，结合窗口检测流程和数据增强策略，实现大规模病理图像的高效细胞检测和分类。
- **论文链接**：[Cell-DETR](https://raw.githubusercontent.com/mlresearch/v250/main/assets/pina24a/pina24a.pdf)

---

## 69. Exploring Transfer Learning in Medical Image Segmentation using Vision-Language Models
- **任务**：探索视觉-语言模型（VLMs）在医学图像分割中的迁移学习能力。
- **数据集**：11个2D医学图像数据集（包括内窥镜、皮肤、超声和X光图像）。
- **方法**：通过微调CLIP和BiomedCLIP模型，结合自动化生成的语言提示，评估VLMs在医学图像分割中的性能和鲁棒性。
- **论文链接**：[Exploring Transfer Learning](https://raw.githubusercontent.com/mlresearch/v250/main/assets/poudel24a/poudel24a.pdf)

---

## 70. NcIEMIL: Rethinking Decoupled Multiple Instance Learning Framework for Histopathological Slide Classification
- **任务**：病理切片的多实例学习（MIL）分类，减少信息冗余，提高分类性能。
- **数据集**：CAMELYON16乳腺癌数据集（270张训练用WSI，129张测试用WSI）和BgIM胃黏膜活检数据集（220个样本，4个等级的肠上皮化生）。
- **方法**：提出NcIEMIL框架，通过弱监督训练的特征提取器、判别性实例选择和混合注意力聚合器，减少信息冗余并优化实例选择。
- **论文链接**：[NcIEMIL](https://raw.githubusercontent.com/mlresearch/v250/main/assets/qiehe24a/qiehe24a.pdf)

---

## 71. Slide-SAM: Medical SAM Meets Sliding Window
- **任务**：3D医学图像分割，解决Segment Anything Model（SAM）在处理3D图像时的上下文关系问题。
- **数据集**：多个公共和私有的医学图像数据集，包括AbdomenCT-1K、TotalSegmentor、CTPelvic1K、WORD等。
- **方法**：提出Slide-SAM模型，通过滑动窗口方法处理相邻切片，并结合混合损失函数，利用SAM的预训练权重进行3D分割。
- **论文链接**：[Slide-SAM](https://raw.githubusercontent.com/mlresearch/v250/main/assets/quan24a/quan24a.pdf)

---

## 72. UltraMAE: Multi-modal Masked Autoencoder for Ultrasound Pre-training
- **任务**：超声图像和视频的无监督预训练，提高超声相关下游任务的性能。
- **数据集**：超过100,000个超声图像和视频，涵盖多种人体部位（如肝脏、骨骼、心脏等）。
- **方法**：提出UltraMAE模型，结合掩码自编码器（MAE）和置信度加权超声图像（CWUS），通过置信度图增强高置信度区域，减少噪声和阴影伪影。
- **论文链接**：[UltraMAE](https://raw.githubusercontent.com/mlresearch/v250/main/assets/rahman24a/rahman24a.pdf)

---

## 73. UnCLe SAM: Unleashing SAM’s Potential for Continual Prostate MRI Segmentation
- **任务**：连续学习（CL）在前列腺MRI分割中的应用，解决医学图像分割中的领域适应性问题。
- **数据集**：四个前列腺MRI数据集（UCL、I2CVB、ISBI、DecathProst）。
- **方法**：提出UnCLe SAM框架，通过持续更新提示（prompt）并利用SAM的预训练知识库，适应动态环境中的数据变化。
- **论文链接**：[UnCLe SAM](https://raw.githubusercontent.com/mlresearch/v250/main/assets/ranem24a/ranem24a.pdf)

---

## 74. Ano-swinMAE: Unsupervised Anomaly Detection in Brain MRI using Swin Transformer-based Masked Auto Encoder
- **任务**：脑部MRI中的无监督异常检测，通过掩码自编码器（MAE）检测病理区域。
- **数据集**：BraTS（胶质瘤）、MSLUB（多发性硬化症）、WMH（白质高信号）和IXI（健康大脑）。
- **方法**：提出Ano-swinMAE模型，结合Swin Transformer和掩码策略，通过重建掩码区域检测潜在病理位置。
- **论文链接**：[Ano-swinMAE](https://raw.githubusercontent.com/mlresearch/v250/main/assets/rashmi24a/rashmi24a.pdf)

---

## 75. Deep Blind Arterial Input Function: Signal Correction in Perfusion Cardiac Magnetic Resonance
- **任务**：校正心脏磁共振灌注成像中的动脉输入函数（AIF）信号。
- **数据集**：43名患者的临床数据集，使用双饱和序列进行评估。
- **方法**：提出基于CNN的深度学习方法，通过模拟数据库训练网络，校正AIF的饱和效应。
- **论文链接**：[Deep Blind Arterial Input Function](https://raw.githubusercontent.com/mlresearch/v250/main/assets/rebbah24a/rebbah24a.pdf)

---

## 76. Re-DiffiNet: Modeling Discrepancies Loss in Tumor Segmentation using Diffusion Models
- **任务**：脑肿瘤分割，通过扩散模型改进U-Net的分割结果。
- **数据集**：BraTS2023数据集（1251个脑MRI扫描）。
- **方法**：提出Re-DiffiNet框架，通过显式建模分割模型输出与真实标签之间的差异，利用扩散模型捕捉高频信息，提高边界定位能力。
- **论文链接**：[Re-DiffiNet](https://raw.githubusercontent.com/mlresearch/v250/main/assets/ren24a/ren24a.pdf)

---

## 77. Parameter-Efficient Generation of Natural Language Explanations for Chest X-ray Classification
- **任务**：为胸部X光分类生成自然语言解释（NLE），减少训练参数数量。
- **数据集**：MIMIC-NLE数据集（38003张图像和NLE对）。
- **方法**：提出基于编码器-解码器架构的NLE生成方法，结合参数高效微调（PEFT）技术，减少训练参数，同时保持性能。
- **论文链接**：[Parameter-Efficient Generation](https://raw.githubusercontent.com/mlresearch/v250/main/assets/rio-torto24a/rio-torto24a.pdf)

---

## 78. Improving Identically Distributed and Out-of-Distribution Medical Image Classification with Segmentation-Guided Attention
- **任务**：医学图像分类，特别是在小数据集场景下提高模型的泛化能力。
- **数据集**：五个儿科医院的肾脏超声数据集（包括SickKids、Stanford、UIowa、CHOP）。
- **方法**：提出分割掩码引导的注意力机制，通过注意力损失函数引导模型关注重要区域，提高模型在同分布和分布外数据上的性能。
- **论文链接**：[Improving Identically Distributed](https://raw.githubusercontent.com/mlresearch/v250/main/assets/rizhko24a/rizhko24a.pdf)

---

## 79. Anomaly-focused Single Image Super-resolution with Artifact Removal for Chest X-rays
- **任务**：胸部X光图像的单图像超分辨率（SISR），同时去除伪影。
- **数据集**：VinBig数据集（18,000张图像）和NIH Chest x-ray14数据集（112,120张图像）。
- **方法**：提出基于扩散模型的SISR方法，结合变分自编码器机制和异常引导训练，去除伪影并强调异常区域的重建。
- **论文链接**：[Anomaly-focused Single Image Super-resolution](https://raw.githubusercontent.com/mlresearch/v250/main/assets/roy24a/roy24a.pdf)

---

## 80. MultiMedEval: Evaluating Medical Visual-Language Models in Multi-modal Tasks
- **任务**：评估医学视觉语言模型（VLM）在多模态任务中的性能，包括图像分类、问答（QA）、视觉问答（VQA）、报告总结、报告生成和自然语言推理（NLI）。
- **数据集**：23个数据集，涵盖11个医学领域，如MIMIC-CXR、Pad-UFES、VinDr Mammo等。
- **方法**：提出MultiMedEval工具包，一个开源的Python框架，用于简化VLM的评估流程。通过统一的基准测试和标准化的评估指标，为医学VLM提供公平的性能比较。
- **论文链接**：[MultiMedEval](https://raw.githubusercontent.com/mlresearch/v250/main/assets/royer24a/royer24a.pdf)

---

## 81. Diffusion X-ray Image Denoising
- **任务**：开发一种基于扩散模型的X射线图像去噪方法，以减少辐射剂量并提高图像质量。
- **数据集**：NIH胸部X射线数据库，包含高剂量和低剂量的X射线图像。
- **方法**：提出DDPM-X，一种基于扩散模型的去噪方法，通过模拟高斯噪声的生成过程来训练模型，并应用于去除X射线图像中的泊松噪声。
- **论文链接**：[Diffusion X-ray Image Denoising](https://raw.githubusercontent.com/mlresearch/v250/main/assets/sanderson24a/sanderson24a.pdf)

---

## 82. Imbalance-aware Loss Functions Improve Medical Image Classification
- **任务**：解决医学图像分类中类别不平衡问题，提高少数类的分类性能。
- **数据集**：Glioma数据集（3D MRI图像）和Glaucoma数据集（2D眼底照片）。
- **方法**：提出基于MCC和F1分数的可微分损失函数，并将其与交叉熵损失结合，以提高模型对少数类的识别能力。
- **论文链接**：[Imbalance-aware Loss Functions](https://raw.githubusercontent.com/mlresearch/v250/main/assets/scholz24a/scholz24a.pdf)

---

## 83. A Patch-based Student-Teacher Pyramid Matching Approach to Anomaly Detection in 3D MRI
- **任务**：开发一种用于3D MRI异常检测的顶向下方法。
- **数据集**：BraTS 2021肿瘤数据集和IXI健康MRI数据集。
- **方法**：提出基于学生-教师特征金字塔匹配（STFPM）的异常检测方法，结合3D补丁自监督预训练和ACS卷积，提升异常检测性能。
- **论文链接**：[A Patch-based Student-Teacher Pyramid Matching Approach](https://raw.githubusercontent.com/mlresearch/v250/main/assets/schwarz24a/schwarz24a.pdf)

---

## 84. Dense Self-Supervised Learning for Medical Image Segmentation
- **任务**：减少医学图像分割中手动标注的负担，通过自监督学习提高分割性能。
- **数据集**：ACDC（心脏MRI分割）。
- **方法**：提出Pix2Rep，一种像素级对比学习方法，通过自监督预训练生成强大的像素级表示，用于少样本和全监督分割任务。
- **论文链接**：[Dense Self-Supervised Learning](https://raw.githubusercontent.com/mlresearch/v250/main/assets/seince24a/seince24a.pdf)

---

## 85. Zero-Shot Medical Image Segmentation Based on Sparse Prompt Using Finetuned SAM
- **任务**：在无需大量标注数据的情况下，实现医学图像的零样本分割。
- **数据集**：AMOS22（腹部CT器官分割）、MoNuSeg（显微镜图像分割）和GlaS（腺体分割）。
- **方法**：提出基于SAM模型的两阶段零样本分割方法，通过稀疏提示和测试时微调，实现对医学图像的快速分割。
- **论文链接**：[Zero-Shot Medical Image Segmentation](https://raw.githubusercontent.com/mlresearch/v250/main/assets/shaharabany24a/shaharabany24a.pdf)

---

## 86. Lupus Nephritis Subtype Classification with only Slide Level Labels
- **任务**：仅使用幻灯片级别标签进行狼疮性肾炎亚型分类。
- **数据集**：包含多染色WSI的LN数据集。
- **方法**：提出LupusNet，一种基于MIL的深度学习模型，通过结合门控注意力和多头注意力，提高LN亚型分类性能。
- **论文链接**：[Lupus Nephritis Subtype Classification](https://raw.githubusercontent.com/mlresearch/v250/main/assets/sharma24a/sharma24a.pdf)

---

## 87. Med-Tuning: A New Parameter-Efficient Tuning Framework for Medical Volumetric Segmentation
- **任务**：开发一种参数高效的微调框架，用于医学体积分割任务。
- **数据集**：KiTS 2019（肾脏肿瘤分割）、BraTS 2019和BraTS 2020（脑肿瘤分割）。
- **方法**：提出Med-Tuning框架和Med-Adapter模块，通过多尺度特征提取和体积相关性建模，提高预训练模型在医学体积分割任务上的性能。
- **论文链接**：[Med-Tuning](https://raw.githubusercontent.com/mlresearch/v250/main/assets/shen24a/shen24a.pdf)

---

## 88. ThickV-Stain: Unprocessed Thick Tissues Virtual Staining for Rapid Intraoperative Histology
- **任务**：开发一种用于厚组织样本的虚拟染色方法，以加速术中组织学检查。
- **数据集**：包含肺腺癌亚型的厚组织样本数据集。
- **方法**：提出ThickV-Stain模型，通过多尺度生成器和判别器，实现从低质量输入图像到虚拟H&E染色图像的转换。
- **论文链接**：[ThickV-Stain](https://raw.githubusercontent.com/mlresearch/v250/main/assets/shi24a/shi24a.pdf)

---

## 89. Advancing Multiplex Immunofluorescence Imaging Cell Detection using Semi-Supervised Learning with Pseudo-Labeling
- **任务**：在多标记免疫荧光图像中检测细胞，解决标注数据有限的问题。
- **数据集**：乳头状尿路上皮癌的mIF图像数据集，包含部分标注的单细胞数据。
- **方法**：提出半监督学习方法，通过伪标签生成和迭代训练，提高细胞检测模型的性能和泛化能力。
- **论文链接**：[Advancing Multiplex Immunofluorescence Imaging](https://raw.githubusercontent.com/mlresearch/v250/main/assets/shokrollahi24a/shokrollahi24a.pdf)

---

## 90. SINR: Spline-enhanced Implicit Neural Representation for Multi-modal Registration
- **任务**：多模态医学图像配准。
- **数据集**：CamCAN数据集（3D单模态和多模态脑部MRI图像）。
- **方法**：提出SINR（Spline-enhanced INR），通过结合隐式神经表示（INR）和自由形变（FFD）来参数化连续变形场。利用B样条FFD的平滑性和控制点稀疏性优化INR的采样效率和变换正则性，同时减少空间折叠现象。
- **论文链接**：[SINR](https://raw.githubusercontent.com/mlresearch/v250/main/assets/sideri-lampretsa24a/sideri-lampretsa24a.pdf)

---

## 91. [Citation needed] Data usage and citation practices in medical imaging conferences
- **任务**：分析医学成像会议中数据集的使用和引用实践。
- **数据集**：20个公开医学数据集，包括MICCAI和MIDL会议论文中使用的数据集。
- **方法**：开发基于OpenAlex的引用分析工具和PDF注释软件，检测数据集的使用情况，并分析2013年至2023年的论文数据。
- **论文链接**：[[Citation needed]](https://raw.githubusercontent.com/mlresearch/v250/main/assets/sourget24a/sourget24a.pdf)

---

## 92. Analysis of Transformers for Medical Image Retrieval
- **任务**：医学图像检索。
- **数据集**：ISIC 2017（皮肤病变图像）、COVID-19胸部X光和Kvasir（内窥镜图像）。
- **方法**：提出基于对比学习的变换器模型，分析不同变换器架构和参数设置，并评估Transformer Input Sampling等解释性技术。
- **论文链接**：[Analysis of Transformers](https://raw.githubusercontent.com/mlresearch/v250/main/assets/susmitha24a/susmitha24a.pdf)

---

## 93. Nuclei Segmentation in Histopathological Images with Enhanced U-Net3+
- **任务**：组织病理学图像中的细胞核分割。
- **数据集**：MoNuSeg 2018、CPM-17和CoNSEP（3D H&E染色组织切片图像）。
- **方法**：提出增强型U-Net3+模型，通过自适应特征选择、最大模糊池化、DropBlock正则化和引导滤波块优化细胞核结构的细节分割。
- **论文链接**：[Nuclei Segmentation](https://raw.githubusercontent.com/mlresearch/v250/main/assets/swain24a/swain24a.pdf)

---

## 94. Weakly supervised deep learning model with size constraint for prostate cancer detection in multiparametric MRI and generalization to unseen domains
- **任务**：多参数MRI中的前列腺癌检测。
- **数据集**：PI-CAI、Prostate158和私有数据库（前列腺MRI图像）。
- **方法**：提出弱监督学习方法，通过尺寸约束损失函数从弱标注（圆形涂鸦）中学习前列腺癌病变的分割，并通过集成多个训练模型的预测提高泛化性能。
- **论文链接**：[Weakly supervised deep learning model](https://raw.githubusercontent.com/mlresearch/v250/main/assets/trombetta24a/trombetta24a.pdf)

---

## 95. Disruptive Autoencoders: Leveraging Low-level features for 3D Medical Image Pre-training
- **任务**：3D医学图像预训练。
- **数据集**：BraTS21、LUNA16、TCIA Covid19、HNSCC、TCIA Colon和LiDC（CT和MRI图像）。
- **方法**：提出Disruptive Autoencoders（DAE），通过局部掩码、添加噪声和下采样等低级扰动训练自编码器，学习医学图像的局部特征表示。
- **论文链接**：[Disruptive Autoencoders](https://raw.githubusercontent.com/mlresearch/v250/main/assets/valanarasu24a/valanarasu24a.pdf)

---

## 96. VariViT: A Vision Transformer for Variable Image Sizes
- **任务**：医学图像分类（胶质瘤基因型预测和脑肿瘤分类）。
- **数据集**：Glioma和Brain Tumor数据集（3D脑部MRI图像）。
- **方法**：提出VariViT，通过中心选择法调整位置嵌入，并采用新的批量策略，使Vision Transformer能够处理可变图像大小。
- **论文链接**：[VariViT](https://raw.githubusercontent.com/mlresearch/v250/main/assets/varma24a/varma24a.pdf)

---

## 97. Shape of my heart: Cardiac models through learned signed distance functions
- **任务**：基于心脏MRI的心脏建模。
- **数据集**：公开的左/右心室内外膜3D形状库（共4种形状，包括健康和心力衰竭患者）。
- **方法**：提出基于深度有符号距离函数（DeepSDF）的心脏建模方法，通过Lipschitz正则化网络学习心脏形状，并从稀疏点云或不同模态数据中重建解剖模型。
- **论文链接**：[Shape of my heart](https://raw.githubusercontent.com/mlresearch/v250/main/assets/verhulsdonk24a/verhulsdonk24a.pdf)

---

## 98. Accelerating physics-informed neural fields for fast CT perfusion analysis in acute ischemic stroke
- **任务**：急性缺血性中风的CT灌注分析。
- **数据集**：CLEOPATRA研究中的CT灌注图像和MRI参考标准。
- **方法**：提出resppinn，通过高效的坐标编码和元学习策略加速3D CTP分析，并引入梗死核心分割功能。
- **论文链接**：[Accelerating physics-informed neural fields](https://raw.githubusercontent.com/mlresearch/v250/main/assets/vries24a/vries24a.pdf)

---

## 99. Target and Task specific Source-Free Domain Adaptive Image Segmentation
- **任务**：医学图像分割中的源自由无监督领域适应。
- **数据集**：CHASE、RITE、HRF（2D视网膜图像）和BraTS 2019（3D脑肿瘤MRI图像）。
- **方法**：提出TT-SFUDA，通过两阶段适应（目标特定适应和任务特定适应）优化分割性能，结合伪标签生成、教师-学生自训练和增强一致性损失。
- **论文链接**：[Target and Task specific Source-Free Domain Adaptive Image Segmentation](https://raw.githubusercontent.com/mlresearch/v250/main/assets/vs24a/vs24a.pdf)

---

## 100. Joint Motion Estimation with Geometric Deformation Correction for Fetal Echo Planar Images via Deep Learning
- **任务**：胎儿运动校正，同时估计胎儿大脑的刚性运动和局部几何变形。
- **数据集**：15名受试者的胎儿MRI扫描数据，包含1881对3D EPI图像。
- **方法**：提出了一种端到端的深度学习框架，结合刚性运动估计和几何变形估计，通过联合学习框架同时处理胎儿运动和几何变形。
- **论文链接**：[Joint Motion Estimation](https://raw.githubusercontent.com/mlresearch/v250/main/assets/wang24a/wang24a.pdf)

---

## 101. OFELIA: Optical Flow-based Electrode Localization
- **任务**：在X射线序列中自动定位导管电极。
- **数据集**：15名患者的心脏消融手术X射线序列，包含560个序列（14,768帧）用于训练，346个序列（7,711帧）用于测试。
- **方法**：提出了一种基于光流的深度学习网络OFELIA，通过整合连续帧之间的时间信息和光流图来提高电极定位精度。
- **论文链接**：[OFELIA](https://raw.githubusercontent.com/mlresearch/v250/main/assets/wang24b/wang24b.pdf)

---

## 102. Skin Malignancy Classification Using Patients’ Skin Images and Meta-data: Multimodal Fusion for Improving Fairness
- **任务**：通过多模态融合（皮肤图像和元数据）提高皮肤癌分类的准确性和公平性。
- **数据集**：Diverse Dermatology Images（DDI）数据集，包含656张图像和患者特征（肤色、癌症类型等）。
- **方法**：结合图像特征和元数据（如肤色指标），通过特征融合和学习特征融合模型提高分类性能，减少肤色相关的性能差异。
- **论文链接**：[Skin Malignancy Classification](https://raw.githubusercontent.com/mlresearch/v250/main/assets/wang24c/wang24c.pdf)

---

## 103. Medical diffusion on a budget: Textual Inversion for medical image generation
- **任务**：在有限的计算资源和数据条件下，通过Textual Inversion技术生成高质量的医学图像。
- **数据集**：三个医学成像模态的小数据集（前列腺MRI、胸部X光和组织病理学图像），每个模态100个样本。
- **方法**：通过训练文本嵌入向量，使Stable Diffusion模型适应不同的医学成像模态，生成诊断准确的图像。
- **论文链接**：[Medical diffusion on a budget](https://raw.githubusercontent.com/mlresearch/v250/main/assets/wilde24a/wilde24a.pdf)

---

## 104. IST-editing: Infinite Spatial Transcriptomic editing in a generated gigapixel mouse pup
- **任务**：在生成的千兆像素小鼠胚胎中进行基因表达引导的编辑。
- **数据集**：Xenium ST数据集，包含一个一天大的小鼠胚胎的379-plex基因转录计数和DAPI染色的WSI。
- **方法**：基于StyleGAN框架，通过基因表达数据作为输入，生物医学图像作为输出进行训练，实现无缝合成任意大小的生物图像。
- **论文链接**：[IST-editing](https://raw.githubusercontent.com/mlresearch/v250/main/assets/wu24a/wu24a.pdf)

---

## 105. Leveraging Probabilistic Segmentation Models for Improved Glaucoma Diagnosis: A Clinical Pipeline Approach
- **任务**：利用概率分割模型提高青光眼诊断的准确性。
- **数据集**：Ch´aks.u和RIGA眼底图像数据集，包含1345张和750张眼底图像。
- **方法**：提出一种多阶段诊断流程，包括概率分割、视网膜厚度曲线（RTC）提取和不确定性传播，以整合概率分割模型中的不确定性。
- **论文链接**：[Leveraging Probabilistic Segmentation Models](https://raw.githubusercontent.com/mlresearch/v250/main/assets/wundram24a/wundram24a.pdf)

---

## 106. Semi-Supervised Segmentation via Embedding Matching
- **任务**：在训练过程中利用少量标记图像和大量未标记图像进行半监督分割。
- **数据集**：950名受试者的髋骨CT扫描数据，手动分割为训练集、验证集和测试集。
- **方法**：提出一种基于嵌入匹配的半监督分割方法，通过不确定性分析和最近邻伪标签化来处理未标记图像。
- **论文链接**：[Semi-Supervised Segmentation](https://raw.githubusercontent.com/mlresearch/v250/main/assets/xie24a/xie24a.pdf)

---

## 107. Deformation-aware GAN for Medical Image Synthesis with Substantially Misaligned Pairs
- **任务**：解决医学图像合成中成对图像严重错位的问题。
- **数据集**：模拟大脑数据集（BraTS）和真实世界的肺部MRI-CT数据集。
- **方法**：提出DA-GAN，通过多目标逆一致性和变形感知对抗损失动态校正错位，提高图像合成质量。
- **论文链接**：[Deformation-aware GAN](https://raw.githubusercontent.com/mlresearch/v250/main/assets/xin24a/xin24a.pdf)

---

## 108. Feasibility and benefits of joint learning from MRI databases with different brain diseases and modalities for segmentation
- **任务**：探索从不同脑部病理和模态的MRI数据库中联合学习的可行性和优势。
- **数据集**：7个包含5种脑部病理和不同MRI模态集的数据库。
- **方法**：开发并比较了Multi-Unet、LFUnet和MAFUnet三种方法，通过联合训练多个数据库，提高模型的泛化能力。
- **论文链接**：[Feasibility and benefits of joint learning](https://raw.githubusercontent.com/mlresearch/v250/main/assets/xu24a/xu24a.pdf)

---

## 109. Erase to Enhance: Data-Efficient Machine Unlearning in MRI Reconstruction
- **任务**：在MRI重建中实现机器遗忘，去除特定数据样本以符合隐私法规并减少偏见。
- **数据集**：FastMRI数据集，包含多线圈大脑和膝关节图像。
- **方法**：提出了一种数据高效的机器遗忘方法，通过遗忘算法（如GA-ℓ1和NL）结合微调，实现对特定数据的去除。
- **论文链接**：[Erase to Enhance](https://raw.githubusercontent.com/mlresearch/v250/main/assets/xue24a/xue24a.pdf)

---

## 110. Evaluating Age-Related Anatomical Consistency in Synthetic Brain MRI against Real-World Alzheimer’s Disease Data
- **任务**：评估通过深度生成模型（如StyleGAN3）生成的脑部MRI图像在模拟与年龄相关的解剖变化以及阿尔茨海默病（AD）相关解剖变化方面的生物学合理性。
- **数据集**：使用了UK Biobank（UKB）和Alzheimer’s Disease Neuroimaging Initiative（ADNI）的真实MRI脑部扫描图像，以及通过StyleGAN3模型生成的合成图像。
- **方法**：通过视觉图灵测试（VTT）评估合成图像的真实性，并使用基于U-Net的分割模型量化评估合成图像与真实图像之间的解剖学一致性。通过统计测试评估合成图像与真实图像在海马体和侧脑室体积分布上的差异。
- **论文链接**：[Evaluating Age-Related Anatomical Consistency](https://raw.githubusercontent.com/mlresearch/v250/main/assets/yassin24a/yassin24a.pdf)

---

## 111. PAAN: Pyramid Attention Augmented Network for polyp segmentation
- **任务**：提高医学图像中息肉分割的准确性，特别是在边界模糊和背景干扰的情况下。
- **数据集**：使用了Kvasir、CVC-ClinicDB、CVC300、ETIS和CVC-colonDB五个息肉数据集。
- **方法**：提出了Pyramid Attention Augmented Network（PAAN），通过金字塔特征分流结构和空间注意力机制，减少信息丢失并提高特征表示的质量。PAAN包含低分辨率去噪模块（LRD）和增强空间注意力模块（ESA），以改善息肉边界的平滑度和背景抑制。
- **论文链接**：[PAAN](https://raw.githubusercontent.com/mlresearch/v250/main/assets/yi24a/yi24a.pdf)

---

## 112. Style Randomization Improves the Robustness of Breast Density Estimation in MR Images
- **任务**：提高乳腺密度估计在MRI图像中的鲁棒性，特别是在脂肪含量变化较大的情况下。
- **数据集**：使用了内部训练集（包含Dixon图像的乳腺MRI数据）和两个公开数据集（Müller-Franzes和Saha数据集）。
- **方法**：提出了一种风格随机化技术，通过混合水图像和脂肪图像来增加训练数据的风格多样性，从而提高网络对脂肪含量变化的适应性。该方法结合了深度强化学习（DRL）和选择性经验回放（SERIL），以实现更好的特征学习和泛化能力。
- **论文链接**：[Style Randomization](https://raw.githubusercontent.com/mlresearch/v250/main/assets/yuksel24a/yuksel24a.pdf)

---

## 113. Boundary-aware Contrastive Learning for Semi-supervised Nuclei Instance Segmentation
- **任务**：在半监督学习场景下，提高病理图像中细胞核实例分割的准确性，特别是在细胞核边界处的噪声问题。
- **数据集**：使用了CryoNuSeg、DigestPath和MoNuSeg三个公共数据集。
- **方法**：提出了边界感知对比学习网络（BASS），包含低分辨率去噪（LRD）模块和跨感兴趣区域（RoI）对比学习（CRC）模块。LRD模块通过伪标签去噪改善细胞核边界的平滑度，而CRC模块则通过边界特征对比学习增强前景和背景之间的区分能力。
- **论文链接**：[Boundary-aware Contrastive Learning](https://raw.githubusercontent.com/mlresearch/v250/main/assets/zhang24a/zhang24a.pdf)

---

## 114. Towards a Collective Medical Imaging AI: Enabling Continual Learning from Peers
- **任务**：提出一种异步去中心化的联邦终身学习（ADFLL）框架，允许代理在异步和去中心化的环境中持续学习，以提高医学成像AI的鲁棒性和效率。
- **数据集**：使用了多参数脑MRI数据集（BraTS）和多模态全身成像数据集（包括PET、CT、MRI-T1、MRI-DIXON-F和MRI-DIXON-W序列）。
- **方法**：ADFLL框架结合了深度强化学习（DRL）和选择性经验回放（SERIL），允许代理不仅从自己的经验中学习，还能从其他代理共享的经验中学习。通过预定义的中心节点进行通信，提高了通信效率并保持了系统的灵活性。
- **论文链接**：[Towards a Collective Medical Imaging AI](https://raw.githubusercontent.com/mlresearch/v250/main/assets/zheng24a/zheng24a.pdf)

---

## 115. Conditional Generation of 3D Brain Tumor ROIs via VQGAN and Temporal-Agnostic Masked Transformer
- **任务**：生成高分辨率和多样化的3D脑肿瘤感兴趣区域（ROIs）的合成图像，以提高脑肿瘤类型分类的准确性。
- **数据集**：使用了BraTS 2019数据集中的FLAIR序列数据。
- **方法**：提出了一个基于矢量量化GAN（VQGAN）和掩码变换器的类条件生成框架。该框架通过学习特征图中的重要性分数，并使用掩码变换器学习离散标记之间的关系，从而生成高质量的脑肿瘤ROIs。
- **论文链接**：[Conditional Generation of 3D Brain Tumor ROIs](https://raw.githubusercontent.com/mlresearch/v250/main/assets/zhou24a/zhou24a.pdf)

---

## 116. DDA: Dimensionality Driven Augmentation Search for Contrastive Learning in Laparoscopic Surgery
- **任务**：在腹腔镜手术的对比学习中自动搜索合适的数据增强策略，以提高表示学习的质量。
- **数据集**：使用了私有的SVHM数据集和公开的Cholec80数据集。
- **方法**：提出了Dimensionality Driven Augmentation Search（DDA）方法，通过优化深度表示的局部维度（LID）作为代理目标，可微分地搜索对比学习中的合适数据增强策略。DDA框架通过固定编码器，仅优化增强策略的参数，以最大化表示的LID。
- **论文链接**：[DDA](https://raw.githubusercontent.com/mlresearch/v250/main/assets/zhou24b/zhou24b.pdf)

---

## 117. Predicting Atrial Fibrillation Treatment Outcome with Siamese Multi-modal Fusion and Cardiac Digital Twins
- **任务**：预测心房颤动（AF）消融治疗的结果，通过模拟心房电活动来评估不同消融策略的效果。
- **数据集**：使用了基于1000名虚拟患者的大规模计算机模拟数据集，这些数据集基于临床数据生成。
- **方法**：提出了一个基于深度学习的管道，结合心脏数字孪生技术和多模态特征融合。该管道使用Siamese架构，融合来自左心房和右心房的多模态特征图，并通过深度学习模型预测AF消融的结果。
- **论文链接**：[Predicting Atrial Fibrillation Treatment Outcome](https://raw.githubusercontent.com/mlresearch/v250/main/assets/zolotarev24a/zolotarev24a.pdf)

---
