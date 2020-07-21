# English-Accent-Modeling-with-Siamese-CNNs

Deep-Learning-based audio project for modeling the native language, sex, and age of speakers using regular & siamese 1-D CNNs.

The dataset is the Speech Accent Archive ([Data can be found here](https://www.kaggle.com/rtatman/speech-accent-archive)). It contains 2140 speech samples of different speakers reading the same english passage. The dataset includes speakers from 177 countries (214 native languages).

Main technologies: Python -> Keras, Scikit-learn, Pandas, Numpy, SciPy, Librosa, Seaborn, and Plotly.


This project is divided as follows:

1. Literature Review -> Overview of the acoustic field with a special focus on audio generation (WaveGAN, GANSynth, DDSP) and speaker recognition (SincNet, d-vectors, x-vectors).

2. Project Description -> Brief description of project's goal, dataset, and methodology.

3. Exploratory Data Analysis (EDA) -> Two types of EDA were developed. First, an analysis of speakers' age, sex, native language looking at correlation and distributions. Second, an analysis of speakers' audio features using raw audios, MFCCs, log-mel spectograms, and chromas.

4. Data Preprocessing -> Audio feature extraction using raw audios, VGGish embeddings (d-vectors), MFCCs, log-mel spectograms, and chromas. Data augmentation using noise injection, time shifting, and speed variations.

5. Deep Learning Modeling ->  Classification models were developed for the speakers' features age, sex, and native language using regular & siamese 1-D CNNs. The five types of feature extraction techniques were tested for the two DL models and the three modeled features.

6. Results -> Regular CNN models were evaluated with accuracy and F1-score and the siamese CNNs with N-way one-shot learning.

7. Conclusions -> Speakers' sex models yielded almost perfect results. Speakers' age models yielded good results but far from perfect. Speakers' native language models yielded modest results (with the exception of models focused on english vs. non-english native speakers). Regular CNNs gave slightly better scores but seemed less robust than siamese CNNs.

You can find the full documentation in docs. 

Developed in Google Colab.

Project proposed also for the subject Deep Learning for Acoustic Signal Processing (DLAS). ETSIT-UPM.
