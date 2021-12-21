# Crowd-Robot-Interaction
2021-2 CAU Robot Vision Project repository

## Abstract
Crowd-robot interaction은 에서 다루는 것은 군중 사이를 통과해서, 안전하고 사회 규범을 지키는 경로를 찾아 목적지를 찾아가는 문제로, 공장, 식당, 병원 등 다양한 장소에서 로봇이 사용됨에 따라 그 중요도가 날로 더해지고 있다. 
Crowd-robot interaction은 단순히 장애물 피하기가 아니라  사람과 사람, 사람과 로봇 사이의 상호작용을 이해하고 예측할 수 있어야 하므로 그 난이도가 더 어렵게 된다. 
본 프로젝트에서는 기존에 작성된 논문 가운데 [CrowdNav](https://arxiv.org/abs/1809.08835)의 특징을 분석하고, 발견한 문제점에 대해 개선을 시도하는 것을 목표로 한다.

## Citation Paper
- CrowdNav : [`Paper`](https://arxiv.org/abs/1809.08835) | [`Code`](https://github.com/vita-epfl/CrowdNav)
- RelationalGraphLearning : [`Paper`](https://arxiv.org/abs/1909.13165) | [`Code`](https://github.com/ChanganVR/RelationalGraphLearning)
- Social NCE : [`Paper`](https://arxiv.org/abs/2012.11717) | [`Code`](https://github.com/vita-epfl/social-nce)

## Code
- CrowdNav
  - [CrowdNav](crowd_nav.ipynb) : CrowdNav Train Test Experiment Code
- Social-NCE
  - [socialNCE](socialNCE_styoo.ipynb) : SocialNCE Training & Evaluation Code
  - [socialNCEtest](SocialNCEtest.ipynb) : SocialNCE Test with CrowdNav unction

## Simulation Setup
- IDE : Google Colab Pro
- Python : 3.6.8

## Train Process
- Imitation learning
  - Used 3,000 ORCA episode
  - 50 epoch train with learning rate 0.01

- reinforcement learning
  - Train 10,000 episode with OM-SARL policy

## Test Environment
- Increasing the number of people (5, 10, 20)
- Fixed Obstacles 10
- Fixed Obstacles 5 + People 5

  
## Simulation Videos


 
## Citation
```bibtex
@article{liu2020snce,
  title   = {Social NCE: Contrastive Learning of Socially-aware Motion Representations},
  author  = {Yuejiang Liu and Qi Yan and Alexandre Alahi},
  journal = {arXiv preprint arXiv:2012.11717},
  year    = {2020}
}
@inproceedings{chen2019crowd,
  title={Crowd-robot interaction: Crowd-aware robot navigation with attention-based deep reinforcement learning},
  author={Chen, Changan and Liu, Yuejiang and Kreiss, Sven and Alahi, Alexandre},
  booktitle={2019 International Conference on Robotics and Automation (ICRA)},
  pages={6015--6022},
  year={2019},
  organization={IEEE}
}
```
