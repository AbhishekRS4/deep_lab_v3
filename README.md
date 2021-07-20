# DeepLab\_v3 implementation on Cityscapes dataset

## Notes
* Implementation of DeepLab\_v3 with ResNet-50
* The original implementation uses ResNet-101 for cityscapes dataset
* The image dimension used to train the model is 1024x512
* 15 custom classes used

## Main idea
* Apply atrous spatial pyramid pooling to feature maps of output stride 8/16 of the input size. Perform bilinear upsampling by a factor of 8/16.

## Intructions to run
* To list training options
```
python3 src/deep_lab_v3_train.py --help
```
* To list inference options
```
python3 src/deep_lab_v3_infer.py --help
```

## Visualization of results
* [DeepLabv3]()

## Reference
* [ResNet-50](https://arxiv.org/abs/1512.03385)
* [DeepLabv3](https://arxiv.org/pdf/1706.05587.pdf)
* [Cityscapes Dataset](https://www.cityscapes-dataset.com/)
