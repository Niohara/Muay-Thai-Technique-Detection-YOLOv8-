# Muay Thai Technique Detection (YOLOv8)

This project is a object detection system built to identify and classify Muay Thai striking techniques. It utilizes the YOLOv8 model trained on a custom dataset to recognize 7 distinct classes.

## Test Results

| Labels | Predictions |
| :---: | :---: |
| <img alt="labels" src="https://github.com/user-attachments/assets/c771f4de-52ec-45bf-b808-d17923421abe" /> | <img alt="pred" src="https://github.com/user-attachments/assets/cbf3bb2d-0893-46fb-9ed3-967351fa1e5f" /> |

---

## Model Performance

The model was evaluated on the test set using the `best.pt` checkpoint.

| Metric | Score |
| :--- | :--- |
| **mAP50** | **0.9427994227994229** |
| **mAP50-95** | **0.9316723845206726** |

| Results | Confusion matrix |
| :---: | :---: |
| <img alt="results" src="https://github.com/user-attachments/assets/112bf200-6880-4467-bab8-4cdb9d93015b" /> | <img alt="confusion_matrix" src="https://github.com/user-attachments/assets/eb941810-9c6b-4125-93c2-048c5ffae23f" /> |

---

## Detected Classes

The model is trained to detect the following 7 classes as defined in `data.yaml`:

1.  `jab`
2.  `l. hook`
3.  `l. uppercut`
4.  `none`
5.  `r. hook`
6.  `r. uppercut`
7.  `straight`

---

## Dataset

This project uses the Muay Thai dataset (Version 2) from Roboflow. URL: `https://universe.roboflow.com/myspace-7h2qj/muay-thai/dataset/2`

To run this project:

1. **Download the dataset from the Roboflow URL above. (Choose the "YOLOv8" format).**

2. **Unzip the data and place the folders (train, valid, test) into the project directory according to the paths in `Data/data.yaml.`**

---

## Installation
Open the Windows (PowerShell) on this project's directory and run this command:
1.  **Create a virtual environment:**
    ```bash
    python -m venv venv
    ```
    
2.  **Activate environment:**
    ```bash
    .\venv\Scripts\activate
    ```

3.  **Install the required dependencies:**
    ```bash
    pip install -r requirements.txt
    ```

4.  **Now you can open the `MuayThai_YOLOV8.ipynb` file to run the project.**
