# Project Name
Dual-Decoder UNetFormer-based Bimodal Semantic Segmentation for Coal Maceral Identification

# Project Description
This project is mainly used for training various deep learning models, including PSP, deeplabV3+, Unet, ATTUNet, UNetFormer, UNetFormerEDGE, etc.

The models are suitable for bimodal coal maceral microscopic image semantic segmentation tasks. We provide the unlabeled raw dataset, [click here to download](https://pan.cumt.edu.cn/share/b05dbe75a684704faf5ca340b5).

The project includes the process of model training and the storage of training results.

# How to Run
First, you need to install all the necessary dependencies, which can be installed with the following command:
```pip install -r requirements.txt```

Then, you can start training and testing the models by running the main.py file:
```python main.py```

# Results
The training and testing results will be saved in the "log/" directory, including the best model files (.pkl) and training logs (.json) for each fold of each model.

You can also run the code to visualize the training loss, validation loss, and mIOU.

# File Structure
The following is a description of the functions of each file in the project:

--image/, label/:  Contains the bimodal dataset and its labels used in this project.

--log/:  This directory will save the training and testing results, including the best model files (.pkl) and training logs (.json) for each model.

--_utils.py:  Contains some utility functions, such as model selection and training.

--dataset.py:  Contains code related to dataset loading, mainly the Dataset class.

--loss.py:  This file contains the loss functions used for model training, such as Dice_Loss.

--main.py:  This is the main entry point of the project, which includes the entire model training process and parameter settings.

--pre_processing.ipynb:  This file contains code related to data preprocessing, such as image segmentation and augmentation.

--README.md:  This file contains the project introduction and usage instructions.

--requirements.txt:  This file lists all the dependencies required to run the project.

--score.py:  This file contains the scoring functions for evaluating model performance.

--UNetFormer.py:  This file contains the implementation code of the UnetFormer and UnetFormerEdge models.

# Raise Questions
If you have any questions or suggestions, feel free to raise them.

Contact emails: liangzou@cumt.edu.cn, ronghuanzhao@cumt.edu.cn
