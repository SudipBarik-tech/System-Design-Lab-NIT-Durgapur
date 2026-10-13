# Smart Ring — V1

Smart gesture-detection ring prototype based on IMU motion data and BLE communication.

## What is included

- BLE IMU data collection utility with live monitoring
- Gesture dataset organisation for click, double-click, idle and swipe gestures
- Random Forest training pipeline using accelerometer and gyroscope features
- Real-time gesture prediction and mouse-control prototypes
- Versioned experimental scripts for iterative testing

## Gesture classes

The supplied dataset contains **179 CSV recordings** across seven gesture classes:

| Gesture | CSV samples |
|---|---:|
| Click | 51 |
| Double Click | 29 |
| Idle | 18 |
| Swipe Up | 18 |
| Swipe Down | 27 |
| Swipe Left | 18 |
| Swipe Right | 18 |

## Main files

- `data_collector.py` — BLE IMU data capture and CSV logging
- `model_train.py` — preprocessing, feature extraction and Random Forest training
- `rt_v5.py` — real-time gesture inference and mouse-control prototype
- `new_py_v4.py`, `new_rt_v2.py`, `v3_rtmodel.py` — earlier/alternate real-time experimental versions
- `Dataset/README.md` — dataset structure and class summary
- `requirements.txt` — Python dependencies used by the supplied scripts

## Notes

The original uploaded project contained the full IMU dataset under `IMU_Gesture_Data/`. The source scripts are being kept in this V1 workspace so the development history remains separate from later Smart Ring iterations.
