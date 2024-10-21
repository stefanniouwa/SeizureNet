# Overview
Using Deep Learning algorithms; namely WaveNet and Bi-Directional LSTM for multi-class classification of (7) seizure types, to be trained and tested on the TUH Seizure Corpus (TUSZ v2.0.3) dataset (March 2024). This repository provides the code.

@author: Stefan Nio
The University of Western Australia

# Development
To set up the development environment for EEG seizure detection, please follow these steps:

1. Navigate to the Project Directory

Open your terminal and navigate to the root directory of the project.

2. Create the Conda Environment

Create a new Conda environment using the provided <code>cits4010.yml</code> file:
```bash
conda env create -f cits4010.yml
```


3. Activate the Environment

Activate the newly created environment:

```bash
conda activate cits4010
```

# The TUSZ Dataset
The Temple University Hospital (TUH) EEG Corpus includes a large number of EEG data recordings. Detailed information and instructions are summarized on the TUH EEG Corpus [Download Page](https://isip.piconepress.com/projects/nedc/html/tuh_eeg/#i_rsyn).

## Downloading the dataset
To access the TUH EEG Corpus, please follow the instructions on the link above, outlining an email to be sent to them.
Once your request is approved, you will receive a username and password to access the dataset.

1. Navigate to Your Desired Download Directory

Open your terminal and navigate to the directory where you want to download the dataset.

2. Use the <code>rsync</code> Command

Execute the following command:

```
rsync --delete -auxv nedc-eeg@www.isip.piconepress.com:data/eeg/tuh_eeg_seizure/v2.0.3/ .
```
where <code>.</code> is where you want the dataset to be downloaded to.

This will take a long time, you will effectively be downloading approx 80Gb of seizure data.
