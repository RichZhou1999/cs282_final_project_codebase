# Fine-tuning Vision Transformer-Based Model forPose-Estimation
Alex Liang, Yihua Zhou, Abdullah Azhar, Anjana Manjunath

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
Link: https://www.kaggle.com/azhara001/simple-text-overfitting/edit
This notebook was trained on 'simple text' using 10 images chosen randomly

## Simple task Baseline: Train the model on larger simple dataset to verify the model has enough ability
Link: https://www.kaggle.com/yihuazhou1999/simple-text-model-checkpoint <br />
This notebook was trained on "simple text" aiming to predict the position of the neck of the person in the image. <br />
The training accuracy is around 90% and the validation accuracy is around 15%. It shows that the model has the potential to learn the desired task.

## Complex task: Training for all 16 Key Points

