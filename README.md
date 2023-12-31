# Fine-tuning BLIP Model for Pose-Estimation task
Jinxuan Liang, Yihua Zhou, Abdullah Azhar, Anjana Manjunath

<img src="https://github.com/RichZhou1999/cs282_final_project_codebase/blob/12516590ee5d5da61698a8490e0a1c6a263ff09d/sample_results.png" width="500">

In this notebook, we provide the code for 
1) Preprocessing the MPII dataset to get the fully labeled and visible data
2) Training loop and hyperparameters for training our base model
3) Three checkpoints for different tasks from simple to hard
5) Plots of our training process

# Checkpoints
## All notebooks and datasets are stored on kaggle. Currently, we do not support the notebook with colab. Please run the notebook in kaggle. 
### Step1: Create a kaggle account
All the notebooks are stored in kaggle, so a kaggle account is needed
### Step2: Run the code in the kaggle notebook(Need to activate GPU accelerator in kaggle!)
You can run the notebook with the link provided below.

## Warmup: Overfit the model on small dataset to verify the method work
Link: https://www.kaggle.com/code/yihuazhou1999/simple-text-overfitting <br />
This notebook was trained on 'simple text' using 10 images chosen randomly

## Simple task Baseline: Train the model on larger simple dataset to verify the model has enough ability
Link: https://www.kaggle.com/yihuazhou1999/simple-text-model-checkpoint <br />
This notebook was trained on "simple text" aiming to predict the position of the neck of the person in the image. <br />
The training accuracy is around 90% and the validation accuracy is around 15%. It shows that the model has the potential to learn the desired task.

## Complex task: Training for all 16 Key Points
Link: https://www.kaggle.com/code/yihuazhou1999/blip-fine-tunning <br />
This is the notebook that can be used to play around with the models and data. One can run the training loop on the pre-trained BLIP model, which will 
take 1.5 hours to reach a similar result as ours. You can also load our checkpoints(early, mid, late) to run inference on the validation data or user input
data. To load the model, run the cell right before the training loop. Details can be found in the notebook. 

## Notebook for generating assets for submission
Link: [https://www.kaggle.com/code/a1exliang/blip-fine-tunning?scriptVersionId=152812535](https://www.kaggle.com/code/yihuazhou1999/blip-fine-tunning) <br />
This is the notebook we used to generate some of the figures and plots in our final report. 
