
# Alzheimer's Detection 

The accurate diagnosis of Alzheimer's disease (AD) plays an important role in patient treatment, especially at the disease's early stages, because risk awareness allows the patients to undergo preventive measures even before the occurrence of irreversible brain damage. AD can be diagnosed-but not predicted-at its early stages, as prediction is only applicable before the disease manifests itself. Deep Learning (DL) has become a common technique for the early diagnosis of AD.

By using State-of-the-Art alogorithm(SOTA) we are detecting the Alzheimer's from the MRI images.
State-of-the-art (SOTA) DNNs are the best models you can use for any particular task. A DNN can be identified as SOTA based on its accuracy, speed, or any other metric of interest. However, in most computer vision areas, there is a trade-off between these metrics. That is, one can have a very fast DNN but its accuracy isn’t up to the mark. Other times, we might be able to build a model with good performance metrics but it would lack the required latency or throughput across various tasks, such as image classification and detection.
## DataSet

The data consists of MRI images. The data has four classes of images both in training as well as a testing set:

* Mild Demented
* Moderate Demented
* Non Demented
* Very Mild Demented
Dataset consists of two files - Training and Testing both containing a total of around ~5000 images each segregated into the severity of Alzheimer's

Download the dataset from : https://www.kaggle.com/datasets/tourist55/alzheimers-dataset-4-class-of-images
## Approach

RESNET50 and VGG16 these two SOTA are used to build the model.

RESNET50 & VGG16 : These are convolutional neural network that is 50 layers deep in case of RESNET50 and 19 layer deep in case of VGG19. You can load a pretrained version of the network trained on more than a million images from the ImageNet database. The pretrained network can classify images into 1000 object categories, here we pre trained to our model to classify into four categories.Early stopping methodology is used in model to prevent from over-fitting.


## Deployment

Deployment is done using Streamlit
( refer : https://docs.streamlit.io/ )
```bash
  streamlit run Alzheimers.py 
```

