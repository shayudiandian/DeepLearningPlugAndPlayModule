# DeepLearningPlugAndPlayModule

## 介绍

深度学习即插即用模块代码复现（代码 + 论文标题 + 论文地址）  基于PyTorch（参考论文给出的源代码）

代码输入张量 N×C×H×W，输出张量 N×C×H×W

创新点（涨点）必备！！！

缝合方式       串行、并行、组合、......（最好将不同模块组合成自己的新模块）

使用位置       特征提取层、任务后处理阶段、特征融合层、注意力模块、跳跃连接、编码器、解码器、...各种位置都可以，只要你讲的明白！！！

不局限于论文所用场景，可尝试用于任何CV任务



如果对你有帮助，点个Star鼓励！！

持续更新中......





## 已复现

**注意力模块**

|       模块       |                          期刊/会议                           | 简单描述                                                     | 论文标题                                                     |                                                                                      论文地址                                                                                       |
|:--------------:|:--------------------------------------------------------:| ------------------------------------------------------------ | ------------------------------------------------------------ |:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------:|
|     SENet      |                        CVPR 2018                         | 通道注意力                                                   | Squeeze-and-Excitation Networks                              |                               [url](https://openaccess.thecvf.com/content_cvpr_2018/html/Hu_Squeeze-and-Excitation_Networks_CVPR_2018_paper.html)                               |
|    NonLocal    |                        CVPR 2018                         | 计算任意两个位置之间的交互直接捕捉远程依赖，而不用局限于相邻点 | Non-Local Neural Networks                                    |                                 [url](https://openaccess.thecvf.com/content_cvpr_2018/html/Wang_Non-Local_Neural_Networks_CVPR_2018_paper.html)                                 |
|      CBAM      |                        ECCV 2018                         | 通道注意力+空间注意力                                        | CBAM: Convolutional Block Attention Module                   |                           [url](https://openaccess.thecvf.com/content_ECCV_2018/html/Sanghyun_Woo_Convolutional_Block_Attention_ECCV_2018_paper.html)                           |
|                |                                                          |                                                              |                                                              |                                                                                                                                                                                 |
|     DANet      |                        CVPR 2019                         | 位置注意力+通道注意力                                        | Dual Attention Network for Scene Segmentation                |                        [url](https://openaccess.thecvf.com/content_CVPR_2019/html/Fu_Dual_Attention_Network_for_Scene_Segmentation_CVPR_2019_paper.html)                        |
|      ECA       |                        CVPR 2020                         | 通道注意力                                                   | ECA-Net: Efficient Channel Attention for Deep Convolutional Neural Networks |        [url](https://openaccess.thecvf.com/content_CVPR_2020/html/Wang_ECA-Net_Efficient_Channel_Attention_for_Deep_Convolutional_Neural_Networks_CVPR_2020_paper.html)         |
|       CA       |                        CVPR 2021                         | 坐标注意力                                                   | Coordinate Attention for Efficient Mobile Network Design     |                  [url](https://openaccess.thecvf.com/content/CVPR2021/html/Hou_Coordinate_Attention_for_Efficient_Mobile_Network_Design_CVPR_2021_paper.html)                   |
|     FcaNet     |                        ICCV 2021                         | 从频域角度出发的通道注意力                                   | FcaNet: Frequency Channel Attention Networks                 |                         [url](https://openaccess.thecvf.com/content/ICCV2021/html/Qin_FcaNet_Frequency_Channel_Attention_Networks_ICCV_2021_paper.html)                         |
|      SRA       |                        ICCV 2021                         | 空间缩减注意力，降低学习高分辨率特征图的资源成本             | Pyramid Vision Transformer: A Versatile Backbone for Dense Prediction Without Convolutions |        [url](https://openaccess.thecvf.com/content/ICCV2021/html/Wang_Pyramid_Vision_Transformer_A_Versatile_Backbone_for_Dense_Prediction_Without_ICCV_2021_paper.html)        |
|                |                                                          |                                                              |                                                              |                                                                                                                                                                                 |
|     SA-Net     |                       ICASSP 2021                        | 轻量且高效的置换注意力                                       | SA-Net: Shuffle Attention for Deep Convolutional Neural Networks |                                                          [url](https://ieeexplore.ieee.org/abstract/document/9414568)                                                           |
|     SimAM      |                        PMLR 2021                         | 轻量且高效的无参注意力                                       | SimAM: A Simple, Parameter-Free Attention Module for Convolutional Neural Networks |                                                                [url](https://proceedings.mlr.press/v139/yang21o)                                                                |
|                |                                                          |                                                              |                                                              |                                                                                                                                                                                 |
|      DAT       |                        CVPR 2022                         | 轻量且高效的可变形注意力                                     | Vision Transformer With Deformable Attention                 |           [url](https://openaccess.thecvf.com/content/CVPR2022/html/Xia_Vision_Transformer_With_Deformable_Attention_CVPR_2022_paper.html?ref=https://githubhelp.com)           |
|                |                                                          |                                                              |                                                              |                                                                                                                                                                                 |
|      MCA       | Engineering Applications of Artificial Intelligence 2023 | 多维协作注意力                                               | MCA: Multidimensional collaborative attention in deep convolutional neural networks for image recognition |                                                 [url](https://www.sciencedirect.com/science/article/abs/pii/S0952197623012630)                                                  |
|      CGA       |                        CVPR 2023                         | 级联群注意力                                                 | EfficientViT: Memory Efficient Vision Transformer With Cascaded Group Attention |       [url](https://openaccess.thecvf.com/content/CVPR2023/html/Liu_EfficientViT_Memory_Efficient_Vision_Transformer_With_Cascaded_Group_Attention_CVPR_2023_paper.html)        |
|      MSPA      | Engineering Applications of Artificial Intelligence 2024 | 多尺度空间金字塔注意力                                       | Multi-scale spatial pyramid attention mechanism for image recognition: An effective approach |                                                 [url](https://www.sciencedirect.com/science/article/abs/pii/S0952197624004196)                                                  |
| AgentAttention |                        ECCV 2024                         | Softmax与线性注意力的整合                                    | Agent Attention: On the Integration of Softmax and Linear Attention |                                                      [url](https://link.springer.com/chapter/10.1007/978-3-031-72973-7_8)                                                       |
|      CGLU      |                        CVPR 2024                         | 卷积门控通道注意力，适用于CV和NLP任务                        | TransNeXt: Robust Foveal Visual Perception for Vision Transformers |              [url](https://openaccess.thecvf.com/content/CVPR2024/html/Shi_TransNeXt_Robust_Foveal_Visual_Perception_for_Vision_Transformers_CVPR_2024_paper.html)              |
|      MLKA      |                        CVPR 2024                         | 多尺度大核注意力                                             | Multi-scale Attention Network for Single Image Super-Resolution |          [url](https://openaccess.thecvf.com/content/CVPR2024W/NTIRE/html/Wang_Multi-scale_Attention_Network_for_Single_Image_Super-Resolution_CVPRW_2024_paper.html)           |
|      MAB       |                        CVPR 2024                         | 增强特征提取和细节恢复                                       | Multi-scale Attention Network for Single Image Super-Resolution |          [url](https://openaccess.thecvf.com/content/CVPR2024W/NTIRE/html/Wang_Multi-scale_Attention_Network_for_Single_Image_Super-Resolution_CVPRW_2024_paper.html)           |
|      LGAG      |                        CVPR 2024                         |         大核分组注意力门控模块                                          |   EMCAD: Efficient Multi-scale Convolutional Attention Decoding for Medical Image Segmentation                                                              |                                                                                     [url](https://openaccess.thecvf.com/content/CVPR2024/html/Rahman_EMCAD_Efficient_Multi-scale_Convolutional_Attention_Decoding_for_Medical_Image_Segmentation_CVPR_2024_paper.html)                                                                                     |
|      AGF       |                        WACV 2024                         | 主要用于3D人体关键点检测任务                                 | MotionAGFormer: Enhancing 3D Human Pose Estimation With a Transformer-GCNFormer Network | [url](https://openaccess.thecvf.com/content/WACV2024/html/Mehraban_MotionAGFormer_Enhancing_3D_Human_Pose_Estimation_With_a_Transformer-GCNFormer_Network_WACV_2024_paper.html) |
|                |                                                          |                                                              |                                                              |                                                                                                                                                                                 |
|                |                                                          |                                                              |                                                              |                                                                                                                                                                                 |
|                |                                                          |                                                              |                                                              |                                                                                                                                                                                 |



**特征提取/融合模块**

|   模块    |                    期刊/会议                    | 简单描述                                                     | 论文标题                                                     |                           论文地址                           |
| :-------: | :---------------------------------------------: | :----------------------------------------------------------- | :----------------------------------------------------------- | :----------------------------------------------------------: |
|    AFF    |                    WACV 2021                    | 基于注意力的特征融合                                         | Attentional Feature Fusion                                   | [url](https://openaccess.thecvf.com/content/WACV2021/html/Dai_Attentional_Feature_Fusion_WACV_2021_paper.html) |
|   PSFM    |             Information Fusion 2023             | 多尺度图像特征融合                                           | Rethinking the necessity of image fusion in high-level vision tasks: A practical infrared and visible image fusion network based on progressive semantic injection and scene fidelity | [url](https://www.sciencedirect.com/science/article/abs/pii/S1566253523001860) |
|           |                                                 |                                                              |                                                              |                                                              |
|   GLSA    |                    PRCV 2023                    | 全局和局部空间特征融合                                       | DuAT: Dual-Aggregation Transformer Network for Medical Image Segmentation | [url](https://link.springer.com/chapter/10.1007/978-981-99-8469-5_27?utm_source=chatgpt.com) |
|    LSK    |                    ICCV 2023                    | 大型选择性核                                                 | Large Selective Kernel Network for Remote Sensing Object Detection | [url](https://openaccess.thecvf.com/content/ICCV2023/html/Li_Large_Selective_Kernel_Network_for_Remote_Sensing_Object_Detection_ICCV_2023_paper.html) |
|   MFII    |           Medical Image Analysis 2024           | 双分支信息交互提取图像特征模块                               | I²U-Net: A dual-path U-Net with rich information interaction for medical image segmentation | [url](https://www.sciencedirect.com/science/article/abs/pii/S136184152400166X) |
|    FCA    |              Neural Networks 2024               | 增强局部和全局特征信息交互                                   | Unsupervised Bidirectional Contrastive Reconstruction and Adaptive Fine-Grained Channel Attention Networks for image dehazing | [url](https://www.sciencedirect.com/science/article/abs/pii/S0893608024002387) |
|   SMFA    |                    ECCV 2024                    | 特征融合模块，高分辨率图像恢复，暗光增强，小目标分割，小目标检测等所有CV任务通用模块 | SMFANet: A Lightweight Self-Modulation Feature Aggregation Network for Efficient Image Super-Resolution | [url](https://link.springer.com/chapter/10.1007/978-3-031-72973-7_21) |
|           |                                                 |                                                              |                                                              |                                                              |
|   CCFF    |                    CVPR 2024                    | 跨尺度特征融合                                               | DETRs Beat YOLOs on Real-time Object Detection               | [url](https://openaccess.thecvf.com/content/CVPR2024/html/Zhao_DETRs_Beat_YOLOs_on_Real-time_Object_Detection_CVPR_2024_paper.html) |
|           |                                                 |                                                              |                                                              |                                                              |
|   CSAM    |                    WACV 2024                    | 交叉切片注意力                                               | CSAM: A 2.5D Cross-Slice Attention Module for Anisotropic Volumetric Medical Image Segmentation | [url](https://openaccess.thecvf.com/content/WACV2024/html/Hung_CSAM_A_2.5D_Cross-Slice_Attention_Module_for_Anisotropic_Volumetric_Medical_WACV_2024_paper.html) |
| CGAFusion |                    TIP 2024                     | 低级特征和高级特征融合，图像去雾                             | DEA-Net: Single Image Dehazing Based on Detail-Enhanced Convolution and Content-Guided Attention | [url](https://ieeexplore.ieee.org/abstract/document/10411857) |
|           |                                                 |                                                              |                                                              |                                                              |
|   CAFM    | IEEE Geoscience and Remote Sensing Letters 2024 | 卷积和注意力特征融合                                         | Hybrid Convolutional and Attention Network for Hyperspectral Image Denoising | [url](https://ieeexplore.ieee.org/abstract/document/10445289) |
|           |                                                 |                                                              |                                                              |                                                              |
|           |                                                 |                                                              |                                                              |                                                              |



**上采样**

|   模块   | 期刊/会议 | 简单描述   | 论文标题                                   |                           论文地址                           |
| :------: | :-------: | :--------- | :----------------------------------------- | :----------------------------------------------------------: |
| DySample | ICCV 2023 | 动态上采样 | Learning to Upsample by Learning to Sample | [url](https://openaccess.thecvf.com/content/ICCV2023/html/Liu_Learning_to_Upsample_by_Learning_to_Sample_ICCV_2023_paper.html) |



**下采样**

| 模块 | 期刊/会议 | 简单描述 | 论文标题 | 论文地址 |
| :--: | :-------: | :------- | :------- | :------: |
|      |           |          |          |          |



**即插即用卷积**

替换普通卷积即可有效涨点！

|    卷积模块    |              期刊/会议              | 简单描述                                                   | 论文标题                                                     |                                                                                 论文地址                                                                                  |
| :------------: |:-------------------------------:| :--------------------------------------------------------- | :----------------------------------------------------------- |:---------------------------------------------------------------------------------------------------------------------------------------------------------------------:|
| MorphologyConv |            TIP 2023             | 形态学卷积                                                 | Single-Source Domain Expansion Network for Cross-Scene Hyperspectral Image Classification |                                                     [url](https://ieeexplore.ieee.org/abstract/document/10050427)                                                     |
|     SCConv     |            CVPR 2023            | 轻量化高效的空间和通道重建卷积                             | SCConv: Spatial and Channel Reconstruction Convolution for Feature Redundancy |    [url](https://openaccess.thecvf.com/content/CVPR2023/html/Li_SCConv_Spatial_and_Channel_Reconstruction_Convolution_for_Feature_Redundancy_CVPR_2023_paper.html)    |
|     DCNv4      |            CVPR 2024            | 可变形卷积v4                                               | Efficient Deformable ConvNets: Rethinking Dynamic and Sparse Operator for Vision Applications | [url](https://openaccess.thecvf.com/content/CVPR2024/html/Xiong_Efficient_Deformable_ConvNets_Rethinking_Dynamic_and_Sparse_Operator_for_Vision_CVPR_2024_paper.html) |
|    StarConv    |            CVPR 2024            | 直接使用卷积层对分辨率进行降采样，并在每个阶段将信道数加倍 | Rewrite the Stars                                            |                                 [url](https://openaccess.thecvf.com/content/CVPR2024/html/Ma_Rewrite_the_Stars_CVPR_2024_paper.html)                                  |
|  DynamicConv   |            CVPR 2024            | 动态卷积，引入额外参数但只增加边际FLOPs                    | ParameterNet: Parameters Are All You Need for Large-scale Visual Pretraining of Mobile Networks |    [url](https://openaccess.thecvf.com/content/CVPR2024/html/Han_ParameterNet_Parameters_Are_All_You_Need_for_Large-scale_Visual_Pretraining_CVPR_2024_paper.html)    |
|        CAMixer        |            CVPR 2024            |      内容感知混合卷积                                     |              CAMixerSR: Only Details Need More "Attention"                                                                                   |                                                                                [url](https://openaccess.thecvf.com/content/CVPR2024/html/Wang_CAMixerSR_Only_Details_Need_More_Attention_CVPR_2024_paper.html)                                                                                |
|     DEConv     |            TIP 2024             | 细节增强                                                   | DEA-Net: Single Image Dehazing Based on Detail-Enhanced Convolution and Content-Guided Attention |                                                     [url](https://ieeexplore.ieee.org/abstract/document/10411857)                                                     |
|     WTConv     |            ECCV 2024            | 小波变换卷积                                               | Wavelet Convolutions for Large Receptive Fields              |                                                 [url](https://link.springer.com/chapter/10.1007/978-3-031-72949-2_21)                                                 |
|    CFBConv     |            AAAI 2024            | 具有语义信息的卷积                                         | SCTNet: Single-Branch CNN with Transformer Semantic Information for Real-Time Segmentation |                                                     [url](https://ojs.aaai.org/index.php/AAAI/article/view/28457)                                                     |
|                |                                 |                                                            |                                                              |                                                                                                                                                                       |
|     LDConv     | Image and Vision Computing 2024 | 线性可变形卷积                                             | LDConv: Linear deformable convolution for improving convolutional neural networks |                                            [url](https://www.sciencedirect.com/science/article/abs/pii/S0262885624002956)                                             |
|                |                                 |                                                            |                                                              |                                                                                                                                                                       |

