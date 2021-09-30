# EuroSATClassification
This model is trained on the [EuroSAT dataset](https://arxiv.org/abs/1709.00029) to classify the 64x64 images into 10 classes namely - 
1. AnnualCrop
2. Forest
3. HerbaceousVegetation
4. Highway
5. Industrial
6. Pasture
7. PermanentCrop
8. Residential
9. River
10. SeaLake

The CNN used is similar to [AlexNet](https://papers.nips.cc/paper/2012/hash/c399862d3b9d6b76c8436e924a68c45b-Abstract.html), with a dropout of 0.65 and 96 kernels instead of 64 in the first convolution layer.

The 27000 data samples were split into 20000 training samples and 7000 validation samples using a random split. The saved model classified the validation data with an accuracy of 96.4945%.

This model has been implemented using PyTorch Lightning.
