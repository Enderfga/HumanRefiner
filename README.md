# HumanRefiner

![Overview](./framework.jpg)

## Introduction

Welcome to the official repository for the [paper](https://arxiv.org/abs/2407.06937) "HumanRefiner: Benchmarking Abnormal Human Generation and Refining with Coarse-to-fine Pose-Reversible Guidance."

In this project, we introduce AbHuman, the first large-scale benchmark focused on anatomical anomalies. The benchmark consists of 56K synthesized human images, each annotated with 147K human anomalies in 18 different categories. Based on this, we developed HumanRefiner, a novel plug-and-play method for coarse-to-fine refinement of human anomalies.

## Data

Our data is available on 🤗 [Hugging Face](https://huggingface.co/datasets/Enderfga/HumanRefiner).

To download the dataset, use the following commands:

```bash
git lfs install
git clone https://huggingface.co/datasets/Enderfga/HumanRefiner
```

After cloning, extract the train and validation datasets:

```bash
tar -xzf train.zip
tar -xzf val.zip
```
## Annotation Examples
Below is a detailed illustration of class definitions with visualized examples from the AbHuman dataset:
![](./example.jpg)

## Cite

If you use our work in your research, please cite our paper:

```bibtex
@InProceedings{10.1007/978-3-031-73411-3_12,
author="Guian Fang, Wenbiao Yan, Yuanfan Guo, Jianhua Han, Zutao Jiang, Hang Xu, Shengcai Liao, Xiaodan Liang",
editor="Leonardis, Ale{\v{s}}
and Ricci, Elisa
and Roth, Stefan
and Russakovsky, Olga
and Sattler, Torsten
and Varol, G{\"u}l",
title="HumanRefiner: Benchmarking Abnormal Human Generation and Refining with Coarse-to-fine Pose-Reversible Guidance",
booktitle="Computer Vision -- ECCV 2024",
year="2025",
publisher="Springer Nature Switzerland",
abstract="Text-to-image diffusion models have significantly advanced in conditional image generation. However, these models usually struggle with accurately rendering images featuring humans, resulting in distorted limbs and other anomalies. This issue primarily stems from the insufficient recognition and evaluation of limb qualities in diffusion models. To address this issue, we introduce AbHuman, the first large-scale synthesized human benchmark focusing on anatomical anomalies. This benchmark consists of 56K synthesized human images, each annotated with detailed, bounding-box level labels identifying 147K human anomalies in 18 different categories. Based on this, the recognition of human anomalies can be established, which in turn enhances image generation through traditional techniques such as negative prompting and guidance. To further boost the improvement, we propose HumanRefiner, a novel plug-and-play approach for the coarse-to-fine refinement of human anomalies in text-to-image generation. Specifically, HumanRefiner utilizes a self-diagnostic procedure to detect and correct issues related to both coarse-grained abnormal human poses and fine-grained anomaly levels, facilitating pose-reversible diffusion generation. Experimental results on the AbHuman benchmark demonstrate that HumanRefiner significantly reduces generative discrepancies, achieving a 2.9x improvement in limb quality compared to the state-of-the-art open-source generator SDXL and a 1.4x improvement over DALL-E 3 in human evaluations. Our AbHuman dataset is available at https://github.com/Enderfga/HumanRefiner.",
isbn="978-3-031-73411-3"
}
```

## Contact

If you have any questions or suggestions, please contact us:

- Email: enderfga@gmail.com
- GitHub Issues: [HumanRefiner Issues](https://github.com/Enderfga/HumanRefiner/issues)

Thank you for your support!
