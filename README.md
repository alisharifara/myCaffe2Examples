# Caffe2 Examples

Caffe2 is an open-source deep learning framework. It's focus is on efficiency and works with constrained environments such as on mobile devices.

1. Blobs and operations
2. Operators and Net
3. Simple Linear Regression (on one feature of Boston Dataset)
4. Classification using Caffe2
5. Image pre-processing pipeline
6. Prediction using pretrained models


# Prerequisites

Install Caffe2 with Python bindings.


# Download

To download a model locally, run

`python -m caffe2.python.models.download squeezenet`

which will create a folder squeezenet/ containing both an init_net.pb and predict_net.pb.

# Install

To install a model, run

`python -m caffe2.python.models.download -i squeezenet`

which will allow later imports of the model directly in Python:

`from caffe2.python.models import squeezenet
 print(squeezenet.init_net.name)
 print(squeezenet.predict_net.name)
`

