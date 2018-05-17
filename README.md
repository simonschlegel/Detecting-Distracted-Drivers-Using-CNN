
# Detecting Distracted Drivers Using A Convolutional Nueral Network.

## Team Members:
## Simon Schlegel

# Overview
The purpose is to build a machine learning model to recognize when a driver is distracted based on a dashboard image.
This can be used to alert the driver and reduce accidents.
This project uses the StateFarm Distracted Driver data set posted on Kaggle.
https://www.kaggle.com/c/5048/download/imgs.zip
It includes 22424 dashboard images of drivers sitting in the front seat. Each image is labeled into one of 10 classes. The classes are safe, texting-right, texting-left, talking on phone-right, talking on phone-left, using radio, drinking, reaching back, hair or makeup, and talking to passenger. I randomly split 25% of the data for testing and the other 75% for training. I use Keras Image Preprocessing Image Generators to randomly augment the training images in realtime to provide more unique examples. A convolutional nueral network is used to learn relevant features of the image useful for the classification task. The model is evaluated using the test set, and accuracy metrics are produced for each class.
Using 32x32 rescaled images, the model produced training accuracy of 91% and a test accuracy of 90%.
Using 64x64 rescaled images, the model produced training accuracy of 98% and a test accuracy of 97%.

## How to run code:
After installing requirements and downloading jupyter notebook and imgs dataset, run the notebook using a jupyter notebook instance.

To download data...
Use this link:  https://www.kaggle.com/c/5048/download/imgs.zip


Video demo link:

Requirements list:
absl-py==0.1.12
appnope==0.1.0
astor==0.6.2
bleach==1.5.0
boto==2.48.0
boto3==1.7.14
botocore==1.10.14
bz2file==0.98
certifi==2018.4.16
chardet==3.0.4
cycler==0.10.0
decorator==4.2.1
docutils==0.14
entrypoints==0.2.3
gast==0.2.0
gensim==3.4.0
grpcio==1.10.0
h5py==2.7.1
html5lib==0.9999999
idna==2.6
ipykernel==4.8.2
ipython==6.2.1
ipython-genutils==0.2.0
ipywidgets==7.1.2
jedi==0.11.1
Jinja2==2.10
jmespath==0.9.3
jsonschema==2.6.0
jupyter==1.0.0
jupyter-client==5.2.3
jupyter-console==5.2.0
jupyter-core==4.4.0
Keras==2.1.5
kiwisolver==1.0.1
Markdown==2.6.11
MarkupSafe==1.0
matplotlib==2.2.2
mistune==0.8.3
nbconvert==5.3.1
nbformat==4.4.0
nltk==3.2.5
notebook==5.4.1
numpy==1.14.2
opencv-python==3.4.0.12
pandas==0.22.0
pandocfilters==1.4.2
parso==0.1.1
pexpect==4.4.0
pickleshare==0.7.4
Pillow==5.0.0
prompt-toolkit==1.0.15
protobuf==3.5.2.post1
ptyprocess==0.5.2
Pygments==2.2.0
pyparsing==2.2.0
python-dateutil==2.7.0
pytz==2018.3
PyYAML==3.12
pyzmq==17.0.0
qtconsole==4.3.1
requests==2.18.4
s3transfer==0.1.13
scikit-learn==0.19.1
scipy==1.0.0
Send2Trash==1.5.0
simplegeneric==0.8.1
simplejson==3.13.2
six==1.11.0
sklearn==0.0
smart-open==1.5.7
tensorboard==1.6.0
tensorflow==1.6.0
termcolor==1.1.0
terminado==0.8.1
testpath==0.3.1
tornado==5.0.1
tqdm==4.21.0
traitlets==4.3.2
urllib3==1.22
wcwidth==0.1.7
webencodings==0.5.1
Werkzeug==0.14.1
widgetsnbextension==3.1.4
