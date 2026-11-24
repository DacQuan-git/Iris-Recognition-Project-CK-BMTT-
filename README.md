# Iris-Recognition-Project-CK-BMTT-
Iris-Based Biometric Authentication Using Python
# Iris-Based Biometric Authentication

A Python-based iris recognition and authentication project developed for the Introduction to Information Security course.

## Project Overview

This project implements an iris recognition system using the CUST-Iris dataset. It extracts binary Iris Codes from eye images and matches them against a database of authorized users.

## Technologies Used

- Python
- OpenCV
- NumPy
- Matplotlib
- ipywidgets
- Google Colab

## Main Features

- Iris image preprocessing and segmentation using provided masks.
- Iris normalization to a fixed resolution of 64 × 512 pixels.
- Iris feature extraction using a Log-Gabor filter.
- Binary Iris Code generation.
- Hamming Distance matching with rotational shift compensation.
- Authorized and unauthorized user verification.

## Dataset

The project uses the CUST-Iris dataset.

Dataset source: https://doi.org/10.17632/3j6skjpsng.3

The dataset is not included in this repository. Users must download the dataset separately and upload the `CUST-Iris` folder to Google Drive.

Required directory structure:

```text
MyDrive/
└── CUST-Iris/
    ├── CUST-Iris-V1/
    └── CUST-Iris-V1-Masks/
```

## How to Run

1. Open the Jupyter Notebook in Google Colab.
2. Mount Google Drive.
3. Upload the CUST-Iris dataset using the directory structure above.
4. Run the notebook cells in order.
5. Select an eye image from the interactive interface.
6. Click **Verify Identity** to view the authentication result.

## Experimental Results

The demonstration uses 10 authorized users and 20 biometric templates.

| Evaluation Metric | Result |
|---|---:|
| Genuine Correct | 20/20 |
| Impostor Rejected | 18/20 |
| False Acceptance | 2 |
| False Rejection | 0 |
| FAR | 10% |
| FRR | 0% |
| Overall Accuracy | 95% |

The system is an academic prototype and is not intended for production use.

## Limitations

- Requires pre-existing segmentation masks.
- Uses a relatively small authorized-user database.
- Does not include liveness detection.
- Biometric templates are not encrypted in the current implementation.

## Authors
Nguyễn Đắc Minh Quân

**Course:** Introduction to Information Security

**Instructor:** Huynh Ngoc Tu
