# Technical validation of FracAtlas Dataset

Here, 2 note books `train_8s_localization.ipynb` and `train_8s-seg_Segmentation.ipynb` are used to train 2 models called 'YOLO8s' and 'YOLO8s-seg' respectively. 

The model details are listed below.

| Model| size<br><sup>(pixels) | mAP<sup>val<br>50-95 | Speed<br><sup>CPU ONNX<br>(ms) | Speed<br><sup>A100 TensorRT<br>(ms) | params<br><sup>(M) | FLOPs<br><sup>(B) |
| ---- | --- | --- | --- | --- | --- | --- |
| [YOLOv8s](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8s.pt) | 640| 44.9| 128.4| 1.20| 11.2| 28.6|
| [YOLOv8s-seg](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8s-seg.pt) | 640| 44.6| 36.8| 155.7| 1.47| 11.8| 42.6|

## System setup

Pip install the ultralytics package including all [requirements](https://github.com/ultralytics/ultralytics/blob/main/requirements.txt) in a [**Python>=3.7**](https://www.python.org/) environment with [**PyTorch>=1.7**](https://pytorch.org/get-started/locally/).

```bash
pip install ultralytics
```

## Training 
To start training the files must be arranged in the following folder structure. 

    root
    ├── ...
    ├── notebooks
    │   ├── Prediction_8s.ipynb
    │   ├── Train_8s.ipynb
    │   ├── dataset                         # Contains the dataset
    |   |   ├── data.yaml                   # Describes the dataset
    |   |   ├── train
    |   |   |   ├── images                  # contains all the training images
    |   |   |   |   └── ... 
    |   |   |   ├── labels                  # contains all the training labels
    |   |   |   |   └── ... 
    |   |   ├── Valid
    |   |   |   ├── images                  # contains all the validation images
    |   |   |   |   └── ... 
    |   |   |   ├── labels                  # contains all the validation labels
    |   |   |   |   └── ... 
    │   └── ...                 
    └── ...                                 # etc.

After training models are save in `.\run\<detect/segment>\train\weights`

## Test
The best models can be accessed from the aforementioned location and used in the `Prediction_8s.ipynb`.