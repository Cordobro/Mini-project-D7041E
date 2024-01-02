# Mini-project-D7041E
This project aims to classify bird sounds using Convolutional Neural Networks (CNNs). The dataset is sourced from xeno-canto, a platform for sharing bird sound recordings worldwide. The sounds are preprocessed into spectrograms, and a CNN model is trained for accurate classification.


## BirdAI Project
This classification model is part of a larger project called BirdAI, which aims to develop an applied AI solution for bird species recognition. The BirdAI project encompasses both image and sound recognition for birds and has been transformed into a web application. If you are interested in the broader context and other components of the project, you can explore the full BirdAI repository at https://github.com/TovahParnes/BirdAI_D7057E.

Feel free to dive deeper into the BirdAI project to understand the overall scope and goals beyond the sound recognition component.


## Import sounds
### Overview
The `Import_sounds` script is designed to download bird sound files in MP3 format from the Xeno-canto API. These sound files will be used for classifying bird species based on their vocalizations in the context of the applied AI project.

### Prerequisites
Before running the script, make sure to install the required dependencies using the following command:

```bash
pip install requests
```

### Dependencies
- [Requests](https://pypi.org/project/requests/): A Python library for making HTTP requests.

### Notes
- Ensure that you have a stable internet connection before running the script to download bird sound files from the Xeno-canto API.


## Resize_sound
### Overview
The `Resize_sound` script is designed to standardize bird sound files to a fixed length of 10 seconds. It's an essential step in preparing the dataset for the applied AI project, ensuring uniformity in the duration of bird vocalizations.

### Prerequisites
Ensure you have the required dependency installed:

```bash
pip install moviepy
```

### Dependencies
- [MoviePy](https://pypi.org/project/moviepy/): Python library for video editing.

### Notes
- The script will automatically process all MP3 files in the specified directory, resizing them to 10 seconds.

- If a sound file is longer than 10 seconds, the script will trim it to the first 10 seconds.

- If a sound file is shorter than 10 seconds, the script will repeat the sound until it reaches the desired length.


## Create_spectogram
### Overview

The `Create_spectogram` script is responsible for converting shortened bird audio files into spectrogram images. Spectrograms visually represent the frequencies present in an audio signal over time, providing valuable insights for the applied AI project's bird species recognition.

### Prerequisites

Before running the script, make sure to install the required dependencies using the following commands:

```bash
pip install matplotlib
pip install librosa
```

### Dependencies
- [Matplotlib](https://pypi.org/project/matplotlib): A Python plotting library.
- [Librosa](https://pypi.org/project/librosa): A Python package for music and audio analysis.

### Notes
- The script converts shortened bird audio files into spectrogram images, providing a visual representation of frequencies over time.

- Spectrograms are useful for extracting features relevant to bird species recognition.

## Accuracy

| Learning rate | Accuracy |
| ------------- |----------|
| 0.001         |   41.5%  |
| 0.01          |    |
| 0.005         |  |


## Images

![Accuracy](https://github.com/Cordobro/Mini-project-D7041E/blob/main/images/lr%3D0.001_accuracy.png)

![Loss](https://github.com/Cordobro/Mini-project-D7041E/blob/main/images/lr%3D0.001_loss.png)