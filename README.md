# fMRI-Image-CLIP

This repository consists of scripts and additional resources used for aligning fMRI data with image semantics using CLIP, as part of the Tether.io assignment. The goal is to explore the BOLD5000 dataset and use contrastive learning techniques to align the fMRI data with semantic information derived from images.

## Objective

The primary objective of this repository is to explore the BOLD5000 fMRI dataset and align its data with semantic information from images using the CLIP model. The repository contains various notebooks and scripts for performing voxel analysis, pretraining encoders, and training contrastive frameworks to align fMRI embeddings with image embeddings.

## Repository Structure

### Notebooks

The `notebooks` folder contains all the code notebooks:

1. **`analysis.ipynb`**:
   - Contains code for voxel analysis from the preprocessed flattened data used in the MindViz repository. The **MindViz** repository can be found [here](https://github.com/zjc062/mind-vis/tree/main).

2. **`Plots.ipynb`**:
   - Contains code for plotting 4D voxel data from the raw BOLD5000 dataset. You can find the dataset here: [BOLD5000 Dataset](https://figshare.com/articles/dataset/BOLD5000_Release_2_0/14456124?file=27663165).

3. **`clip-bold.ipynb`**:
   - Implements the first method in the procedure: developing a simple fMRI encoder without pretraining.

4. **`train-fmri-enc.ipynb`**:
   - Contains code to pretrain an encoder-decoder model for reconstructing fMRI data.

5. **`contrastive.ipynb`**:
   - Trains the contrastive framework to align fMRI and image embeddings using CLIP, ResNet, and fMRI from the pretrained network.

### Python Scripts

1. **`fmri-encoder.py`**:
   - Contains code for the masked brain model used in the **MindViz** repository. You can refer to the **MindViz** repository [here](https://github.com/zjc062/mind-vis).

## Environment Setup

To set up the environment for running the notebooks and scripts in this repository, follow these steps:

1. **Create a Conda Environment**:

   First, download the `requirements.yaml` file provided and create a conda environment using the following command:

   ```bash
   conda env create -f requirements.yaml
