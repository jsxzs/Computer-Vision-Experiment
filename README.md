# Computer-Vision-Experiment
Computer Vision, CS, HUST, 2023

## Exp1: Regression

Design a feedforward neural network to do regression task. Please refer to [exp1](exp1\上机实验一.docx) for more details.

- A Simple Fully Connected Neural Network

![](images\exp1\train_val_loss.png)

- Different Hidden Layer Numbers

  ![](images\exp1\diff_layer_num.png)

- Different Neuron Numbers

  ![](images\exp1\diff_neuron_num.png)

- Different Activation Functions

  ![](images\exp1\diff_activation.png)

## Exp2: CIFAR-10 Image Classification Based On CNN

Please refer to [exp2](exp2) for more details.

Download work_dir [here](https://drive.google.com/drive/folders/1O2jsRZCIPPoS6uzmSbIFIsVM_SGvNybJ?usp=share_link), which contains training logs, json files and .pth files.

Folder structure:

```
Computer-Vision-Experiment\exp2
│ command.txt
│ exp2_cifar10.ipynb
├─configs       
├─datasets
│  └─cifar-10-batches-py
│          batches.meta
│          data_batch_1
│          data_batch_2
│          data_batch_3
│          data_batch_4
│          data_batch_5
│          readme.html
│          test_batch      
├─modules
├─tools
└─work_dir
    ├─resnet
    |  ├─resnet18
    │  ├─resnet34
    │  ├─resnet50
    │  └─resnet9
    └─vgg
        ├─vgg11_bn    
        ├─vgg13_bn
        ├─vgg16_bn
        └─vgg19_b
```

Results:

|          | Total Accuracy | plane  | car    | bird   | cat    | deer   | dog    | frog   | horse  | ship   | truck  |
| -------- | -------------: | :----: | ------ | ------ | ------ | ------ | ------ | ------ | ------ | ------ | ------ |
| Resnet9  |         90.56% | 91.8%  | 95.90% | 86.60% | 80.40% | 91.40% | 85.80% | 93.30% | 91.50% | 94.90% | 94.00% |
| VGG11_bn |         90.42% | 93.00% | 92.50% | 85.70% | 84.20% | 89.80% | 82.40% | 93.30% | 93.50% | 95.90% | 93.90% |
| VGG13_bn |         92.18% | 93.70% | 96.10% | 91.10% | 79.50% | 93.60% | 87.30% | 94.70% | 95.60% | 95.40% | 94.80% |
| VGG16_bn |         91.91% | 94.90% | 96.70% | 90.40% | 81.70% | 95.10% | 86.70% | 93.60% | 92.50% | 92.50% | 95.00% |
| VGG19_bn |         91.81% | 93.10% | 97.20% | 88.40% | 85.40% | 92.30% | 87.10% | 91.40% | 94.00% | 95.00% | 94.20% |
| Resnet18 |         90.76% | 93.20% | 95.20% | 84.50% | 76.30% | 91.80% | 89.60% | 93.50% | 93.90% | 95.60% | 94.00% |
| Resnet34 |         90.13% | 91.90% | 95.80% | 84.40% | 77.50% | 93.30% | 83.20% | 92.60% | 94.20% | 95.00% | 93.40% |
| Resnet50 |         91.41% | 93.20% | 95.50% | 88.20% | 80.50% | 92.30% | 85.50% | 96.20% | 92.70% | 95.60% | 94.40% |



- A Simple Resnet (Resnet9)

  <center>![](images\exp2\resnet9.png)<center>

  ![](images\exp2\resnet9_train.png)

- VGG11_bn

  ![](images\exp2\vgg11_bn_train.png)

- VGG13_bn

  ![](images\exp2\vgg13_bn_traint.png)

- VGG16_bn

  ![](images\exp2\vgg16_bn_train.png)

- VGG19_bn

  ![](images\exp2\vgg19_bn_train.png)

- Compare VGG

  ![](images\exp2\vgg.png)

- ResNet13

  ![](images\exp2\resnet13_train.png)

- ResNet34

  ![](images\exp2\resnet34_train.png)

- ResNet50

  ![](images\exp2\resnet50_train.png)

- Compare ResNet

  ![](images\exp2\resnet.png)

