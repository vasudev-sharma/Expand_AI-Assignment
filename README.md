# Expand AI Assignment

## Problem Statement: 
**Computer Vision Track** - Chest X Ray Classification into 3 categories namely **COVID**, **Normal**, and **Pneumonia**<br>

For more details, read the problem statement available [here](https://github.com/vasudev-sharma/Expand_AI-Assignment/blob/master/Expand%20AI%20Computer%20Vision%20Assignment.pdf)

## Data
Dataset is in this Gdrive location:-> https://drive.google.com/file/d/1PVJcXmKz-QPAvPV-rRFYnjh7BsFnAeq8/view?usp=sharing

## Usage:
The Colab notebooks for the [Assignment-1](https://github.com/vasudev-sharma/Expand_AI-Assignment/blob/master/Expand_ai_problem_1.ipynb) and [Assignment-2](https://github.com/vasudev-sharma/Expand_AI-Assignment/blob/master/Expand_ai_problem_2.ipynb) are self-explantory. 

**NOTE** It is recommended to run the notebook on a GPU instance. If not available, kindly use the free Google Colab GPU instance

## RESULTS: 
### Assignment 1 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://github.com/vasudev-sharma/Expand_AI-Assignment/blob/master/Expand_ai_problem_1.ipynb) [![](https://raw.githubusercontent.com/wandb/assets/main/wandb-github-badge-28.svg)](https://wandb.ai/vs74/Expand-ai-problem-1?workspace=user-vs74) <img alt="PyTorch" src="https://img.shields.io/badge/PyTorch-%23EE4C2C.svg?style=for-the-badge&logo=PyTorch&logoColor=white" />

| Base Model      | Macro_f1_score | Accuracy    | Micro_F1_score | Model Logs                                                                  |
|-----------------|----------------|-------------|----------------|-----------------------------------------------------------------------------|
| densenet121     | 0.64502938     | 0.989583373 | 0.98958333     | https://wandb.ai/vs74/Expand-ai-problem-1/runs/1f2z5217?workspace=user-vs74 |
| efficientnet-b5 | 0.59190719     | 0.979166687 | 0.97916667     | https://wandb.ai/vs74/Expand-ai-problem-1/runs/3czw9l6w?workspace=user-vs74 |
| efficientnet-b3 | 0.65858588     | 0.989583373 | 0.98958333     | https://wandb.ai/vs74/Expand-ai-problem-1/runs/g3folx1r?workspace=user-vs74 |
| efficientnet-b0 | 0.60034412     | 0.989583373 | 0.98958333     | https://wandb.ai/vs74/Expand-ai-problem-1/runs/2urz30gh?workspace=user-vs74 |
| resnet101       | 0.57482045     | 0.963541687 | 0.96354167     | https://wandb.ai/vs74/Expand-ai-problem-1/runs/2w044b3y?workspace=user-vs74 |
| densenet169     | 0.59401157     | 0.984375    | 0.984375       | https://wandb.ai/vs74/Expand-ai-problem-1/runs/1f136ly7?workspace=user-vs74 |

---

### Assignment 2 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://github.com/vasudev-sharma/Expand_AI-Assignment/blob/master/Expand_ai_problem_2.ipynb) [![](https://raw.githubusercontent.com/wandb/assets/main/wandb-github-badge-28.svg)](https://wandb.ai/vs74/Expand-ai-problem-2?workspace=user-vs74) <img alt="PyTorch" src="https://img.shields.io/badge/PyTorch-%23EE4C2C.svg?style=for-the-badge&logo=PyTorch&logoColor=white" />

To tackle limited labels for Chest XRay images, a semi-supervised learning apprach known as [MixMatch](https://arxiv.org/abs/1905.02249) approach is adopted.<br>

The [Assignment-2](https://github.com/vasudev-sharma/Expand_AI-Assignment/blob/master/Expand_ai_problem_2.ipynb) solution has been inspired from this https://github.com/YU1ut/MixMatch-pytorch repository. 

| Base Model | Accuracy | Macro_F1_Score | Micro_F1_score | Model Logs                                                                        |
|------------|----------|----------------|----------------|-----------------------------------------------------------------------------|
| ResNet-50  | 96.90%   | 0.3452         | 0.9609         | https://wandb.ai/vs74/Expand-ai-problem-2/runs/3bistr67?workspace=user-vs74 |

## [Report](https://github.com/vasudev-sharma/Expand_AI-Assignment/blob/master/Report.pdf)
Well, you might be wondering why a specific model/algorithm was tried for this problem, right? To know about the thought process, kindly refer [here](https://github.com/vasudev-sharma/Expand_AI-Assignment/blob/master/Report.pdf)

## Contributing
We ❤️ contributions. Feel free to send us a PR or raise an issue.

1. Create an issue if there is one.
2. Fork the repo.
3. Create your feature branch (`git checkout -b your-feature`).
4. Add and commit your changes (`git commit -am 'message'`).
5. Push the branch (`git push origin your-feature`).
6. Create a new Pull Request.


## TODO
- [ ] Play with the hyperparameters of the MixMatch algorithm
- [ ] Experiment with differnt baseline models. Eg.. DenseNets, EfficientNets, etc...
