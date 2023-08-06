<div align="center">
<h2>Violence Detection Using YOLOv8 - Towards Automated Video Surveillance and Public Safety</h2>
</div>

</br>

### Title:

- Violence Detection Using YOLOv8: Towards Automated Video Surveillance and Public Safety

### Team-mates:

- [Md. Alahi Almin Tansen](https://github.com/aatansen)
- [Umayer Mohammad Affan](https://github.com/um-affan18)
- [Afruja Sultana Muniya](https://github.com/Muniyasultana111)
- [Md. Delower Hosen](https://github.com/DelowerHossain1)

### Supervisor:

- [Sovon Chakraborty](https://scholar.google.com/citations?user=B_jBQo0AAAAJ)

### Selected Dataset:

- Custom training dataset : [Roboflow Dataset](https://universe.roboflow.com/shah-xxxqs/violence-3h8pw)
    - Total = `2834 images`
        - Train = `1969 images`
        - Valid = `575 images`
        - Test = `290 images`
- Video dataset: [Kaggle Dataset](https://www.kaggle.com/datasets/mohamedmustafa/real-life-violence-situations-dataset)
    - Total = `2000 videos`
        - Non-violence = `1000 videos`
        - Violence = `1000 videos`

### Selected model

- [Yolov8](https://github.com/ultralytics/ultralytics)
- [Some CNN models](https://keras.io/api/applications/)
- [Yolo-NAS](https://github.com/Deci-AI/super-gradients)

### [Update 01](https://github.com/aatansen/Violence-Detection-Using-YOLOv8-Towards-Automated-Video-Surveillance-and-Public-Safety/tree/main/Update%2001)

- Model used `YOLOv8s`
- Number of epochs  = `25`
- Batch size = `16`
- Total training time = `0.255 hours`
- Confidence threshold = `0.25`
- Prediction on videos  = `10 videos`

### [Update 02](https://github.com/aatansen/Violence-Detection-Using-YOLOv8-Towards-Automated-Video-Surveillance-and-Public-Safety/tree/main/Update%2002)

As advised by the supervisor we used some CNN models and Yolo-NAS model and compare each of those models.

CNN models we used:

- VGG16
- VGG19
- ResNet152V2
- InceptionV3
- MobileNetV2
- DenseNet201

CNN models:

- Number of epochs  = `25`
- Batch size = `32`
- Loss function used = `smooth_l1_loss`
- Intersection Over Union `(IOU)` is observed in train , test , validation
- Total training time:
    - VGG16 - `1640.69 seconds`
    - VGG19 - `1962.71 seconds`
    - InceptionV3 - `1204.79 seconds`
    - MobileNetV2 - `1023.70 seconds`
    - DenseNet201 - `1547.24 seconds`

Yolo-NAS model:

- Model used `yolo_nas_s`
- Number of epochs  = `25`
- Batch size = `16`
- Caching annotation time (minutes) = `Train datase-07:35` `Valid dataset-02:10` `Test dataset-01:03`
- Confidence threshold = `0.25`
- Prediction on videos  = `10 videos`

### [Update 03](https://github.com/aatansen/Violence-Detection-Using-YOLOv8-Towards-Automated-Video-Surveillance-and-Public-Safety/tree/main/Update%2003)

### Vehicle detection and count

Selected Dataset:

- Custom training dataset : [Roboflow Dataset](https://universe.roboflow.com/traffic-hxmtd/vehicles-aet91/dataset/3)
    - Total = `17491 images`
        - Train = `15296 images`
        - Valid = `1458 images`
        - Test = `737 images`
- Model used `YOLOv8s`
- Number of epochs  = `15`
- Batch size = `16`
- Total training time = `2.568 hours`
- Confidence threshold = `0.25`
- Prediction on images  = `737 images`
- For object tracking = `ByteTrack`
- For Line drawing ,annotation , coloring frame by frame = `Supervision`
- Prediction and tracking on videos = `2 Videos`