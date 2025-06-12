# vanguard-dataset-exploration
Repository to explore defense datasets

## xView Dataset (Drone / Overhead Imagery)
**Link**: [Kaggle - xView Dataset](https://www.kaggle.com/datasets/hassanmojab/xview-dataset)  
**License**: CC BY-NC-SA 4.0  
**Modality**: Drone / Satellite Imagery  
**Size**: ~20 GB (images + annotations)

### Description
xView is one of the largest publicly available overhead imagery datasets for object detection.  
It contains over 1 million labeled objects** across 60 classes.
The dataset supports computer vision applications in defense, intelligence, and surveillance.

### File Structure (in this repo)
The `datasets/xview/` folder includes:
- `xview-sample.tif` — A representative satellite image tile
- `xview-sample-annotation.json` — A GeoJSON-style file with sample object annotations
  - Includes polygon coordinates and properties such as `type_id`, `feature_id`, and `image_id`