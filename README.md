# MediMentor
MediMentor is an AI-powered health assistant designed to provide users with accurate and personalized responses to their health-related questions. By analyzing user inputs, MediMentor offers insights into symptoms, possible conditions, and recommended actions, facilitating a proactive approach to health management.

MediMentor Project Documentation

This project is divided into three main groups:

	•	Group 1: Preprocessing the data.
	•	Group 2: Model training.
	•	Group 3: Model evaluation and hyperparameter tuning.

Each group works on their specific branch, and the final step is to merge all the work into the main branch. Below are the step-by-step instructions for each group.

Clone the Repository (For all groups)

First, clone the repository locally to begin work:
git clone https://github.com/dhruv-pithadia/MediMentor.git
cd MediMentor

For Group 1 (Preprocessing Team)

Step 1: Switch to the Group 1 Branch
Switch to the group1-preprocessing branch and ensure it’s up to date:
git checkout group1-preprocessing
git pull origin group1-preprocessing

Step 2: Add Preprocessing Scripts
After writing your preprocessing scripts (in the preprocessing/ or scripts/ folder), stage and commit them:
git add .
git commit -m "Add preprocessing scripts"
git push origin group1-preprocessing


For Group 2 (Model Training Team)

Step 1: Switch to the Group 2 Branch
Switch to the group2-model-training branch:
git checkout group2-model-training
git pull origin group2-model-training

Step 2: Merge Preprocessing Data from Group 1
Before starting model training, merge the pre-processed data from group1-preprocessing:
git merge group1-preprocessing

If there are conflicts, Git will prompt you to resolve them manually. After resolving any conflicts, stage the changes:
git add .
git commit -m "Resolved merge conflicts between group1-preprocessing and group2-model-training"

Step 3: Add Model Training Scripts
After writing your model training scripts (in the models/ or scripts/ folder), stage and commit them:
git add .
git commit -m "Add model training code"
git push origin group2-model-training



For Group 3 (Evaluation and Tuning Team)

Step 1: Switch to the Group 3 Branch
Switch to the group3-evaluation-tuning branch:
git checkout group3-evaluation-tuning
git pull origin group3-evaluation-tuning

Step 2: Merge Model Data from Group 2
Before evaluating the model, merge the trained model from group2-model-training:
git merge group2-model-training

If there are conflicts, resolve them manually and stage the resolved files:
git add .
git commit -m "Resolved merge conflicts between group2-model-training and group3-evaluation-tuning"

Step 3: Add Evaluation and Tuning Scripts
After writing your evaluation and tuning scripts (in the evaluation/ folder), stage and commit them:
git add .
git commit -m "Add evaluation and tuning scripts"
git push origin group3-evaluation-tuning