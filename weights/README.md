# Model description

This folder contains 2 trained models based on 'YOLO8s' and 'YOLO8s-seg' for localization and segemetaion tasks respectively.

## Usage

These models can be used to predict fracture in an X-Ray image. The following snippet can be run in the command line for prediction.

```shell
  yolo task=<segment/detect> mode=predict save=True model=<trained_model> conf=0.25 source=<target_image_source>
```

The prdiction results can be found inside
`.\run\<detect/segment>\predict`
