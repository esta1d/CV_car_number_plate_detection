# CV_car_number_plate_detection

The project CV_car_number_plate_detection is a solution for detecting car license plates using computer vision methods. The primary goal of the project is automatic recognition of vehicle registration numbers in images and video streams.

## Main components of the project:
* **Detection algorithm:** The OpenCV library is used for image preprocessing, along with machine learning algorithms to highlight areas containing license plates.
* **Image processing:** Methods such as noise reduction, contrast enhancement, and color transformation are applied to improve detection accuracy.
* **Character recognition:** After isolating the number plate area, Optical Character Recognition (OCR) techniques are employed to accurately identify the characters of the vehicle's registration mark.
* **Model integration:** The project allows integrating various deep learning models to increase both precision and speed of recognition.

## Capabilities and applications:
* **Automated parking systems:** Fast and accurate identification of license plates helps optimize paid parking lots and automated parking facilities.
* **Security system:** Detection and identification of vehicles can be utilized for traffic control and preventing road violations.
* **Traffic management:** Automated vehicle tracking simplifies traffic flow management and data collection.

<img src="https://habrastorage.org/webt/cs/te/hx/cstehxj5rouuyq0jzox2to4vvi8.gif" width="100%" alt="gif">

## Project structure

```
CV_CAR_NUMBER_PLATE_DETECTION/
│
├── data                     # Project Data
│   ├── annotations          # Annotation files (*.xml)
│   │   └── *.xml
│   └── images               # Images
│       └── *.png
├── runs                      # Run Results
│   ├── weights              # Model Weights (*.pt)
│   │   └── *.pt
│   ├── *.csv                # Final predictions in CSV format
│   ├── *.png                # Visualization graphics
│   └── *.yaml               # Configuration YAML files
├── yolo                     # Folder for YOLO-related data
│   ├── images               # Separate sets of images
│   │   ├── train            # Training images
│   │   │   └── *.png
│   │   └── val              # Validation images
│   │       └── *.png
│   ├── labels               # Text annotation files
│   │   ├── train            # Labels for training set
│   │   │   └── *.txt
│   │   └── val              # Labels for validation set
│   │       └── *.txt
│   └── dataset.yaml         # Dataset configuration file
├── yolov5                   # Repository for YOLOv5 (https://github.com/ultralytics/yolov5)
│   └── repository
├── car.ipynb                # Main Jupyter notebook with code
├── .gitignore               # Files ignored by Git
├── readme.md                # Documentation
├── requirements.txt         # Requirements for Python packages
└── yolov5_predictions.csv   # Final prediction output file
```



