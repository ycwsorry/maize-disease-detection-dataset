# Maize Disease Detection Dataset

This repository provides reproducibility materials for the manuscript:

LSL-YOLOv11n: An Improved Model for Maize Leaf Disease Detection in Complex Field Environments

## Dataset Size

The dataset contains 15,119 images and 29,366 annotated instances across eight categories.

| Split | Images | Label files | Annotated instances |
|---|---:|---:|---:|
| Train | 10,609 | 10,609 | 20,386 |
| Validation | 3,004 | 3,004 | 6,033 |
| Test | 1,506 | 1,506 | 2,947 |
| Total | 15,119 | 15,119 | 29,366 |

## Contents

- corn_disease_only.yaml: dataset configuration file.
- labels/: YOLO-format annotation files.
- splits/: train, validation, and test image lists.
- dataset_statistics.csv: dataset statistics.
- class_instance_statistics.csv: per-class annotation statistics.
- data_sources.csv: original dataset source information.
- data_check_report/: data consistency check files.

## Classes

0. Blight
1. brown_spot
2. corn_rust
3. corn_smut
4. downy_mildew
5. grey_leaf_spot
6. healthy
7. maize-streak-disease

## Annotation Format

All annotations are provided in YOLO TXT format:

class_id x_center y_center width height

All coordinates are normalized to the range [0, 1].

## Data Availability

The original images were collected from a public Kaggle dataset. The original image files are not included in this repository to avoid potential redistribution restrictions. This repository provides processed YOLO-format annotations, dataset split files, dataset statistics, and data consistency check files.
