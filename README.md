# vanguard-dataset-exploration
Repository to explore defense datasets

## xView Dataset (Drone / Overhead Imagery)
**Link**: [Kaggle - xView Dataset](https://www.kaggle.com/datasets/hassanmojab/xview-dataset)  
**License**: CC BY-NC-SA 4.0  
**Modality**: Drone / Satellite Imagery  
**Size**: ~20 GB (images + annotations)

### Description
xView is one of the largest publicly available overhead imagery datasets for object detection.  
It contains over 1 million labeled objects across 60 classes.
The dataset supports computer vision applications in defense, intelligence, and surveillance.

### File Structure (in this repo)
The `datasets/xview/` folder includes:
- `xview-sample.tif` — A representative satellite image tile
- `xview-sample-annotation.json` — A GeoJSON-style file with sample object annotations
  - Includes polygon coordinates and properties such as `type_id`, `feature_id`, and `image_id`

## RadarScenes (Radar Point Cloud Data Set)
**Link**: [RadarScenes - Dataset](https://radar-scenes.com/dataset/about)

**Liscense**: CC BY-NC-SA 4.0	

**Modality**: Automotive Radar

**Size**: ~4 hours driving data 7500+ unique objects

### Description
The RadarScenes data set contains data from four automotive radar sensors mounted on one measurement vehicle. 
The data set was recorded between 2016 and 2018 in Ulm, Germany.
This datasets contains and supplies about 4 million annotated detections of 11 different object classes.

### File Structure
The xxx folder includes:
- xxx — the recorded data from radar and odometry sensors
  - radar and odometry data of  timestamp(xxx), x_seq(xxx), y_seq(xxx), yaw_seq(xxx), vx(xxx), yaw_rate(xxx)  
- xxx — in which meta-information are stored
  - Specific json files include
    -sensors — describes the position and orientation of the four radar sensors.
    -sequences — 1 entry/sequence of category, scenes, and duration.
    -scenes — meta-information for a specific sequence and the scenes.
