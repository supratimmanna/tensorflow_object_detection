# tensorflow_object_detection
This repo describes how to train the tensorflow object detection api using your own **custom data**.

#### Requirements to use the tensorflow object detection api are following:
* Anaconda Python 3.7
* TensorFlow
* Protobuf
* TensorFlow Object Detection API
* LabelImg

  

> **Install Anaconda Python 3.7**

* Go to [Official Website of Anaconda](https://www.anaconda.com/products/individual) and click the “Download” button.
* Download the Python 3.7 64-Bit Graphical Installer or the 32-Bit Graphical Installer installer, per your system requirements.
* Run the downloaded executable (.exe) file to begin the installation. See [here](https://docs.anaconda.com/free/anaconda/install/windows/) for more details.
* Create a new virtual environment for your work and activate the virtual environment.
```
conda create -n tensorflow pip python=3.8
conda activate tensorflow
```

> **Install TensorFlow**

Run the following command to install tensorflow:
```
pip install --ignore-installed --upgrade tensorflow==2.2.0
```

> **Install Protobuf**

Run the following command to install tensorflow:
```
pip install protobuf
```

Run the following command in a new terminal to check the installation of tensorflow.
```
python -c "import tensorflow as tf;print(tf.reduce_sum(tf.random.normal([1000, 1000])))"
```

> **TensorFlow Object Detection API Installation**
1. Step 1:
   
* Create a new folder under a path of your choice and name it TensorFlow. (e.g. C:\Users\sglvladi\Documents\TensorFlow).

* From your Terminal **_cd_** into the TensorFlow directory.

* To download the models you can either use Git to clone the TensorFlow Models repository inside the TensorFlow folder, or you can simply download it as a ZIP and extract its contents inside the TensorFlow folder. To keep things consistent, in the latter case you will have to rename the extracted folder **models-master** to **models**.

* You should now have a single folder named models under your TensorFlow folder, which contains another 4 folders as such:
```
TensorFlow/
└─ models/
   ├─ community/
   ├─ official/
   ├─ orbit/
   ├─ research/
   └── ...
```
