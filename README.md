# DWS-Loss: Distance-Weighted Sinkhorn Loss for Alzheimer’s Disease Classification

This repository holds the official source codes of the **DWS_Loss** (Distance-Weighted Sinkhorn Loss)  for the paper [Distance-Weighted Sinkhorn Loss for Alzheimer’s Disease Classification]()

```
@article {
}
```

### Abstract
Traditional loss functions such as cross-entropy loss often quantify the penalty for each mis-classified
training sample without adequately considering its distance from the target ground truth class distribution
in the feature space. Intuitively, the larger this distance is, the higher the penalty should be. With this
observation, we propose a penalty called Distance-Weighted Sinkhorn (DWS) loss. For each mis-classified
training sample (say, with predicted label A and true label B), its contribution to the DWS loss is defined
to be positively correlated to the distance the training sample needs to travel to reach the true distribution
of all the A samples. We implement a neural network with the DWS loss and apply it to a multi-class
diagnosis task on classifying Alzheimer’s disease (AD), Mild Cognitive Impairment (MCI), and Cognitively
Normal (CN) subjects using FDG-PET imaging data capturing glucose metabolism. Our empirical results
demonstrate that the proposed DWS framework outperforms the traditional neural networks with various
loss functions such as hinge loss, cross-entropy loss, and mean square error. In comparison with traditional
machine learning methods, such as SVM, logistic regression, and gradient boosting, the DWS method also
yields either comparable or better performances. These highly promising results suggest the tremendous
potential of the newly proposed DWS loss in solving multi-class classification problems in the fields of
biomedical informatics and data science.

### Data
The simulation data is named DWS_Simulation.csv. 
### Requirments
The implementation is based on Python and Pytorch. We provide our code using the Google Colab. All the relevant packages are installed within the Notebook. To run this file, one might need to access to a GPU for faster computation.
### Usage
Please run the cells one by one. We compare the proposed method with the cross entropy, cross entropy with logit activation and the focal loss. The evaluation metric is also shown in the code. Notice that if this is run on the local machine, please adjust the path of simulation data.


### Contacts

- [Zexuan Wang](mailto:zxwang@sas.upenn.edu) 
- [Li Shen](mailto:li.shen@pennmedicine.upenn.edu) 
