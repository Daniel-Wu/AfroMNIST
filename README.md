# Afro-MNIST
Four Synthetic MNIST-like Datasets for African Numeral Systems: Ge`ez (Ethiopic), Vai, Osmanya, and N'Ko. 

Each dataset contains 60000 training examples and 10000 test examples. Each dataset contains an equal number of examples of the numerals 0-9, except for Ethiopic, which lacks the numeral 0, and thus contains the numerals 1-10. Datasets were generated by using elastic deformations of Unicode exemplar numerals.

This dataset was presented at Practical Machine Learning for Developing Countries at ICLR 2020, and you can see the paper and presentation at https://pml4dc.github.io/iclr2020/program/pml4dc_34.html, or the paper at https://arxiv.org/abs/2009.13509.

## Usage

1. Download the datasets:

a. Through git-lfs (First install git-lfs [here](https://github.com/git-lfs/git-lfs/wiki/Installation)):
```bash
git clone https://github.com/Daniel-Wu/AfroMNIST.git
```

b. Kaggle (https://www.kaggle.com/danjwu/afromnist)

c. Zenodo (https://zenodo.org/record/4050071)

2. Load in the datasets:
```python
import numpy as np
X_train = np.load("Ethiopic_MNIST_X_train.npy")
y_train = np.load("Ethiopic_MNIST_y_train.npy")
X_test  = np.load("Ethiopic_MNIST_X_test.npy")
y_test  = np.load("Ethiopic_MNIST_y_test.npy")
```

3. Plug and play with your favorite machine learning framework!


## Citing
If this dataset was useful to you, we suggest citing this paper with the following Bibtex:
```
@misc{wu2020afromnist,
      title={Afro-MNIST: Synthetic generation of MNIST-style datasets for low-resource languages}, 
      author={Daniel J Wu and Andrew C Yang and Vinay U Prabhu},
      year={2020},
      eprint={2009.13509},
      archivePrefix={arXiv},
      primaryClass={cs.CV}
}
```
