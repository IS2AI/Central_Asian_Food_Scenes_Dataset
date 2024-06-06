# Central_Asian_Food_Scenes_Dataset
In this work, we propose the first Central Asia Food Scenes Dataset that contains 21,306 images with 69,856 instances across 239 food classes. To make sure that the dataset contains various food items, we took as a benchmark the ontology of Global Individual Food Tool developed by Food and Agriculture Organization (FAO) together with the World Health Organization (WHO). The dataset contains food items across 18 coarse classes: vegetables, baked flower-based products, cooked dishes, fruits, herbs, meat dishes, desserts, salads, sauces, drinks, dairy, fast-food, soups, sides, nuts, pickled and fermented food, egg product, and cereals. 

The dataset contains open source web-scraped images from the search engines (15,939 images) (i.e., Google, YouTube, and Yandex) and our own collected food images from everyday life (2,324 images). To additionally extend the number of instances of the underrepresented classes, we have scraped open-source videos and extracted frames at a rate one frame per second (3,043 images). The dataset has been checked and cleaned for duplicates using the Python Hash Image library. Furthermore, we have also filtered out images less than 30 kB in size and replaced them by performing additional iterative data scraping and duplicate check to make sure the high quality of the dataset.

Sample Food scenes annotated images are shown below. Figures illustrate annotated food scenes samples based on our annotation rules that we have followed to create the dataset: the liquid objects such as beverages and soups are annotated together with the dish itself (see upper image), solid food items are annotated without the plate, in case one class is located on top of another class the annotations are made as shown on lower image; in case one class is obscured by another class and the rest of the background class is not visible we highlight only the visible part (see `Salad leaves' class annotation on the lower image. 

<img src="https://github.com/IS2AI/Central_Asian_Food_Scenes_Dataset/blob/main/figures/protocol_1.png" width="800" height="700">
<img src="https://github.com/IS2AI/Central_Asian_Food_Scenes_Dataset/blob/main/figures/protocol_2.png" width="800" height="700">

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
