
# Requirements

1. Install docker:

    * [docker](https://www.docker.com/products/docker-toolbox)


# Usage

1. Clone this repository

    git clone https://github.com/rostiq/tf_image.git

2. Start the docker image:

    docker run -it --volume ${HOME}/tf_image:/tf_image  --workdir /tf_image tensorflow/tensorflow:1.1.0 bash

3. Run retrain.py for training

    python retrain.py --bottleneck_dir=bottlenecks --model_dir=inception --summaries_dir=training_summaries/long --output_graph=retrained_graph.pb --output_labels=retrained_labels.txt --image_dir=images

4. Run the label_image.py:

    python label_image.py images/panda/image_0032.jpg

