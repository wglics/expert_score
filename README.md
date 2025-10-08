Setup (expert_score)

1. Create a Conda virtual environment.
> conda create -n expert_score python==3.11.13

2. Install required packages.
> conda activate expert_score
> pip install torch==2.7.1 torchvision==0.22.1 torchaudio==2.7.1 --index-url https://download.pytorch.org/whl/cu118
> pip install transformers==4.52.4 tqdm datasets accelerate

3. Run expert_score.py.
> python expert_score.py
