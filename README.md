## This repository is aimed to compare simple classification model performance using tensorflow inference and openvino inference


### Requirement
1. Install openvino toolkit from https://docs.openvinotoolkit.org/latest/_docs_install_guides_installing_openvino_apt.html.
2. Clone this repository https://github.com/muhammadsyahyas/masked-face-image-classification to get simple classification model.
3. Install tensorflow==1.15.*


### Steps
1. Freeze keras model using code on freeze_keras_model.ipynb (obtaining pb file)
2. Convert frozen model (pb file) to beintermediary representative (IR) model by follow instruction on https://docs.openvinotoolkit.org/latest/_docs_MO_DG_prepare_model_convert_model_Convert_Model_From_TensorFlow.html
3. Do inference for two kind of batches using code on local_inference.ipynb