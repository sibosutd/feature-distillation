# feature-distillation

This repository implements DNN-Oriented JPEG compression introduced in the following paper 

[Feature Distillation: DNN-Oriented JPEG Compression Against Adversarial Examples](https://arxiv.org/abs/1803.05787)

## Introduction

![DNN-Oriented JPEG Compression][fig1]

Figure 1: Diagram of DNN-Oriented JPEG compression

## Usage

```
python jpeg.py --image fig/lena.png --component dnn
```

```
usage: jpeg.py [-h] [--image IMAGE] [--component COMPONENT] [--factor FACTOR]
optional arguments:
  -h, --help            show this help message and exit
  --image IMAGE         image name
  --component COMPONENT
                        dnn-oriented or jpeg standard
  --factor FACTOR       compression factor
```

## Results

![Compare][fig2]

Figure 2: Standard JPEG compression (Q = 50)

![Compare][fig3]

Figure 3: DNN-Oriented JPEG compression (Q = 50)

## TODO

- [x] zigzag sorting
- [ ] sorting by standard deviation
- [ ] adversarial defense evaluation

## Contribution

If you find a bug, feel free to create an issue.

## Reference
+ [ghallak/jpeg-python](https://github.com/ghallak/jpeg-python)

<!-- Links -->

[fig1]: fig/fig1.png
[fig2]: fig/compare1.png
[fig3]: fig/compare2.png
