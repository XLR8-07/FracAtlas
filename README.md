# FracAtlas: A Dataset for Fracture Classification, Localization and Segmentation on Musculoskeletal Radiographs

The majority of the existing X-Ray datasets are either very small in size to be used in training machine learning models or lack proper annotation to be used in localization and segmentation. This creates a limitation while comparing different state-of-the-art (SOTA) methods as each study uses its own set of data that is not made public. It also hinders the development of machine-learning algorithms for classification, localization and segmentation. In this work, we introduce a new dataset of more than 14,000 X-Ray scans which was collected from 3 major hospitals in Bangladesh. From this raw data, we isolated 4,083 images which have been manually annotated for classification, localization and segmentation of bone fractures with the help of 2 expert radiologists and later validated by a medical officer. Each scan in the dataset was independently labeled by both radiologists and later confirmed by the medical officer. The annotation was done with the help of makesense.ai, an open-source labeling platform. All the scans are available in JPG format along with proper annotations.

The dataset can be downloaded from [FigShare](https://doi.org/10.6084/m9.figshare.22363012).

## Code
There are 2 notebooks in the root folder called 'Train_8s.ipynb' and 'Pred_8s.ipynb'. 'Train_8s.ipynb' is used to train 2 models of 'YOLO8s_seg' and 'YOLO8s' variants targeted toward segmentation and localization tasks respectively. 'Pred_8s.ipynb' is used to generate predictions out of the 2 aforementioned models and view the results.

## Citation
If [FracAtlas](https://doi.org/10.6084/m9.figshare.22363012) dataset is used in your work, the authors must cite the [original paper](https://rdcu.be/diAK9) as follows:
```code
  @article{Abedeen_2023,
	title        = {{FracAtlas}: A Dataset for Fracture Classification, Localization and Segmentation of Musculoskeletal Radiographs},
	author       = {Iftekharul Abedeen and Md. Ashiqur Rahman and Fatema Zohra Prottyasha and Tasnim Ahmed and Tareque Mohmud Chowdhury and Swakkhar Shatabda},
	year         = 2023,
	month        = {aug},
	journal      = {Scientific Data},
	publisher    = {Springer Science and Business Media {LLC}},
	volume       = 10,
	number       = 1,
	doi          = {10.1038/s41597-023-02432-4},
	url          = {https://doi.org/10.1038%2Fs41597-023-02432-4}
}
```
We also encourage such authors to release their code and models, which will help the community to reproduce experiments and to boost research in the field of medical imaging.
