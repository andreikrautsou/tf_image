
# Requirements

1. Install docker:

https://www.docker.com/products/docker-toolbox

2. Install TensorFlow:

https://www.tensorflow.org/install/

# Usage

1. Clone this repository

2. Start the docker image:

docker run -it --volume ${HOME}/tf_img:/tf_img  --workdir /tf_img tensorflow/tensorflow:1.1.0 bash

3. Run the label_image.py:

python label_image.py animals_photos/crocodile/image_0001.jpg 

