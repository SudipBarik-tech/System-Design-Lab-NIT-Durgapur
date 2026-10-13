# Smart Ring V1 — IMU Gesture Dataset

The uploaded Smart Ring project contains **179 CSV recordings** organised by gesture and recording session.

## Classes

| Gesture | Files |
|---|---:|
| `click` | 51 |
| `double_click` | 29 |
| `idle` | 18 |
| `swipe_up` | 18 |
| `swipe_down` | 27 |
| `swipe_left` | 18 |
| `swipe_right` | 18 |
| **Total** | **179** |

## CSV fields

The data collector writes the following columns:

- `t_ms`
- `Accel_X`, `Accel_Y`, `Accel_Z`
- `Gyro_X`, `Gyro_Y`, `Gyro_Z`
- `label`
- `session_id`

## Original organisation

```text
IMU_Gesture_Data/
├── click/
├── double_click/
├── idle/
├── swipe_up/
├── swipe_down/
├── swipe_left/
└── swipe_right/
```

Each class contains one or more session folders such as `day1_me`, `day2_me`, etc., with files named `sample1.csv`, `sample2.csv`, and so on.

The source scripts in the V1 folder use this dataset structure for preprocessing, feature extraction, model training and real-time gesture recognition.
