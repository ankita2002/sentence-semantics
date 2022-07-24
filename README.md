# sentence-semantics

This project makes use of Random Forest to check if two sentences are similar or not. It has been trained on Quora Question Pair dataset at [Kaggle](https://www.kaggle.com/c/quora-question-pairs).

## Installation and Usage
1. Clone the repository.
```
git clone https://github.com/ankita2002/sentence-semantics.git
```

2. Install Python dependencies (recommended to create a virtual environment using `python -m venv env`)
```
pip install -r requirements.txt
```

3. Download the trained model `dqi.pickle` from [Google Drive](https://drive.google.com/drive/folders/1qNPsdXuqU1m1_Y5mqyBsN--fakmngfX_?usp=sharing). Save it in directory `/bin/dqi.pickle` of the project's root.

4. Run the application
```
python app.py
```

The server should be running on [127.0.0.1:8000](http://127.0.0.1:8000).

## Examples

### Similar sentences
![similar](https://i.imgur.com/YFEB80w.jpg)

### Not similar sentences
![not similar](https://i.imgur.com/iAp8xMQ.jpg)

## Dataset
The dataset is downloaded from Kaggle. 

## Training

The Random Forest Model training steps can be found in `Model_Building.ipynb`. The csv file from Kaggle underwent data cleaning for which steps can be found in `DQI_feature_extraction.ipynb`. The resultant csv file can also be downloaded from [Google Drive](https://drive.google.com/drive/folders/1qNPsdXuqU1m1_Y5mqyBsN--fakmngfX_?usp=sharing) named as `final_train.csv`.

## Technologies used

* NumPy
* Pandas
* Keras
* Tensorflow
* NLTK
* Jupyter Notebook and Google Collab
* Flask
* Bootstrap