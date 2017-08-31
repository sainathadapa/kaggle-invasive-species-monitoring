This repository contains my personal code for the Kaggle competition - [Invasive Species Monitoring](https://www.kaggle.com/c/invasive-species-monitoring/overview). Leaderboard score for the best submission was 0.99553. And as of 31st August 2017, the Leaderboard position was 6th.

Description:
- `01-create-validation-set.ipynb`: Divide the entire training dataset into training and validation datasets.
- `02-vgg.ipynb`: Finetunes the Vgg model (with Imagenet weights), for the current dataset.
- `04-inception.ipynb`: Finetunes the InceptionV3 model (with Imagenet weights), for the current dataset.
- `05-more-vgg-finetuning.ipynb`: Starting with the weights from `02-vgg.ipynb`, all the layers of the Vgg model are finetuned in here.
- `06-resnet.ipynb`: Finetunes the ResNet50 model (with Imagenet weights), for the current dataset.
- `07-inception-class-weights.ipynb`, `08-resnet-class-weights.ipynb` and `09-vgg-class-weights.ipynb`: As the dataset is imbalanced, training the models a little bit more, this time with class weights specified. Also, tracking the AUC after each epoch.
- `10-ensemble.ipynb`: Ensemble model
