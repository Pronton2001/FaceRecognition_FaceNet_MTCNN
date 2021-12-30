# FaceNet_MTCNN

Face recognition using FaceNet and MTCNN
[Link to github](https://github.com/Pronton2001/FaceRecognition_FaceNet_MTCNN)

## Work flow

* Processing and training stages: `src/facenet_keras_preprocessing_and_embeddings.ipynb`. All of the result are stored in foler `EmbeddingFace` and `NumpyFace`.

* Classification stage: `src/facenet_keras_recognition.ipynb`.

## Download the dataset for preprocessing and training stages (Optional)

The dataset used in this project are:

* [Yale](http://vision.ucsd.edu/content/yale-face-database)
* [Yale B+](http://vision.ucsd.edu/data#:~:text=Extended%20Yale%20Face%20Database%20B%20%28B%2B%29%20The%20extended,the%20same%20as%20the%20Yale%20Face%20Database%20B.)

* [5-celebrity-faces-dataset](https://www.kaggle.com/dansbecker/5-celebrity-faces-dataset)
* [AT&T](https://www.kaggle.com/kasikrit/att-database-of-faces)

After downloading, navigate them into folder `data/`.

## Run the experiment with Google Colab (Recommended)

Clone this repository
```
from google.colab import drive
drive.mount('/content/drive')

%cd gdrive/My Drive/project_folder
!git clone https://github.com/Pronton2001/FaceRecognition_FaceNet_MTCNN
```

At the begin of 2 notebook, add:

```
from google.colab import drive
drive.mount('/content/drive')

%cd gdrive/My Drive/project_folder
%cd src/
```

Since GG colab have almost all the required library that we needed, we only need to install `mtcnn` at the beginning of `src/facenet_keras_preprocessing_and_embeddings.ipynb`:

```
!pip install mtcnn
```


## Run the experiment with virtual env Anaconda

### Install the requirement using virtual env Anaconda

```
conda create --name face python=3.9
conda activate face
pip install -r requirements.txt
```

### Run the experiment

* Download jupyter-notebook or jupyter-lab
* Run the 2 notebooks

## Quick test

Just run `facenet_keras_recognition.ipynb` for testing the classification performance. Ignore the preprocessing and training stage.
