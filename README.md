# Data Science Case Studies

picture here

## What is it?
This is a repo for data anaylsis and ML models for several subprojects on the advertising industry, auto industry, housing market, the Boston Housing market, and Austalian weather. 

This repo also includes subprojects that explore using various types of models, optimizers, and loss functions for the classic MNIST dataset, signal processing, and predicting/recognizing protein structures.

---


## Table of Contents

- [Advertising](#advertising)
- [Auto](#auto)
- [Auto Regression Case Study](#auto-regression-case-study)
- [Boston](#boston)
- [Housing](#housing)
- [MNIST](#mnist)
- [Protein Stucture](#protein-stucture)
- [Signals](#signals)


## Advertising
- Analyzes a dataset of 200 samples, focusing on TV, Radio, and Newspaper advertising budgets along with sales figures.
- Data loaded from Google Drive using pandas for analysis.
- Explores dataset statistics and distributions.
- Utilizes kernel density plots to visualize Gaussian distribution of features and sales.
- Identifies key relationships between advertising channels (TV, Radio, Newspaper) and sales.
- Provides valuable insights for marketing strategies.



## Auto
- Utilizes pandas, numpy, statsmodels, matplotlib, and seaborn for data analysis and visualization.
- Loads data from Google Drive, handles data cleaning, and converts horsepower values.
- Analyzes dataset with 9 features and 397 samples, exploring distributions and relationships.
- Identifies strong negative correlations with mpg for features like cylinders, displacement, horsepower, and weight.
- Visualizes correlations using a heatmap, revealing significant relationships.
- Prepares for applying single linear regression to predictors for in-depth analysis.


## Auto Regression Case Study
- **Melbourne Temperature Dataset** 
  - Explored and forecasted minimum daily temperatures (1981-1990).
  - Used rolling mean, lag plots, and AR modeling for analysis.
- **Sine Wave Modeling**
  - Generated a 10 Hz sine wave and predicted using AR and RNN models.
  - Experimented with scaling, shifting, and noise addition.
- **Summary**
  - Applied AR and RNN models effectively to diverse time series datasets.


## Housing
- Explored various neural network configurations for the housing dataset regression problem to optimize model performance.
- **Best Configuration:** Two hidden layers yielded the best results with a **Test RMSE of 3.96**.
- **Optimizers:** Adam optimizer outperformed others, coupled with Mean Squared Error (MSE) loss.
- For similar regression tasks, consider using a neural network with 2 hidden layers and the Adam optimizer with MSE loss.
- Experimentation on different datasets can further validate these findings.
- **Frameworks:** TensorFlow, Keras
- **Techniques:** Early stopping, dataset normalization



## MNIST
- Built upon the existing MNIST notebook, experimenting with custom loss functions, optimizers, and CNN architectures to optimize performance for the MNIST dataset.
- **Adamax:** Achieved the best accuracy of **95.97%** in 10 epochs.
- **Optimizers Tested:** Adamax, SGD, RMSprop. Adamax outperformed others.
- **Best Loss Function:** `sparse_categorical_crossentropy` worked best for classification tasks.
- Other tested loss functions: `mse`, `categorical_hinge`, `huber_loss`. None performed as well as `sparse_categorical_crossentropy`.
- **CNN Architectures:** Experimented with different architectures including variations in pooling layers and activation functions.
- **Simpler Architectures:** Even simplified architectures with fewer layers maintained high accuracy, indicating efficiency in model design.
- **Optimizers:** Use Adamax optimizer for efficient and accurate training on MNIST.
- **Loss Function:** Prefer `sparse_categorical_crossentropy` for classification tasks.
- **Model Complexity:** Simple CNN architectures can be highly effective, reducing training time without compromising accuracy.
- **Frameworks:** TensorFlow, Keras
- **Techniques:** Custom loss functions, different optimizers, CNN architecture variations


## Protein Stucture
- This project contains Python code demonstrating the prediction of protein secondary structures using Recurrent Neural Networks (RNNs). 
- The dataset comprises 10k amino acid sequences and their corresponding secondary structures (helix, sheet, coil).
- The implemented models include Simple RNN, LSTM, GRU, as well as combinations such as LSTM-LSTM, LSTM-GRU, and Bidirectional LSTM.