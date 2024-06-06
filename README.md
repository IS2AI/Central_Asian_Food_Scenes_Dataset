# Central_Asian_Food_Scenes_Dataset
This is the repository for the Central Asian Food Scenes Dataset

Central Asian Food Scenes Dataset (CAFSD) for food object detection contains 21,305 images across 239 food classes commonly consumed in Central Asia. The dataset contains manually collected real-life images, web-scraped images and frames extracted from different videos. Images have various resolution.
Figure below illustrates the samples and name for each class.

Sample Food scenes annotated images are shown below. 

<img src="https://github.com/IS2AI/Central_Asian_Food_Scenes_Dataset/blob/main/figures/statistics.png" width="800" height="900">

The dataset is unbalaced. The statistics across high-level 18 classes is shown on Figure below.

<img src="https://github.com/IS2AI/Central_Asian_Food_Scenes_Dataset/blob/main/figures/statistics.png" width="800" height="900">

# Dataset split across the folds

|Fold| Train| Valid| Test| 
|----|-----------------|-----------------|--------------------|
|images|17,046|2,084|2,176|
|instances|55,422|7,062|7,381|

# Download the dataset

The dataset can be downloaded using the link below. If there are some issues with the link, please, email us on issai@nu.edu.kz

https://issai.nu.edu.kz/wp-content/themes/issai-new/data/models/CAFD/CAFD.zip

# Training results

To illustrate the performance of different classification models on CAFD we have trained different models. We used the largest publicly available fine-grained dataset Food1K [[1]](#1) that contains 1,000 food classes to evaluate the performance of classifier with the 1,042 food categories.

<img src="https://github.com/IS2AI/Central_Asian_Food_Scenes_Dataset/blob/main/figures/table_results.png" width="1200" height="290">

# Pre-trained models

Pre-trained weights of the YOLOv8 model can be downloaded using these links:

## YOLOv8n: 
https://issai.nu.edu.kz/wp-content/themes/issai-new/data/models/CAFD/cafd_resnet152.pt

## YOLOv8s: 
https://issai.nu.edu.kz/wp-content/themes/issai-new/data/models/CAFD/cafd_resnet152.pt

## YOLOv8m: 
https://issai.nu.edu.kz/wp-content/themes/issai-new/data/models/CAFD/cafd_resnet152.pt

## YOLOv8l: 
https://issai.nu.edu.kz/wp-content/themes/issai-new/data/models/CAFD/cafd_resnet152.pt

## YOLOv8x: 
https://issai.nu.edu.kz/wp-content/themes/issai-new/data/models/CAFD/cafd_resnet152.pt



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
