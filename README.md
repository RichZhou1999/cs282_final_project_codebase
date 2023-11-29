# Fine-tuning Vision Transformer-Based Model forPose-Estimation
Jinxuan Liang, Yihua Zhou, Abdullah Azhar, Anjana Manjunath

In this notebook, we provide the code for 
1) Preprocessing the MPII dataset to get the fully labeled and visible data
2) Three checkpoints for different tasks from simple to hard
3) Plots of our training process

# Checkpoints
### Step1: Create a kaggle account
All the notebooks are stored in kaggle, so a kaggle account is needed
### Step2: Run the code in the kaggle notebook
You can run the notebook with the link provided below.

## Warmup: Overfit the model on small dataset to verify the method work
Link: https://www.kaggle.com/azhara001/simple-text-overfitting/edit <br />
This notebook was trained on 'simple text' using 10 images chosen randomly

## Simple task Baseline: Train the model on larger simple dataset to verify the model has enough ability
Link: https://www.kaggle.com/yihuazhou1999/simple-text-model-checkpoint <br />
This notebook was trained on "simple text" aiming to predict the position of the neck of the person in the image. <br />
The training accuracy is around 90% and the validation accuracy is around 15%. It shows that the model has the potential to learn the desired task.

## Complex task: Training for all 16 Key Points
Link: https://www.kaggle.com/code/a1exliang/blip-fine-tunning (Make sure the notebook version is 6) <br />
This is the notebook that can be used to play around with the models and data. One can run the training loop on the pre-trained BLIP model, which will 
take 1.5 hours to reach a similar result as ours. You can also load our checkpoints(early, mid, late) to run inference on the validation data or user input
data. To load the model, run the cell right before the training loop. Details can be found in the notebook. 

## Notebook for generating assets for submission
Link: https://www.kaggle.com/code/a1exliang/blip-fine-tunning?scriptVersionId=152812535 <br />
This is the notebook we used to generate some of the figures and plots in our final report. 

