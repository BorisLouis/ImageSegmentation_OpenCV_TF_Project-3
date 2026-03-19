# ImageSegmentation_OpenCV_TF_Project-3

#TO BE UPDATED


Semantic image segmentation project built as part of the [OpenCV University TensorFlow Deep Learning course](https://opencv.org/university/), submitted to the [Kaggle competition: OpenCV TF Project-3 Image Segmentation Round 4](https://www.kaggle.com/competitions/open-cv-tf-project-3-image-segmentation-round-4).

---

## Project Description & Goal

The goal of this project is to train a deep learning model capable of performing **semantic segmentation** — assigning a class label to every pixel in an image.

The model architecture follows a **multi-scale feature pyramid** design:
- A **CNN backbone** extracts rich feature representations from the input
- A **Pooling Pyramid Module (PPM)** captures context at multiple scales simultaneously
- An **upsampling + concatenation** decoder fuses multi-scale features
- A **classification head** produces the final per-pixel predictions

Performance is evaluated using **mean Intersection over Union (mIoU)** across all classes.

---

## Dataset

> ⚠️ *Fill in the details below from the Kaggle competition page once you have access.*

| Property | Details |
|---|---|
| Dataset name | <!-- e.g. FloodNet --> |
| Number of images | <!-- e.g. 2343 train / 522 val --> |
| Image size | <!-- e.g. 3000 × 4000 px --> |
| Number of classes | <!-- e.g. 10 --> |
| Mask format | <!-- e.g. PNG, single-channel label map --> |
| Task type | Semantic Segmentation |

### Classes
<!-- List the segmentation classes here, e.g.:
- 0: Background
- 1: Building flooded
- 2: Building non-flooded
- ...
-->

---

## Project Structure

```
ImageSegmentation_OpenCV_TF_Project-3/
├── notebooks/
│   └── project.ipynb         # Main training notebook (Colab)
├── src/
│   ├── model.py              # Model architecture
│   ├── dataset.py            # Data loading & augmentation
│   └── train.py              # Training loop & config
├── README.md
└── .gitignore
```

---

## Setup

### 1. Clone the repo
```bash
git clone https://github.com/YOUR_USERNAME/ImageSegmentation_OpenCV_TF_Project-3.git
cd ImageSegmentation_OpenCV_TF_Project-3
```

### 2. Download the data (Kaggle API)
```bash
pip install kaggle
kaggle competitions download -c open-cv-tf-project-3-image-segmentation-round-4
unzip \*.zip
```

### 3. Run in Google Colab
Open `notebooks/project.ipynb` in Google Colab and follow the cells in order.

---

## Results

| Metric | Score |
|---|---|
| mIoU (validation) | *TBD* |
| Kaggle leaderboard score | *TBD* |

---

## References

- [OpenCV University Deep Learning Course](https://opencv.org/university/)
- [Kaggle Competition Page](https://www.kaggle.com/competitions/open-cv-tf-project-3-image-segmentation-round-4)
