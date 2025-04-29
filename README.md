# Elderly Fall Detection Algorithm Based on Improved YOLOv5s (ITC 2024)

Zhongze Luo, Siying Jia, Hongjun Niu, Yifu Zhao, Xiaoyu Zeng, Guanghui Dong*

College of computer and control engineering, Northeast Forestry University, Harbin, 150040, China

The indoor fall detection for the elderly can effectively help the treatment after falling, but many existing detection methods have the problems of inconvenient use, high misjudgement rate and slow speed. Using deep learning methods can effectively solve these problems, and YOLOv5s is a kind of deep learning algorithm that can perform real-time fall detection. In order to achieve a more lightweight and higher detection accuracy, this paper proposes a fall detection algorithm for the elderly based on improved YOLOv5s, called YOLOv5s-GCC. Firstly, the original Conv and C3 structures are replaced by GhostConv and C3GhostV2 structures in backbone to achieve model lightweight, which reduces model computation and improves accuracy. Secondly, the lightweight upsampling operator CARAFE is introduced to expand the receptive field for data feature fusion and reduce the loss of feature information in upsampling. Finally, the deepest C3 is integrated with CBAM attention mechanism in the neck, because the deepest neck receives more abundant feature information, and CBAM can increase the efficiency of the algorithm in extracting important information from the feature map. Experimental results show that YOLOv5s-GCC has increased by 1.2% to 0.935 on the hybrid open source fall dataset mAP@0.5; FLOPs decreased by 29.1%. Params are reduced by 27.5% and have obvious advantages over
similar object detection algorithms.

Paper: [https://doi.org/10.5755/j01.itc.53.2.36336](https://doi.org/10.5755/j01.itc.53.2.36336)

Dataset and experimental data, 
Comparative experiments and visual comparison data: [Huggingface link](https://huggingface.co/datasets/luozhongze/YOLO-GCC/tree/main)
