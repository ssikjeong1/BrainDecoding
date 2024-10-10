# MindControl


### Environment setup
```
# install anaconda
wget "https://repo.anaconda.com/archive/Anaconda3-2024.06-1-Linux-x86_64.sh"
bash ./Anaconda3-2024.06-1-Linux-x86_64.sh

eval "$(/home/wsjeong/anaconda3/bin/conda shell.bash hook)"
source ~/.bashrc
conda init

conda create -n mindcontrol python=3.10.8 -y
conda activate mindcontrol
pip install -r requirements.txt
```
## Preparation
### Data

## Training
### 

## Evaluation (w/ reconstruction)
This script performs the following tasks:
1. Reconstruct images for a single subject (e.g., subject 1) from the test set using our proposed model.
2. In this setting, our proposed model was trained on a subset of subjects (e.g., subjects 1, 2, 5, and 7).
3. Assess all relevant metrics for the reconstructed images.
4. Saves all assessed values in a CSV file for further analysis.

This script reconstructs one subject's (e.g., subject 1) images on the test set from our proposed model (e.g., subjects 1, 2, 5, and 7) and then assesses all the metrics. All assessed values will be saved in a csv file.
```
bash scripts/inference.sh
```
