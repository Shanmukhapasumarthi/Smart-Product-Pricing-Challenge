# Smart Product Pricing Challenge

## Problem Statement

In e-commerce platforms, determining the optimal price for products is crucial for business success and customer satisfaction.  
Product pricing depends on multiple factors such as product description, brand, specifications, and product appearance.

The objective of this project is to build a machine learning model that can analyze product details and product images together to predict the optimal price of a product.

### The problem is broken into smaller parts:

1. Load product dataset containing text descriptions, image links, and prices  
2. Clean and preprocess textual product information  
3. Download product images using provided URLs  
4. Extract meaningful features from both text and images  
5. Combine all features into a single dataset  
6. Train a regression model to predict product prices  

---

## What I Have Done

- Preprocessed and cleaned product text data and pricing values  
- Converted product descriptions into numerical features using TF-IDF vectorization  
- Downloaded product images and extracted deep visual features using pretrained MobileNetV2  
- Combined text and image features and trained an XGBoost regression model for price prediction  

---

## How to Run the Project

### Step:1 Run the requirements.txt

```bash
pip install -r requirements.txt
```
---
### Step 2: Run the notebool
---

###  Model Architecture
Text Feature Extraction

• Cleaned product descriptions
• Applied TF-IDF vectorization
• Used unigrams and bigrams
• Limited vocabulary size to 10,000 features

Image Feature Extraction

• Downloaded images from URLs
• Resized to 224 x 224
• Used pretrained MobileNetV2 convolutional neural network
• Removed classification layer to extract deep features

Final Prediction Model

• Combined text and image features
• Used XGBoost regression model for predicting prices

---

### Training Details
Text features generated using TF-IDF (maximum 10,000 features)
Image features extracted using pretrained MobileNetV2
Regression model used: XGBoost
Hyperparameters:
n_estimators = 200
learning_rate = 0.1
max_depth = 6
Evaluation metric used:
SMAPE (Symmetric Mean Absolute Percentage Error)

---

### Limitations of the project
• Image download may fail for broken or missing URLs
• Pretrained CNN was not fine-tuned on product images
• TF-IDF does not capture deep semantic meaning of text
• No separate validation set used
• Model performance depends heavily on data quality
• High memory usage when handling large TF-IDF matrices

---

### Conclusion
This project demonstrates a multimodal machine learning approach to predict product prices by combining text descriptions and product images.
By integrating NLP techniques, deep visual feature extraction, and a powerful regression model, the system can effectively learn pricing patterns.

---
