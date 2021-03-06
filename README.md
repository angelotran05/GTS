# GTS
[Grid Tagging Scheme for Aspect-oriented Fine-grained Opinion Extraction](https://arxiv.org/pdf/2010.04640.pdf). Zhen Wu, Chengcan Ying, Fei Zhao, Zhifang Fan, Xinyu Dai, Rui Xia. In Findings of EMNLP, 2020.

## Data
Data format descriptions are [here](https://github.com/NJUNLP/GTS/blob/main/data/datareadme.md).

## Requirements
* pytorch=1.4.0
* python=3.6

## Usage
- ### Training
For example, you can use the folowing command to fine-tune Bert on the OPE task (the pre-trained Bert model is saved in the folder "pretrained/"):
```
python main.py --task pair --mode train --dataset res14
```
The best model will be saved in the folder "savemodel/".

- ### Testing
For example, you can use the folowing command to test Bert on the OPE task:
```
python main.py --task pair --mode test --dataset res14
```

**Note**: In our pre-experiments, a smaller batch size and learning rate can achieve better performance on certain datasets, while we use a general setting in our paper to save time instead of adopting grid search.

## Citation
If you used the datasets, please cite our paper:
```bibtex
@article{wu2020grid,
  title     = {Grid Tagging Scheme for Aspect-oriented Fine-grained Opinion Extraction},
  author    = {Zhen Wu and Chengcan Ying and Fei Zhao and Zhifang Fan and Xinyu Dai and Rui Xia},
  booktitle = {Findings of EMNLP},
  year      = {2020},
  url       = {https://arxiv.org/pdf/2010.04640.pdf},
}
```

## Reference
[1]. Zhen Wu, Chengcan Ying, Fei Zhao, Zhifang Fan, Xinyu Dai, Rui Xia. [Grid Tagging Scheme for Aspect-oriented Fine-grained Opinion Extraction](https://arxiv.org/pdf/2010.04640.pdf). In Findings of EMNLP, 2020.

[2]. Zhifang Fan, Zhen Wu, Xin-Yu Dai, Shujian Huang, Jiajun Chen. [Target-oriented Opinion Words Extraction with Target-fused Neural Sequence Labeling](https://www.aclweb.org/anthology/N19-1259.pdf). In Proceedings of NAACL, 2019.
