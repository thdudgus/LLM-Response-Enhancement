# LLM-Response-Enhancement: Predicting Human Preferences

This guide outlines the steps to participate in the Kaggle competition for predicting human preferences to enhance LLM responses.    
[kaggle address: LLM Classification Finetuning](https://www.kaggle.com/competitions/llm-classification-finetuning)      

## 1. Join Kaggle Competition
* Create a Kaggle account if you don't have one.
* Join the "LLM Classification Finetuning" competition.
* Familiarize yourself with the rules, evaluation metric (Log Loss), and data format.

## 2. Notebook Setup
* Create a new notebook in Kaggle or your preferred environment.
* Add the competition dataset (`llm-classification-finetuning`) to your notebook.

## 3. Environment Settings
### RANDOM SEED
* Random seed: 42

### TF-IDF + Logistic Regression
* **Kaggle:**
    * Set Accelerator to **GPU P100**.
* **Colab:**
    * Set Runtime Type to **GPU (T4)**.
    * Upload `train.csv` and `test.csv` directly to the runtime file system (left sidebar > Files folder). *Note: Files are ephemeral and will be deleted upon runtime recycling.*   
    Adapt the `BASE_PATH` in your code to match your environment's data location.

### MiniLM + Logistic Regression
* **Kaggle:**
    * Set Accelerator to **GPU P100**.

### DeBERTa V3 (Fine-tuning)
* **Kaggle:**
    * Set Accelerator to **GPU T4 x2** for efficient fine-tuning.

## 4. Run Notebook
* Execute the cells in your notebook sequentially to train models and generate predictions.
* Ensure your final submission file matches the required format (`submission.csv`).
