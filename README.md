
# Requirements

1. Install docker:

* [docker](https://www.docker.com/products/docker-toolbox)


# Usage

1. Clone this repository

2. Start the docker image:

docker run -it --volume ${HOME}/tf_img:/tf_img  --workdir /tf_img tensorflow/tensorflow:1.1.0 bash

3. 

python retrain.py --bottleneck_dir=bottlenecks --model_dir=inception --summaries_dir=training_summaries/long --output_graph=retrained_graph.pb --output_labels=retrained_labels.txt --image_dir=[path_to_dir]

4. Run the label_image.py:

python label_image.py [path_to_photo]

