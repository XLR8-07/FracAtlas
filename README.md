# MLBFR: A Dataset for Fracture Classification, Localization and Segmentation in Musculoskeletal Radiographs

The majority of the existing X-Ray datasets are either very small in size to be used in training machine learning models or lack proper annotation to be used in localization and segmentation. This creates a limitation while comparing different state-of-the-art (SOTA) methods as each study uses its own set of data that is not made public. It also hinders the development of machine-learning algorithms for classification, localization and segmentation. In this work, we introduce a new dataset of more than 14,000 X-Ray scans which was collected from 3 major hospitals in Bangladesh. From this raw data, we isolated 4,083 images which have been manually annotated for classification, localization and segmentation of bone fractures with the help of 2 expert radiologists and later validated by a medical officer. Each scan in the dataset was independently labeled by both radiologists and later confirmed by the medical officer. The annotation was done with the help of makesense.ai, an open-source labeling platform. All the scans are available in JPG format along with proper annotations.

The dataset can be downloaded from [FigShare](). By downloading the dataset users agree that they will not share the data and that the dataset can be used for scientific research and educational purposes only according to [DUA](https://vindr.ai/wp-content/uploads/2022/04/DUA-BodypartXR.pdf).

## Code
The relevant code to this dataset can be found within 2 folders ‘Utility’ and ‘Technical Validation’. The details regarding files inside those folders can be found within. The ‘Utility’ contains notebooks used in the development of the dataset and in ‘Technical Validation’ the codes used for testing the usability of the dataset for Segmentation and Localization can be found.

## Citation
If [MLBFR]() dataset is used in your work, the authors must cite the [original paper]() as follows:
```code
  bibtext here
```
We also encourage such authors to release their code and models, which will help the community to reproduce experiments and to boost the research in the field of medical imaging.
