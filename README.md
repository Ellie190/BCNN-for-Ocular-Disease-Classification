# BCNN-for-Ocular-Disease-Classification
**Adaptive Computation and Machine Learning Project:** Bayesian Convolutional Neural Network for Detection of Cataract Ocular Disease

## Project Overview 
- Built a Bayesian Convolutional Neural Network (BCNN) to classifying Cataract Images of patients
- A Standard Convolutional Neural Network was built as a benchmark model for performance comparison with the BCNN model
- Kaggle Data Name: Ocular Disease Recognition
- Evaluation metric: Accuracy
- Experiment 1: Tuning the number of neurons
- Experiment 2: Tuning the learning rate

## Workflow
![WorkFlow](https://github.com/Ellie190/BCNN-for-Ocular-Disease-Classification/blob/main/Images/workflow.png)

## Context
**Ocular Disease:** Ocular diseases are those that affect the eye health and vision in patients of all different ages. <br>
**Cataract:** A cataract is a dense, cloudy area that forms in the lens of the eye. A cataract begins when proteins in the eye form clumps that prevent the lens from sending clear images to the retina. The retina works by converting the light that comes through the lens into signals. Cataract  is one of the most prevalent ailments that can lead to blindness. 

**Why Bayesian Convolution Neural Network?** 
- Cataract diagnosis is not a simple classification/detection problem
- Uncertainty quantification plays an important role in model classifications due to the risks/stakes involved in incorrectly classifying a patient as not having cataract. 
- BCNN provides an opportunity to reason under uncertainty which is crucial in medical practice.
- BCNN enables the capturing of Aleatoric and Epistemic uncertainty
- `Aleatoric uncertainty` is the uncertainty that arises from the quality of the data
- `Epistemic uncertainty` is the uncertainty that arises from the model itself

## Resources 
**Python Version:** 3.9.7 <br>
**Main Python Packages:** numpy, pandas, sklearn, cv2, tensorflow, keras, seaborn, matplotlib, random, pickle <br>
**Python Packages:** See `requirements.txt` file <br>
**Kaggle Dataset:** https://www.kaggle.com/datasets/andrewmvd/ocular-disease-recognition-odir5k
**Install prerequisite libraries**
Download requirements.txt file

```
wget https://raw.githubusercontent.com/Ellie190/BCNN-for-Ocular-Disease-Classification/main/requirements.txt?token=GHSAT0AAAAAABSH6TIYTOF5IW6ILOXEC24UYVKCX4A
```

Pip install libraries
```
pip install -r requirements.txt
```


## BCNN Model Performance
- `Epochs:` 100, `Learning rate:` 0.001, `Accuracy:` 93.16%, `Validation Accuracy:` 92.50%
![BCNN Model Performance](https://github.com/Ellie190/BCNN-for-Ocular-Disease-Classification/blob/main/Images/bcnn_model_performance.png)

## BCNN Model Classifications Samples
- Cataract Patient Classification 
![BCNN Cataract Classification](https://github.com/Ellie190/BCNN-for-Ocular-Disease-Classification/blob/main/Images/bcnn_prediction1.png) <br>
- Cataract Patient Classification
![BCNN Cataract Classification](https://github.com/Ellie190/BCNN-for-Ocular-Disease-Classification/blob/main/Images/bcnn_prediction2.png) <br>
- Normal Patient Classification
![BCNN Normal Classification](https://github.com/Ellie190/BCNN-for-Ocular-Disease-Classification/blob/main/Images/bcnn_prediction3.png) <br>
- Normal Patient Classification
![BCNN Normal Classification](https://github.com/Ellie190/BCNN-for-Ocular-Disease-Classification/blob/main/Images/bcnn_prediction4.png)




