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

## Usage
1. Data Downloading, Exploratory, and Preprocessing
    - Data source: https://www.kaggle.com/datasets/ritiksharma07/80-indian-cuisines-for-classification-projects
    - Running the script to preprocess data: rt_indian_data_processing.ipynb
2. Model Creation and Training, Hyperparamter Tunning to improve performance
    - For basic CNN and EfficientNet: run python3 shrabhat-munging-experimentation-llm.py
    - For RexNet150: run the script vynguyen_rexnet150.ipynb
    - For M-GCN and ADD-GCN: run the script test_model.ipynb
3. Model Evaluation and Prediction
    - The models were evaluated against their history of loss and accuracy over training epochs. The resulting models exhibited desired training and validation accuracy over 0.7 and a consistent decreasing trend in both training and validation loss.
    - Evaluation metrics included Mean Average Precision (mAP), Mean Average Recall (mAR), and Cross-Entropy as the loss function.
    - Actual and predicted labels are plotted on images for comparison.

## Results
- Through rigorous experimentation and hyperparameter tuning, we validated our models using against quantitative and qualitative evidence. Advanced architectures and precise hyperparameter tuning significantly improved model performance. In contrast, data augmentation did not show any notable benefits for model performance.

- Models like ADD-GCN and M-GCN demonstrated superior performance compared to basic CNN, RexNet150, and EfficientNet. These advanced architectures leverage CNNs for feature extraction and attention-driven transformers to capture complex patterns within the dataset. M-GCN's memory mechanisms enhanced its ability to learn intricate label relationships, while ADD-GCN's dynamic attention mechanisms captured nuanced, context-aware data representations.

- Ultimately, ADD-GCN emerged as the top performer due to its superior adaptation capabilities, effectively managing the complexity and variability of our dataset. Its ability to dynamically adjust the importance of nodes and edges in the graph allowed it to capture more detailed and contextually relevant information, leading to superior performance in image classification tasks.

## Limitation and Future Work
The model is trained and tested exclusively on Indian cuisine dishes, which may limit its generalization to other cuisines and introduce bias toward certain ingredients. To improve model performance and generalization, things can be done as followed:
- Incorporated with datasets from a wider variety of cuisines to improve model generalization.
- Exploring advanced graph-based and hybrid models to enhance performance.
- Developing real-time, user-friendly food recognition applications.

## Contributions
- Shravan Bhatnagar (sbhatnagar45@gatech.edu)
- K Raviteja Vadrevu (kvadrevu3@gatech.edu)
- Vy Nguyen (vnguyen374@gatech.edu)

