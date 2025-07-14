# 🌴 Tunisian Date Classification AI Project

## Project Overview

This project develops an advanced image classification system to identify and classify 11 different varieties of Tunisian dates using deep learning techniques. The system leverages Convolutional Neural Networks (CNNs) to distinguish between date varieties based on their unique visual characteristics.

## 🎯 Objectives

- Develop a high-performing CNN model for Tunisian date variety classification
- Implement advanced image processing and enhancement techniques
- Achieve robust model performance through cross-validation and data augmentation
- Provide explainable AI insights using LIME for model interpretability
- Support agricultural stakeholders with accurate date variety identification

## 📊 Dataset

**Source:** Deglet Nour Date Fruit Dataset 
**Classes:** 11 different Tunisian date varieties
**Size:** 300-473 images per class

### Date Varieties Included:
- Bessra
- Deglet Nour Dryer
- Deglet Nour Oily
- Deglet Nour Semi-Oily Treated
- Deglet Nour Semi-Dryer
- Alig
- Kenta
- Deglet Nour Oily Treated
- Deglet Nour Semi-Dryer Treated
- Deglet Nour Semi-Oily
- Deglet Nour

## 🔧 Technical Architecture

### Model Architecture
- **Input Layer:** 224x224x3 RGB images
- **Convolutional Layers:** Multiple Conv2D layers with ReLU activation
- **Pooling Layers:** Combination of AveragePooling2D and MaxPooling2D
- **Dense Layers:** Fully connected layers with dropout regularization
- **Output Layer:** 11-class softmax classification

### Image Enhancement Pipeline
1. **Resizing:** Standard 224x224 pixel dimensions
2. **Normalization:** Pixel value normalization for improved contrast
3. **Sharpening:** Convolutional filter for edge enhancement
4. **CLAHE:** Contrast Limited Adaptive Histogram Equalization for local contrast enhancement

## 🚀 Methodology

Following **CRISP-DM** methodology:

### 1. Business Understanding
- Define classification objectives and success criteria
- Identify stakeholder requirements (farmers, researchers, agricultural businesses)
- Establish model performance metrics

### 2. Data Understanding
- Analyze dataset structure and quality
- Explore class distribution and image characteristics
- Assess data relevance for classification task

### 3. Data Preparation
- Implement image enhancement pipeline
- Apply data augmentation techniques
- Normalize and preprocess images for model input

### 4. Modeling
- Build CNN architecture with optimized layers
- Implement stratified k-fold cross-validation (6 splits)
- Apply data augmentation for improved generalization

### 5. Evaluation
- Assess model performance using multiple metrics
- Generate classification reports and confusion matrices
- Compute ROC curves for multi-class evaluation

### 6. Deployment
- Implement explainable AI using LIME
- Provide model interpretability and transparency

## 📈 Performance Metrics

The model is evaluated using:
- **Accuracy:** Overall classification accuracy
- **Precision:** Class-specific precision scores
- **Recall:** Class-specific recall scores
- **F1-Score:** Harmonic mean of precision and recall
- **ROC-AUC:** Multi-class ROC curve analysis
- **Confusion Matrix:** Detailed classification performance visualization

## 🛠️ Key Features

### Data Augmentation
- Rotation (±20°)
- Shear transformation (0.2)
- Zoom (±10%)
- Horizontal flipping
- Nearest neighbor fill for missing pixels

### Cross-Validation
- Stratified K-Fold with 6 splits
- Maintains class balance across folds
- Ensures robust model validation

### Explainable AI (XAI)
- LIME implementation for local interpretability
- Visual explanation of model decisions
- Highlight important image regions for classification

## 🔍 Model Interpretability

The project implements **LIME (Local Interpretable Model-agnostic Explanations)** to provide:
- Visual explanations of individual predictions
- Identification of important image regions
- Transparency in model decision-making process
- Heatmap visualization of feature importance

## 📋 Requirements

```
tensorflow>=2.8.0
keras>=2.8.0
opencv-python>=4.5.0
matplotlib>=3.5.0
numpy>=1.21.0
pandas>=1.3.0
scikit-learn>=1.0.0
lime>=0.2.0
seaborn>=0.11.0
kagglehub>=0.1.0
```


## 📊 Results

The model achieves robust performance across all 11 date varieties with:
- High classification accuracy
- Balanced precision and recall scores
- Effective generalization through cross-validation
- Interpretable predictions through LIME analysis

## 🎯 Business Impact

This classification system enables:
- **Quality Control:** Automated variety identification for agricultural businesses
- **Supply Chain Optimization:** Accurate product categorization and inventory management
- **Research Support:** Tools for agricultural research and crop analysis
- **Market Differentiation:** Enhanced product identification for premium market positioning

## 👥 Development Team

**Released by:**
- Abed El Aziz Bouebsa


## 🔒 Confidentiality Notice

**Dataset Access:** The Deglet Nour Date Fruit Dataset used in this project is confidential and restricted to authorized personnel only. Access to the dataset requires proper authorization and is intended for sharing among approved team members and collaborators.

**Project Availability:** The project code, methodology, and implementation details are open for collaboration and sharing within the research community.

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

