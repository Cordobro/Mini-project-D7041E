# Mini-project-D7041E
This project aims to classify bird images and sounds using Convolutional Neural Networks (CNNs). The image dataset is sourced from Kaggle, a platform for sharing diverse datasets, while the bird sounds are obtained from xeno-canto, a global platform for sharing bird sound recordings. 

## Must contain
- Andreas Form 
- Group nr 10
- Mail: Formarn3@gmail.com
- Student-id: Forane-9
- Dataset for image https://www.kaggle.com/datasets/gpiosenka/100-bird-species 
- Dataset for sound https://xeno-canto.org/
- Complete dataset for sounds [drive](https://drive.google.com/drive/folders/1DxpEXlCTJc13DQlRF1Y0mBS9rMhDrddH?usp=sharing)

## BirdAI Project
This classification project is part of a larger project called BirdAI wich I worked at during this time period, which aims to develop an applied AI solution for bird species recognition. The BirdAI project encompasses both image and sound recognition for birds and has been transformed into a web application. If you are interested in the broader context and other components of the project, you can explore the full BirdAI website at https://99jessve.github.io./

Feel free to dive deeper into the BirdAI project to understand the overall scope and goals beyond the sound recognition component. 


## Import sounds
### Overview
The `Import_sounds` script is designed to download bird sound files in MP3 format from the Xeno-canto API. These sound files will be used for classifying bird species based on their vocalizations in the context of the applied AI project.

### Prerequisites
```bash
pip install requests
```

### Dependencies
- [Requests](https://pypi.org/project/requests/): A Python library for making HTTP requests.


## Resize_sound
### Overview
The `Resize_sound` script is designed to standardize bird sound files to a fixed length of 10 seconds. It's an essential step in preparing the dataset for the applied AI project, ensuring uniformity in the duration of bird vocalizations.

### Prerequisites
```bash
pip install moviepy
```

### Dependencies
- [MoviePy](https://pypi.org/project/moviepy/): Python library for video editing.


## Create_spectogram
### Overview
The `Create_spectogram` script is responsible for converting shortened bird audio files into spectrogram images. Spectrograms visually represent the frequencies present in an audio signal over time, providing valuable insights for the applied AI project's bird species recognition.

### Prerequisites
```bash
pip install matplotlib
pip install librosa
```

### Dependencies
- [Matplotlib](https://pypi.org/project/matplotlib): A Python plotting library.
- [Librosa](https://pypi.org/project/librosa): A Python package for music and audio analysis.

## Spectogram_classification
### Overview
The `Create_spectogram` script is responsible for converting shortened bird audio files into spectrogram images. Spectrograms visually represent the frequencies present in an audio signal over time, providing valuable insights for the applied AI project's bird species recognition.

### Prerequisites
```bash
pip install scikit-learn
pip install scipy

```

### Dependencies
- [Matplotlib](https://pypi.org/project/matplotlib): A Python plotting library.
- [Librosa](https://pypi.org/project/librosa): A Python package for music and audio analysis.

## Accuracy for 9 different sounds with 1 hidden layer

| Learning rate | Accuracy | F1-Score | Precision | Recall |
| ------------- |----------| -------- |---------- |--------|
| 0.001         |   76.0%  |   76%    |    76%    |   76%  |
| 0.005         |   76.3%  |   76%    |    77%    |   76%  |
| 0.01          |   77.8%  |   78%    |    78%    |   78%  |
| 0.05          |   76.1%  |   77%    |    78%    |   76%  |
| 0.1           |   78.4%  |   78%    |    79%    |   78%  |
| 0.5           |   76.0%  |   76%    |    77%    |   76%  |

## Accuracy for 9 different sounds with 3 hidden layer

| Learning rate | Accuracy | F1-Score | Precision | Recall |
| ------------- |----------| -------- |---------- |--------|
| 0.001         |   76.5%  |   75%    |    77%    |   74%  |
| 0.005         |   76.6%  |   77%    |    77%    |   77%  |
| 0.01          |   75.1%  |   75%    |    75%    |   75%  |
| 0.05          |   76.7%  |   77%    |    77%    |   77%  |
| 0.1           |   76.6%  |   77%    |    78%    |   77%  |
| 0.5           |   77.2%  |   77%    |    78%    |   77%  |