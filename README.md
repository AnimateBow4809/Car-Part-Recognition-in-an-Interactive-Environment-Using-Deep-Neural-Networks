# Car-Part-Recognition-in-an-Interactive-Environment-Using-Deep-Neural-Networks
This thesis presents a lightweight, car part classification model designed for interactive
image-based annotation tasks. Given a user-selected point or line on a car image, a local
image patch centered on the input location is extracted and passed to a neural network
for classification. The main motivation and usage of this work is to speed up the labeling
process during the annotation of different vehicle parts. The model uses an EfficientNet
backbone for feature extraction, followed by a simple multi-layer perceptron (MLP) head
to predict the class of the target point (e.g., front left tire, center points, edge points).
This approach avoids full-scene processing, focusing instead on relevant local context,
which significantly reduces computational cost while maintaining competitive accuracy.
Experiments on a custom dataset of annotated car part keypoints demonstrate that this
method is fast, simple to deploy, and effective for on-demand vehicle part identification
in real-world scenarios. In particular, the point-based model achieved a micro precision
of 0.88 , while the line-based model achieved 0.82 , highlighting the effectiveness of the
proposed approach across both interactive settings.
