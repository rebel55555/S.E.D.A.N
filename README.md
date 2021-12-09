
# SEDAN
 Our project is based on the idea of detecting different emotions from a range of different audio files. Our primary focus is to > detect a variety of basic human emotions such as happiness, sadness, anger, disgust, etc.

The main objective of our project is to distinguish between the various emotions and implement the different models used for the same.



## Download data files from Kaggle

```bash
!pip install -q kaggle
```
Upload the kaggle.json file which is generated for your Kaggle account for your profile.
```bash
from google.colab import files
files.upload()
```

Make directory for kaggle and change the accessibility rights for the colab user using below commands:
```bash
! mkdir ~/.kaggle
! cp kaggle.json ~/.kaggle/
! chmod 600 ~/.kaggle/kaggle.json
```

Source of Dataset we used and code snippet to download and unzip it on your drive:

```bash
!kaggle datasets download -d uwrfkaggler/ravdess-emotional-speech-audio --force
from google.colab import drive
drive.mount('/content/drive')
!unzip -u /content/ravdess-emotional-speech-audio.zip -d /content/drive/MyDrive/Projects/RAVDESS/
```

Or you can save efforts and download our [Data_download_file.ipynb](https://github.com/S-E-D-A-N/src/blob/main/Data_download_file.ipynb) and run it.



## Running SEDAN

### For 1D - CNN

You can download and use the file [SEDAN_CNN.ipynb](https://github.com/S-E-D-A-N/src/blob/main/SEDAN_CNN.ipynb)

### For other models

You can download and use the file [Final_SEDAN.ipynb](https://github.com/S-E-D-A-N/src/blob/main/Final_SEDAN.ipynb)
