# SRCNN-dicom
[SRCNN-Tensorflow](https://github.com/tegg89/SRCNN-Tensorflow)의 코드에서 data load 부분을 dicom 파일을 읽을 수 있도록 바꾼 코드입니다.  
또한, [Image Super-Resolution Using Deep Convolutional Networks](https://arxiv.org/pdf/1501.00092.pdf) 논문을 바탕으로 하고 있습니다.  

## Prerequisites
 * Tensorflow
 * Scipy version > 0.18 ('mode' option from scipy.misc.imread function)
 * h5py
 * matplotlib

This code requires Tensorflow. Also scipy is used instead of Matlab or OpenCV. Especially, installing OpenCV at Linux is sort of complicated. So, with reproducing this paper, I used scipy instead. For more imformation about scipy, click [here](https://www.scipy.org/).

## Data
`/train` 에 train data를 넣고, 
`/test/Set15` 에 test data를 넣으면 됩니다.  
결과는 `/Sample`에 저장됩니다.

## Usage
train을 시킬 시에는 `python main.py` 를 입력하고,
<br>
test 시에는 `python main.py --is_train=False --stride 21`를 입력합니다.  

## References
* [liliumao/Tensorflow-srcnn](https://github.com/liliumao/Tensorflow-srcnn) 
<br>

* [carpedm20/DCGAN-tensorflow](https://github.com/carpedm20/DCGAN-tensorflow) 
<br>

* [SRCNN-Tensorflow](https://github.com/tegg89/SRCNN-Tensorflow)
