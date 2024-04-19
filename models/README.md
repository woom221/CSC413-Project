# README

## Overview

This repository contains three Jupyter Notebook files (`Segformer.ipynb`, `FCN.ipynb`, and `LRASPP.ipynb`) used for semantic segmentation projects. Each file utilizes a different model specified in its name, but otherwise, they share a similar structure.

## Setup Instructions

### Prerequisites

- A Google Colab account with access to GPU.
- Internet connection to download the dataset.

### Folder Structure

1. Inside your Google Drive, create a folder named `413_Project`.
2. Upload the `.ipynb` files mentioned above into the `413_Project` folder.
3. Within `413_Project`, create another folder named `Med-Seg-Decathlon`.
4. Download `Task02_Heart.tar` from the following Google Drive link:
   [Task02_Heart.tar Download](https://drive.google.com/drive/folders/1HqEgzS8BV2c7xYNrZdEAnrHk7osJJ--2)
5. Upload the downloaded `.tar` file into the `Med-Seg-Decathlon` folder.

Ensure the following paths are valid:

- `My Drive/413_Project/Segformer.ipynb`
- `My Drive/413_Project/Med-Seg-Decathlon/Task02_Heart.tar`

### Running the Notebooks

1. Open any of the `.ipynb` files in Google Colab and set the runtime to use a GPU.
2. Navigate to `Part 1 - 2: Task02 Heart Dataset Split`.
3. Execute all code blocks above the section that says, "YOU CAN MOVE TO PART 2 or 3 After running code above this block!" by selecting `Runtime` -> `Run Before`.
4. If running for the first time, uncomment and run the code block containing `!tar` to unzip `Task02_Heart.tar`.
   - If a `Task02_Heart` folder already exists in `Med-Seg-Decathlon`, skip the unzipping step.
5. Proceed to `Part 3: Training the Model` and run all subsequent blocks.

### Configurations

- **Data Augmentation:** To toggle data augmentation, navigate to the `split_dataset()` function and change the third parameter passed to `MedicalImageDataset` to either `True` (enable) or `False` (disable). Typically, this is used to control the augmentation of the training set.
- **Transfer Learning vs. Learning from Scratch:** In `Part 3 - 3: Model Initialization and Parameter Info Log`, you can choose to freeze (transfer learning) or unfreeze (from scratch) the `requires_grad` attribute of the parameters depending on your training approach.
