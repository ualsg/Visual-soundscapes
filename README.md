# Sensing soundscapes from street view imagery

## Introduction
The acoustic environment is an essential component of healthy and sustainable cities. We present a machine-learning framework for portraying large-area high-resolution urban soundscapes using ubiquitous street view imagery(SVI), without ground measurements. This dataset includes two parts: (1) SVI visual features and soundscape indicators data; (2) field-measured SVI and noise intensity data.

### SVI visual features and soundscape indicators data
We also extract a total of 482 visual features from each imagery using computer vision algorithms and deep learning model. The extraction of visual features including: Object Detection(by [Faster R-CNN](https://pytorch.org/vision/stable/generated/torchvision.models.detection.fasterrcnn_resnet50_fpn.html#torchvision.models.detection.fasterrcnn_resnet50_fpn)), Semantic Segmentation(by [DeepLabV3P](https://github.com/PaddlePaddle/PaddleSeg)), and Scenes Classification(by [ResNet](https://pytorch.org/vision/stable/generated/torchvision.models.resnet50.html?highlight=resnet#torchvision.models.resnet50)
) features and low-level features by the algorithms from the [OpenCV](https://opencv.org/) library. Each imagery was labeled a total of **15 soundscape indicators** are divided into four categories:
* Noise intensity
* Sound quality
* Sound sources: traffic noise, human sounds, natural sounds, mechanical noise, and music noise
* Perceptual emotion: pleasant, chaotic, vibrant, uneventful, calm, annoying, eventful, and monotonous

<div align=center>
<img src="https://github.com/ualsg/Visual-soundscapes/blob/main/fig1.png" width="400px">
</div>

We invited a total of 338 people to participate in the survey via [Amazon Mechanical Turk](https://www.mturk.com/) and social media.

### Field-measured SVI and noise intensity data
The devices used in the collection include a Sound Level Meter(UT353BT) for noise intensity recording and a smartphone for the shooting of videos and street view imagery. Each investigation points include:
* Three-minute video clips
* 4-10 street view imageries
* Three-minute recording of variations in sound intensity 

<div align=center>
<img src="https://github.com/ualsg/Visual-soundscapes/blob/main/fig2.png" width="700px">
</div>

## Access

The raw SVI data can be dowmloaded at [figshare](https://figshare.com/s/2e7e23a20be112d828ea). The SVI visual features and soundscape indicators data can be found at *Label_Features*. The Field-measured SVI and noise intensity data can be downloaded at [figshare](https://figshare.com/s/2e7e23a20be112d828ea).

## Paper

A [paper](https://doi.org/10.1016/j.compenvurbsys.2022.101915) about the work was published in _Computers, Environment and Urban Systems_ and it is available open access.

If you use this work in a scientific context, please cite this article.

Zhao T, Liang X, Tu W, Huang Z, Biljecki F (2023): Sensing urban soundscapes from street view imagery. Computers, Environment and Urban Systems, 99: 101915. doi:10.1016/j.compenvurbsys.2022.101915

```
@article{2023_ceus_soundscapes,
  author = {Zhao, Tianhong and Liang, Xiucheng and Tu, Wei and Huang, Zhengdong and Biljecki, Filip},
  doi = {10.1016/j.compenvurbsys.2022.101915},
  journal = {Computers, Environment and Urban Systems},
  pages = {101915},
  title = {Sensing urban soundscapes from street view imagery},
  volume = {99},
  year = {2023}
}
```

## License
This dataset is released under the [CC BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/) license.

## Contact
Feel free to contact [Tianhong Zhao](https://ual.sg/authors/tianhong/)  or [Filip Biljecki](https://ual.sg/authors/filip/) should you have any questions.
For more information, please visit the website of the [Urban Analytics Lab](https://ual.sg/), National University of Singapore.

## Acknowledgements
We gratefully acknowledge the participants of the survey and the input data. We thank the members of the NUS Urban Analytics Lab for the discussions. The Institutional Review Board of the National University of Singapore has reviewed and approved the ethical aspects of this research (reference code NUS-IRB-2021-906).

