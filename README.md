# FracAtlas: A Dataset for Fracture Classification, Localization and Segmentation on Musculoskeletal Radiographs

The majority of the existing X-Ray datasets are either very small in size to be used in training machine learning models or lack proper annotation to be used in localization and segmentation. This creates a limitation while comparing different state-of-the-art (SOTA) methods as each study uses its own set of data that is not made public. It also hinders the development of machine-learning algorithms for classification, localization and segmentation. In this work, we introduce a new dataset of more than 14,000 X-Ray scans which was collected from 3 major hospitals in Bangladesh. From this raw data, we isolated 4,083 images which have been manually annotated for classification, localization and segmentation of bone fractures with the help of 2 expert radiologists and later validated by a medical officer. Each scan in the dataset was independently labeled by both radiologists and later confirmed by the medical officer. The annotation was done with the help of makesense.ai, an open-source labeling platform. All the scans are available in JPG format along with proper annotations.

The dataset can be downloaded from [FigShare](https://doi.org/10.6084/m9.figshare.22363012). By downloading the dataset users agree that they will not share the data and that the dataset can be used for scientific research and educational purposes only according to [DUA](https://www.physionet.org/about/licenses/physionet-credentialed-health-data-license-150/).

## Code
There are 2 notebooks in the root folder called 'Train_8s.ipynb' and 'Pred_8s.ipynb'. 'Train_8s.ipynb' is used to train 2 models of 'YOLO8s_seg' and 'YOLO8s' variant targeted toward segementation and localization tasks respectively. 'Pred_8s.ipynb' is used to generate predictions out of the 2 aforementioned models and view the results.

## Citation
If [FracAtlas](https://doi.org/10.6084/m9.figshare.22363012) dataset is used in your work, the authors must cite the [original paper]() as follows:
```code
  bibtext here
```
We also encourage such authors to release their code and models, which will help the community to reproduce experiments and to boost the research in the field of medical imaging.
