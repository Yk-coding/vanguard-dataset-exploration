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

### File Structure
The `datasets/xview/` folder includes:
- `xview-sample-image.tif` — A representative satellite image tile
- `xview-sample-annotation.json` — A GeoJSON-style file with sample object annotations
  - Includes polygon coordinates and properties such as `type_id`, `feature_id`, and `image_id`

## RadarScenes (Radar Point Cloud Data Set)
**Link**: [RadarScenes - Dataset](https://radar-scenes.com/dataset/about)
**License**: CC BY-NC-SA 4.0	
**Modality**: Automotive Radar
**Size**: ~4 hours driving data 7500+ unique objects

### Description
The RadarScenes data set contains data from four automotive radar sensors mounted on one measurement vehicle. 
The data set was recorded between 2016 and 2018 in Ulm, Germany.
This datasets contains and supplies about 4 million annotated detections of 11 different object classes.

### File Structure
The folder `datasets/radarscenes/` includes:
- `radarscenes-sample-data.h5` — Radar target and motion data for one sequence  
- `radarscenes-sample-scene.json` — Metadata about the recorded sequence  
- `radarscenes-sample-image.jpg` — Camera image showing one annotated frame with highlighted objects

### Usage Notes
- Use `h5py` or similar libraries to read `radar_data.h5`

## Noisy Drone RF Signal Classification (RF Waveform)
**Link**: [Kaggle - Noisy Drone RF Signal Classification Dataset](https://www.kaggle.com/datasets/sgluege/noisy-drone-rf-signal-classification)    
**License**: CC BY 4.0    
**Modality**: RF Waveform    
**Size**: ~25 GB (6 drone types + 4 controller types + noise class)  

### Description
The Noisy Drone RF Signal Classification dataset contains data from six consumer grade drones and noise. 
The dataset contains 7 different object classes, 6 being for the drones and 1 being noise (around 8872 noise samples in total). 
More detailed information about this dataset and its initial use to support a convolutional neural network that detected and classified drones using radio frequency signals can be found here: https://www.scitepress.org/Papers/2023/121768/121768.pdf.   

### File Structure
The `datasets/noisydronerf/` folder includes:
- `class_stats.csv` — Number of samples per drone class and their integer class ID (`class_int`)
- `SNR_stats.csv` — Number of samples per signal-to-noise ratio (SNR) level across the dataset

### Usage Notes
The full dataset is stored in a large PyTorch tensor file named `dataset.pt`, which is not included here due to its size (~25.88 GB). 
To load the full dataset, download it from Kaggle.
