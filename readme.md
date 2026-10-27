# Fault Diagnosis Model Based on 1DCNN-Informer+MATT Fusion

Preface
This issue introduces a classification model based on FFT+VMD preprocessing, 1DCNN-Informer dual-route feature extraction in parallel, and multi-head attention fusion. It has achieved significant results in fault diagnosis tasks!
1. Introduction to the Model and Innovation Points
1.1 Model Introduction
● Dataset: CWRU West Reserve University Bearing Dataset
● Environment Framework: Python 3.9, PyTorch 1.8 and above can be run.
● Accuracy: 100% on the test set.
● Usage Object: Paper requirements, graduation design requirements.
● Code Guarantee: The code comments are detailed and ready to run.
\t\tNote:
(1) We also offer comprehensive model explanations (for learning network architecture) and parameter tuning guidance! For students in need of graduation projects or writing small papers, this is a must-see. The modules are rich, innovative, and boast superior performance!
(2) Supplementary instructional videos, further optimization and innovative improvement ideas!
1.2 Innovation Points Introduction
Innovation 1: Preprocessing
Combined with the Fast Fourier Transform (FFT) and Variational Mode Decomposition (VMD), signal time-frequency and domain features can be extracted, which can reveal multi-scale features in fault signals.
(1) Preprocessing - FFT:
FFT is a widely used method for frequency domain analysis, which converts signals from the time domain to the frequency domain and obtains the signal's spectrum information. Through FFT, we can acquire the energy distribution of signals at different frequencies, thereby understanding the frequency components of the signals. However, FFT only provides the spectrum information of a signal at a certain moment, unable to reflect the change of the signal over time.
(2) Preprocessing - VMD:
To address this issue, Variational Mode Decomposition (VMD) can be introduced. VMD is a mode decomposition method based on signal adaptation, which can decompose the signal into a series of mode functions, each representing the characteristics of the signal at different scales. Through VMD, we can obtain the time-domain feature information of the signal at different scales.
Innovation 2: Dual-Branch Feature Extraction Parallel Network
(1) Design of dual-branch structure:
After preprocessing, the signal is processed through two parallel feature extraction branches to capture different features of the signal:
1DCNN branch: The one-dimensional convolutional neural network (1DCNN) is used to process the time-series signal after FFT+VMD preprocessing, focusing on capturing local temporal features. The sliding of convolution kernels achieves translation invariance, enhancing the ability to recognize local patterns.
Informer branch: The Informer encoder architecture is used to process the global features of the signal, especially suitable for modeling long sequence data, and can better capture the sequential dependencies and global patterns of the signal.
(2) Advantage of parallel processing:
The two branches can perform feature extraction simultaneously, independent but complementary. The 1DCNN focuses on short-term local features, while the Informer covers long-term dependencies and global features. Through this parallel processing approach, it achieves comprehensive capture of the signal's multi-scale and multi-faceted features.
Innovation 3: Multi-Head Attention Mechanism for Feature Fusion
(1) Multi-Head Attention mechanism for feature fusion:
Use a multi-head attention mechanism to fuse features from different branches. Each attention head can be considered as an extractor, focusing on different parts or aspects of the features.
The multi-head attention mechanism calculates the correlation weights between features and dynamically adjusts the importance of features to achieve weighted fusion of features. This mechanism not only enhances the expressiveness of features but also strengthens the model's robustness against noise and interference by focusing on important features.
(2)Advantages:
1.1 The use of multi-head attention mechanism enhances the hierarchical and diverse features of the fused features, which is conducive to improving the accuracy and generalization ability of classification models.
1.2 It can better capture the subtle features and pattern changes of fault signals when processing complex signals, thereby enhancing the accuracy and reliability of fault diagnosis.
2 Preprocessing of Bearing Fault Data
2.1 Import Data
Refer to previous articles for preprocessing of fault 10 classification, using the Case Western Reserve University bearing data 10 classification dataset:
train_set, val_set, test_set are divided into training set, validation set, and test set in a ratio of 7:2:1, and finally save the data.
The above figure shows the reading form of the data and the preprocessing idea.
2.2 Fault FFT Transform Visualization
2.3 Fault VMD Decomposition Visualization
2.4 Feature Preprocessing Dataset Production for Fault Data
3 Bearing Fault Diagnosis Model Based on 1DCNN-Informer+MATT
3.1 Set parameters and train the model
The model has significant classification effects, with an accuracy of 100% after 50 epochs, and Fast Fourier Transform (FFT) and Variational Mode Decomposition (VMD) can effectively mine multi-scale features from the signal. The 1DCNN-Informer+MATT parallel innovation model can fully extract spatial and temporal features of bearing fault signals, converges quickly, performs excellently, has high precision, and can extract important features from the frequency domain and time domain characteristics of the fault signal, making the effect obvious, with high innovation!
3.2 Model Evaluation
Accuracy, Precision, Recall, F1 Score
Fault very class confusion matrix:
3.3 Other Visualization Figures:
(1) Classification Label Visualization
(2) Original Data t-SNE Feature Visualization
1. After model training, t-SNE feature visualization:
  
Click to download: Complete original data and Python code
Previously excellent content:
Python bearing fault diagnosis | From beginner to publication
Python bearing fault diagnosis (14) High innovation fault recognition model
SCI 1st-class high-innovation bearing fault diagnosis model!
Attention modification | Super strong bearing fault diagnosis model!
Bearing fault diagnosis based on K-NN + GCN
27 bearing fault diagnosis models | The most cost-effective family set online
Based on KAN, KAN convolutional bearing fault diagnosis model
Time-frequency graph update | Bearing fault diagnosis based on visual top conference + time-frequency graph
Fault diagnosis | Code explanation + live courses, hotly ongoing!
Rapid paper release | Based on 2D-SWinTransformer+1D-CNN-SENet parallel fault diagnosis model
Position encoding demystification | Detailed explanation of Transformer's positional encoding Positional Encoding
Resource sharing | Intelligent fault diagnosis and prediction based on graph neural networks
Innovation point | Fault diagnosis model based on Fast Fourier Transform Convolution (FFC)
Code open-source! | Parallel domain adversarial graph convolution network fault diagnosis under variable conditions
More than thirty open datasets | No more worries about datasets for fault diagnosis!
Fault diagnosis | A must-have for postgraduates and second-year students in research papers!!!
Super strong! Top-level conference innovation integration! Parallel classification network based on 2D-SWinTransformer
Multimodal - fault diagnosis | Large kernel convolution opens a new era in vision!
Transformer structure advantage, How much attention do you need?
Fault diagnosis | A small innovation: feature extraction + KAN classification
Superior! Directly write in Zone 1! SSA+Informer-SENet Fault Diagnosis Model
Fault Diagnosis | Collection of Signal Noise Reduction Algorithms
New additions to the GAT, SGCN, and GIN classification models for fault diagnosis through convolutional neural networks.
Bearing Lifespan Prediction Kit is here!
Cannot miss out! A major update on fault diagnosis and time-frequency image classification!
Recommended journals for intelligent fault diagnosis and lifespan prediction.
Fault Diagnosis directly written in Zone 1, parallel diagnostic model with graph convolution and BiGRU-Attention.
END

## Images

<!-- PAYMENT_BLOCK -->

## Get this dataset

- Payment link (Stripe): [Buy now](https://buy.stripe.com/3cs8yP7sY87d0vu9AB)
- Payment QR code: ![Payment QR code](pay.png)

<!-- /PAYMENT_BLOCK -->
