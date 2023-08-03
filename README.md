![Logo](DIETxPosome.jpg)

# Literature_mining_of_contaminants_in_food_groups
Literature mining of 96 contaminants in 72 foods from PubMed. This work is part of [DIETxPOSOME](https://i3a-laqv.pt/Projects_DIETxPosomePhone/Projects_DIETxPosomePhone/) project of [FOODinteract Research Team](https://i3a-laqv.pt/). The code used in this repository was adapted from [FoodMine](https://github.com/fhooton/FoodMine).

> **From data to insight: Exploring contaminants in different food groups with literature mining and machine learning techniques**
>
> **Abstract**
>
> Food remains a major source of human exposure to chemical contaminants that are unintentionally present in commodities globally, despite strict regulation. Scientific literature is a valuable source of quantification data on those contaminants in various foods, but manually summarizing the information is not practicable. In this review, literature mining and machine learning techniques were applied in 72 foods to obtain relevant information on 96 contaminants, including heavy metals, polychlorinated biphenyls, dioxins, furans, polycyclic aromatic hydrocarbons (PAHs), pesticides, mycotoxins, and heterocyclic aromatic amines (HAAs). The 11,723 data points collected from 254 papers from the last two decades were then used to identify the patterns of contaminants distribution. Considering contaminant categories, metals were the most studied globally, followed by PAHs, mycotoxins, pesticides, and HAAs. As for geographical region, the distribution was uneven, with Europe and Asia having the highest number of studies, followed by North and South America, Africa and Oceania. Regarding food groups, all contained metals, while PAHs were found in seven out of 12 groups. Mycotoxins were found in six groups, and pesticides in almost all except meat, eggs, and vegetable oils. HAAs appeared in only three food groups, with fish and seafood reporting the highest levels. The median concentrations of contaminants varied across food groups, with citrinin having the highest median value. The information gathered is highly relevant to explore, establish connections, and identify patterns between diverse datasets, aiming at a comprehensive view of food contamination.

## Setup
* See **Setup** section from [FoodMine](https://github.com/fhooton/FoodMine)

Run the [python notebooks](https://jupyter-notebook-beginner-guide.readthedocs.io/en/latest/) in the following order to replicate the process.
 - Paper_Screening_CRFS.ipynb
 - Paper_Ranking_CRFS.ipynb
   

## Files

#### Paper_Screening_CRFS.ipynb
Notebook to search through the PubMed database and filter out search results.

#### Paper_Ranking_CRFS.ipynb
Notebook to build a Machine Learning model to classify potential useful papers to later review manually.

#### Data
Folder that holds raw data from paper data collection.

#### Ranking
Folder that holds raw data from paper after Machine Learning classification.

#### Other files

* **pubmed_util.py**
Holds functions to interact with PubMed API for the purposes of our research.

* **filter.py**
Contains class Filter to filter out PubMed search results.

Select data files:

* (Apple/Cheese/Chicken/Corn_oil/Ginger/Mussel/Peanut/Potato/Soybean/Tomato/Wheat)_scoring.xlsx
Files that contain papers with potentially useful classification (0/1), used to train Machine Learning algorithm

* dict_CRFS.pkl
File that contains food name, food scientific name, and chemical compounds included in the study

## Authors
[Zita Martins](https://github.com/zitasamartins) - feel free to contact me!


## Acknowledgments

* [FoodMine](https://github.com/fhooton/FoodMine)
