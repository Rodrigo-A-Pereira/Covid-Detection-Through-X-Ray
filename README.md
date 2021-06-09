# COVID-19-detection-through-X-Ray-chest-images

This repository contains the notebooks used in the development of the study "COVID-19 detection through X-Ray chest images
" wich explores the use of Deep Convolutional Neural Networks in order to identify Covid-19 cases based based on frontal chest X-Ray images.

## Data
Covid-19 cases X-Ray images were obtained form the [Italian Society of Medical
and Interventional Radiology website](https://www.sirm.org/category/senzacategoria/covid-19/).

Non-Covid cases images where obtained from the [ChexPert dataset](https://stanfordmlgroup.github.io/competitions/chexpert/) provided by Standford University's ML group.

## Architectures Used

Given the samll number of Covid-positive we had to work wit, Transefer Learning was one of the best approaches available. As such we used pretrained ResNet50 and VGG16 models traied with ImageNet, froze the parameters and added a final group of trainable dense layers.

VGG16                      |  ResNet50
:-------------------------:|:-------------------------:
![](https://github.com/Rodrigo-A-Pereira/COVID-19-detection-through-X-Ray-chest-images/blob/main/VGG16.png)                      |  ![](https://github.com/Rodrigo-A-Pereira/COVID-19-detection-through-X-Ray-chest-images/blob/main/ResNet50.png)

## Citation 
If you have found this studies useful in your work, please consider citing our [paper](https://doi.org/10.1109/ICAI50593.2020.9311372)

```bibtex
@INPROCEEDINGS{9311372,
  author={Hernandez, Diego and Pereira, Rodrigo and Georgevia, Petia},
  booktitle={2020 International Conference Automatics and Informatics (ICAI)}, 
  title={COVID-19 detection through X-Ray chest images}, 
  year={2020},
  volume={},
  number={},
  pages={1-5},
  doi={10.1109ICAI50593.2020.9311372}}
  ```
