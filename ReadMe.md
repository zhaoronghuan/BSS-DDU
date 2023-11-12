# 项目名称
BSS-DDU: Dual-Decoder Fusion UNetFormer-based Bimodal Semantic Segmentation for Automated Coal Maceral Identification

# 项目描述
本项目主要是用于训练不同的深度学习模型，包括PSP, deeplabV3+, Unet, ATTUNet, UNetFormer, UNetFormerEDGE等。

这些模型用于处理双模态图像数据语义分割任务，具体数据集因为保密原因不能提供。

项目中还包含了模型训练的过程，以及训练结果的保存。

本项目还在补充完善中（2023.11.10）

# 如何运行
首先，你需要安装所有必要的依赖，可以通过以下命令安装：
```pip install -r requirements.txt```

然后，你可以通过运行main.py文件来开始训练和测试模型：
```python main.py```

# 结果
训练和测试的结果会被保存在"log/"目录下，包括每个模型的每折的最佳模型文件（.pkl）和训练日志（.json）。

你还可以通过运行代码来查看训练损失，验证损失和mIOU的可视化结果。

# 文件结构
以下是项目中各个文件的功能描述：

--cut_image1/, cut_image2/, cut_label/:        包含本项目所使用的双模态数据集及其标签。

--cut_label_v/:  标签的可视化结果。

--log/：        这个目录下会保存训练和测试的结果，包括每个模型的最佳模型文件（.pkl）和训练日志（.json）。

--utils.py：    包含了一些工具函数，如模型选择、训练等。

--dataset.py：  包含了数据集加载的相关代码，主要是Dataset类。

--loss.py：     这个文件包含了用于训练模型的损失函数，例如Dice_Loss等。

--main.py：     这是项目的主入口，包含了模型的整个训练过程以及参数设置等内容。

--pre_processing.ipynb：    这个文件包含了数据预处理的相关代码，例如图像切分、增强等。

--README.md：   这个文件包含了项目的介绍和使用说明。

--requirements.txt：    这个文件列出了项目运行所需的所有依赖。

--score.py：    这个文件包含了评价模型性能的评分函数。

--UnetFormer.py：这个文件包含了UnetFormer及UnetFormerEdge模型的实现代码。

# 提出问题
如果你有任何问题或者建议，欢迎提出。