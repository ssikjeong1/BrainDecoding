# MindControl


## Preparation
### Data
1. Agree to the Natural Scenes Dataset's [Terms and Conditions](https://cvnlab.slite.page/p/IB6BSeW_7o/Terms-and-Conditions) and fill out the [NSD Data Access form](https://forms.gle/xue2bCdM9LaFNMeb7)
2. Create a conda environment and install the packages necessary to run the code.
```
# install anaconda (optional)
wget "https://repo.anaconda.com/archive/Anaconda3-2024.06-1-Linux-x86_64.sh"
bash ./Anaconda3-2024.06-1-Linux-x86_64.sh
eval "$(/home/wsjeong/anaconda3/bin/conda shell.bash hook)"
source ~/.bashrc
conda init

# create a conda environment and install the packages
conda create -n mindcontrol python=3.10.8 -y
conda activate mindcontrol
pip install -r requirements.txt
```
## Training
### 

## Evaluation (w/ reconstruction)
This script performs the following tasks:
1. Reconstruct images for a single subject (e.g., subject 1) from the test set using our proposed model.
2. In this setting, our proposed model was trained on a subset of subjects (e.g., subjects 1, 2, 5, and 7).
3. Assess all relevant metrics for the reconstructed images.
4. Saves all assessed values in a CSV file for further analysis.
```
bash scripts/inference.sh
```
