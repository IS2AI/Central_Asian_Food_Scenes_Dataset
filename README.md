# Central_Asian_Food_Scenes_Dataset
This is the repository for the Central Asian Food Scenes Dataset

Central Asian Food Scenes Dataset (CAFSD) for food object detection contains 21,305 images across 239 food classes commonly consumed in Central Asia. The dataset contains manually collected real-life images, web-scraped images and frames extracted from different videos. Images have various resolution.
Figure below illustrates the samples and name for each class.

<img src="https://github.com/IS2AI/Kazakh-Food-Dataset/blob/main/figures/samples.png" width="750" height="700">

The dataset is unbalaced. The statistics across all 42 classes is shown on Figure below.

<img src="https://github.com/IS2AI/Kazakh-Food-Dataset/blob/main/figures/stats_plot.png" width="500" height="600">

# Download the dataset

The dataset can be downloaded using the link below. If there are some issues with the link, please, email us on issai@nu.edu.kz

https://issai.nu.edu.kz/wp-content/themes/issai-new/data/models/CAFD/CAFD.zip

# Pre-trained models

To illustrate the performance of different classification models on CAFD we have trained different models. We used the largest publicly available fine-grained dataset Food1K [[1]](#1) that contains 1,000 food classes to evaluate the performance of classifier with the 1,042 food categories.

<img src="https://github.com/IS2AI/Central_Asian_Food_Scenes_Dataset/blob/main/figures/table_results.png" width="500" height="600">

Pre-trained model weights of the best performing models: ResNet152 on KFD and EfficientNet-b4 on Food1K+KFD can be downloaded using these links:

## ResNet152 trained on CAFD: 

https://issai.nu.edu.kz/wp-content/themes/issai-new/data/models/CAFD/cafd_resnet152.pt

## EfficientNet-b4 trained on Food1K+CAFD:

https://issai.nu.edu.kz/wp-content/themes/issai-new/data/models/CAFD/food1k_kfd_efficientnet.pt

## Model training and testing

To train and test using pre-trained models use train.py and test.py files. 

## References
<a id="1">[1]</a> 
Min, Weiqing and Wang,  Zhiling (2021). 
Large Scale Visual Food Recognition. 
arXiv.

# In case of using our dataset and/or pre-trained models, please cite our work:
```
@Article{nu15071728,
AUTHOR = {Karabay, Aknur and Bolatov, Arman and Varol, Huseyin Atakan and Chan, Mei-Yen},
TITLE = {A Central Asian Food Dataset for Personalized Dietary Interventions},
JOURNAL = {Nutrients},
VOLUME = {15},
YEAR = {2023},
NUMBER = {7},
ARTICLE-NUMBER = {1728},
URL = {https://www.mdpi.com/2072-6643/15/7/1728},
ISSN = {2072-6643}
}
```
