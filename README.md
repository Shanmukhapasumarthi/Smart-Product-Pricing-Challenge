##Problem Statement

In e-commerce platforms, determining the optimal price for products is crucial for business success and customer satisfaction.
Product pricing depends on multiple factors such as product description, brand, specifications, and product appearance.

The objective of this project is to build a machine learning model that can analyze product details and product images together to predict the optimal price of a product.

##The problem is broken into smaller parts:
1.Load product dataset containing text descriptions, image links, and prices
2.Clean and preprocess textual product information
3.Download product images using provided URLs
4.Extract meaningful features from both text and images
5.Combine all features into a single dataset
6.Train a regression model to predict product prices

##What I Have Done:
1.Cleaned and preprocessed the product data including text and price values
2.Converted product descriptions into TF-IDF numerical vectors
3.Downloaded product images and extracted deep features using a pretrained MobileNetV2 model
4.Combined text and image features and trained an XGBoost regression model for price prediction

