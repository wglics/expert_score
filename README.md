Setup (expert_score)

1. Create a Conda virtual environment.
> conda create -n expert_score python==3.11.13

2. Install required packages.
> conda activate expert_score
> pip install torch==2.7.1 torchvision==0.22.1 torchaudio==2.7.1 --index-url https://download.pytorch.org/whl/cu118
> pip install transformers==4.52.4 tqdm datasets accelerate

3. Run expert_score.py.
> python expert_score.py

The output should match the following result:
# ['In', ' machine', ' learning', ',', ' diffusion', ' models', ',', ' also', ' known', ' as', ' diffusion', '-', 'based', ' gener', 'ative', ' models', ' or', ' score', '-', 'based', ' gener', 'ative', ' models', ',', ' are', ' a', ' class', ' of', ' latent', ' variable', ' gener', 'ative']
# expert_score.shape torch.Size([16, 100, 32, 64])
# expert_score[0, 2, 1, :] tensor([-0.2563, -0.6067, -0.2866, -0.5339, -0.5868, -1.0188,  0.6949, -1.4125,
#         -0.1977, -0.0346, -0.7053, -1.0664, -2.8447, -0.4771,  1.7898, -0.0778,
#         -0.2615,  0.5611, -1.1094, -2.1070, -0.4468, -0.2739, -2.4814, -0.6204,
#         -1.0243, -0.1866,  2.9565,  0.0549, -2.2698, -0.9345, -0.9147, -0.4220,
#         -0.5807, -0.0620, -2.0663, -0.1985, -0.7091, -0.2198, -0.4348, -0.3085,
#         -0.9570, -1.0319, -1.0329, -1.2994, -0.6700,  0.0754, -1.1656, -0.1296,
#         -0.7994, -0.2970, -0.5266, -0.0370,  0.2275, -1.3549, -0.4351, -0.6719,
#         -0.3611, -0.5907, -1.9266, -0.2232, -0.9368, -0.3309, -0.2454, -0.4561],
#        device='cuda:0')
# top_n_experts[0, 2, 1, :] tensor([26, 14,  6, 17, 52, 45, 27,  9], device='cuda:0')