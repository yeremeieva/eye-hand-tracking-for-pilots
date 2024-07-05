# Eye-Tracking and Hand Movement Analysis

## Project Overview

This project aims to analyze eye-tracking and hand movement data to understand different behavioral patterns between the pilot and not experienced pilot. The aim is to be able to classify if the data is for experienced pilot or not experienced pilot. The project is structured into different directories, each serving a specific purpose in the analysis workflow.

## Directory Structure

```
eye-tracking-hand-movement/
├── .idea/
├── data/
│   ├── eye-tracking/
│   │   ├── example/
│   │   ├── left right classification/
│   │   ├── narein_piloting/
│   │   │   ├── 3d_eye_states.csv
│   │   │   ├── blinks.csv
│   │   │   ├── events.csv
│   │   │   ├── fixations.csv
│   │   │   ├── gaze.csv
│   │   │   ├── imu.csv
│   │   │   ├── info.json
│   │   │   ├── labels.csv
│   │   │   ├── saccades.csv
│   │   │   ├── scene_camera.json
│   │   │   ├── world_timestamps.csv
│   │   ├── Person1 gaze analysis/
│   │   ├── Person2 gaze analysis/
│   │   ├── screen classification/
│   │   ├── sofiia_piloting/
│   ├── hand-movement/
│   │   ├── example/
│   │   ├── narein_hands.csv
│   │   ├── sofiia_hands.csv
├── notebooks/
│   ├── eye-tracking/
│   │   ├── analysis_schema.ipynb
│   │   ├── gaze_analysis.ipynb
│   │   ├── left_right_classification.ipynb
│   │   ├── piloting_first_try.ipynb
│   ├── hand-movement/
│   │   ├── analysis_schema.ipynb
│   ├── sofiia_narein_piloting_eyes.ipynb
└── venv/
```

## Contents

### .idea/
Contains project-specific settings and configurations for the IDE.

### data/
Houses all the datasets used in the project. 

#### eye-tracking/
Contains eye-tracking data and for various experiments.

- **narein_piloting/**: Example of the data structure.
  - `3d_eye_states.csv`: 3D states of eye movements.
  - `blinks.csv`: Data on blinks.
  - `events.csv`: Various eye-tracking events.
  - `fixations.csv`: Data on fixations.
  - `gaze.csv`: Gaze data.
  - `imu.csv`: Inertial measurement unit data.
  - `info.json`: Information about the dataset.
  - `labels.csv`: Labels for the data.
  - `saccades.csv`: Saccade data.
  - `scene_camera.json`: Scene camera settings.
  - `world_timestamps.csv`: Timestamps for world events.


#### hand-movement/
Contains hand movement data.

### notebooks/
Jupyter notebooks for data analysis and experimentation.

#### eye-tracking/
- `analysis_schema.ipynb`: Schema for analyzing eye-tracking data.
- `gaze_analysis.ipynb`: Notebook for gaze analysis, also can be treated as a schema.
- `left_right_classification.ipynb`: Notebook for left-right classification analysis.
- `piloting_first_try.ipynb`: Initial piloting data analysis.

#### hand-movement/
- `analysis_schema.ipynb`: Schema for analyzing hand movement data.

#### sofiia_narein_piloting_eyes.ipynb
The final analysis notebook that contains all plots and strategies to classify the data. Should be treated as the main file in the project.


## Getting Started

1. Clone the repository.
2. Set up the virtual environment:
   ```sh
   python -m venv venv
   source venv/bin/activate  # On Windows use `venv\Scripts\activate`
   pip install -r requirements.txt
   ```
3. Navigate to the `notebooks` directory to start analyzing the data.
