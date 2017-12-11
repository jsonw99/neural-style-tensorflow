## The implement of neural-style in tensorflow
This is an implementation of [Image Style Transfer Using Convolutional Neural Networks](https://www.cv-foundation.org/openaccess/content_cvpr_2016/papers/Gatys_Image_Style_Transfer_CVPR_2016_paper.pdf). The original post can be found [here]( https://github.com/cysmith/neural-style-tf), by @cysmith. <br />
The code had been tested with python3.5.

### 1. preparation
Download the [VGG-19 model weights](http://www.vlfeat.org/matconvnet/models/imagenet-vgg-verydeep-19.mat). And save it to the root folder of the project directory. 

### 2. Rendering a single image
```bash
python my_neural_style.py \
--content_img golden_gate.jpg \
--style_imgs wave.jpg \
--max_size 1000 \
--max_iterations 100 \
--device /cpu:0 \
--verbose

```
The result image file will use saved in the directory "./image_output/".
