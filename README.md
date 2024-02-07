# LoRA: Low-Rank Adaptation of Large Language Models

This repository contains the implementation of LoRA (Low-Rank Adaptation), a technique proposed by researchers at Microsoft Corporation for adapting large-scale language models to specific tasks efficiently. 
LoRA reduces the number of trainable parameters and GPU memory requirements, making it feasible to adapt models like GPT-3 for various downstream tasks without significant computational overhead.

## Abstract

LoRA freezes the pre-trained model weights and introduces trainable rank decomposition matrices into each layer of the Transformer architecture. This significantly reduces the number of trainable parameters for downstream tasks while maintaining or improving model quality compared to full fine-tuning. The key advantages of LoRA include:
- Reduction in trainable parameters by up to 10,000 times
- Lower GPU memory requirement by up to 3 times
- No additional inference latency compared to fully fine-tuned models
- Compatibility with various prior methods, enhancing its versatility

## Contents

- `README.md`: Overview of the repository and LoRA technique
- `LoRA.ipynb`: Implementation of LoRA module in PyTorch
- `SVD_and_Rank.ipynb`: Notebook to understand rank of matrix and SVD.
- `requirements.txt`: List of required Python packages

## Usage

1. Install the required Python packages:

```
pip install -r requirements.txt
```


## Acknowledgements

I would like to thank the authors of LoRA for their contribution to the natural language processing community.


## Citation
```
@article{hu2021lora,
title={LoRA: Low-Rank Adaptation of Large Language Models},
author={Hu, Edward and Shen, Yelong and Wallis, Phillip and Allen-Zhu, Zeyuan and Li, Yuanzhi and Wang, Shean and Wang, Lu and Chen, Weizhu},
journal={arXiv preprint arXiv:2106.09685},
year={2021}
}
```

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
