# 🌠 FLARE: Fast Learning for Astronomical Real-time Events 🌠

This project implements a machine learning pipeline to classify astronomical transient alerts from survey images as either "Real" astrophysical events or "Bogus" instrumental artifacts. The goal is to automate the vetting process, accelerating discovery.

## Setup Instructions

Follow these steps to set up and run the project:

### 1. Clone the Repository

Clone this repository to your local machine using Git:

```bash
git clone https://github.com/ShivamChaturvedi05/FLARE.git
cd FLARE
```

### 2\. Install Dependencies

Install the required Python packages using the provided `requirements.txt` file:

```bash
pip install -r requirements.txt
```

### 3\. Download the Dataset

The astronomical image dataset is large and not included in this repository.

  * Download the dataset files from the **Zenodo repository**: [**https://zenodo.org/records/14714279**](https://zenodo.org/records/14714279)
  * Inside the `FLARE` project directory, create a new folder named `dataset`.
  * Place all the downloaded `.npy` and `.csv` files directly into this `FLARE/dataset/` folder.

Your project directory structure should now look like this:

```
FLARE/
├── dataset/
│   ├── ATLAS_images.npy
│   ├── ATLAS_labels.csv
│   ├── MeerLICHT_images.npy
│   ├── MeerLICHT_labels.csv
│   ├── PANSTARRS_images.npy
│   └── PANSTARRS_labels.csv
├── FLARE.ipynb
├── .gitignore
├── requirements.txt
└── README.md
```

### 4\. Run the Jupyter Notebook

You can now launch Jupyter Notebook or Jupyter Lab and open the `FLARE.ipynb` notebook to run the analysis and model training pipeline.

```bash
jupyter notebook FLARE.ipynb
# or
jupyter lab FLARE.ipynb
```

Make sure the file paths for loading the dataset within the notebook (e.g., `dataset/ATLAS_images.npy`) are correct.
