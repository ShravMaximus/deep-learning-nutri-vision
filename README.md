# NutriVision
This project explores different deep learning architectures: a basic Convolutional Neural Network (CNN), Rank Expansion Network (RexNet150), EfficientNet, Memory Graph Convolutional Network (M-GCN), and Attention Driven Dynamic Graph Convolutional Network (ADD-GCN) on multi-label image classification to identify ingredients present in various Indian dishes. Identifying ingredients as outcomes, we integrate Large Language Models (LLMs) to analyze corresponding nutritional information. 
Nutritionists, dietitians, health-conscious individuals, and food service providers would benefit from this project. If successful, it would enable automated and accurate identification of ingredients in dishes, allowing for precise nutritional analysis. This could help people make informed dietary choices, manage allergies, track nutrient intake, and support health and wellness programs.

## Project Overview
The project consists of the following main steps:
    1. Data collection and preprocessing
    2. Deep learning models implementation and training
    3. Model evaluation and prediction
    4. Google's LLM integration and nutrition analysis generation
    5. Web GUI deployment

## Requirements
- Python 3.x
- Libraries: Pandas, Scikit-learn, Pytorch, Tensorflow, Keras, Matplotlib
- Hardware: GPU
- Environment: VSCode, Jupyter Notebook

You can install the required libraries using pip:
```sh
    pip install pandas scikit-learn tensorflow keras matplotlib

## Usage 
    1. Data Downloading, Exploratory, and Preprocessing
        - Running the script: `rt_indian_data_processing.ipynb`

    2. Model Creation and Training
        - For basic CNN and EfficientNet: run `python3 shrabhat-munging-experimentation-llm.py`
        - For RexNet150: run the script `vynguyen_rexnet150.ipynb`
        - For M-GCN and ADD-GCN: run the script `test_model.ipynb`

    3. Model Evaluation and Prediction
        - The models were evaluated against their history of loss and accuracy over training epochs. The resulting models exhibited desired training and validation accuracy over 0.7 and a consistent decreasing trend in both training and validation loss.
        - Evaluation metrics included Mean Average Precision (mAP), Mean Average Recall (mAR), and Cross-Entropy as the loss function.
        - Actual and predicted labels are plotted on images for comparison.

