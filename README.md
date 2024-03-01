# Ravdess
Data understanding, Clustering and Classification of a dataset created from the RAVDESS dataset <br />

This dataset was created from the RAVDESS dataset (https://es.sonicurlprotection-fra.com/click?PV=2&MSGID=202209141411100289250&URLID=1&ESV=10.0.18.7423&IV=CDD893A9D96AB6D6469DFBAF03B52C7A&TT=1663164671774&ESN=SJ44mpH7HPEgdwadIHqGKE9aHAKB%2FGfCfiESv9Jnnj4%3D&KV=1536961729280&B64_ENCODED_URL=aHR0cHM6Ly96ZW5vZG8ub3JnL3JlY29yZC8xMTg4OTc2KSw&HK=3428F8A9C48043894424396B826370722E127A5AEC482B778236DC3B3D0A300B extracting basic statistics (mean, std, min, max, etc.) from the original audio data and after transforming it using: zero-crossing rate, Mel-Frequency Cepstral Coefficients, spectral centroid, and the stft chromagram. Features were extracted from the 2452 wav files. <br />

## Data understanding
Data semantics <br />
Distribution of the variables and statistics <br />
Assessing data quality (missing values, outliers) <br />
Variables transformations <br />
Pairwise correlations and eventual elimination of redundant variables <br />

## Clustering
Clustering Analysis by K-means <br />
Choice of attributes and distance function <br />
Identification of the best value of k <br />
Characterization of the obtained clusters by using both analysis of the k centroids and comparison of the distribution of variables within the clusters and that in the whole dataset <br />
Analysis by density-based clustering <br />
Choice of attributes and distance function <br />
Study of the clustering parameters <br />
Characterization and interpretation of the obtained clusters <br />
Analysis by hierarchical clustering <br />
Choice of attributes and distance function <br />
Show and discuss different dendograms using different algorithms <br />
Final evaluation of the best clustering approach and comparison of the clustering obtained <br />

## Classification
Learning of different decision trees with different hyper-parameters with the object of maximizing the performances <br />
Decision trees interpretation, validation with test and training set <br />
Training of different KNN classifiers with different parameters with the object of maximizing the performances <br />
Training of different RandomFOrests, SVM with different parameters with the object of maximizing the performances <br />
Discussion of the best prediction model

## Dataset description
### Features:
modality (audio-only) <br />
vocal_channel (speech, song) <br />
emotion (neutral, calm, happy, sad, angry, fearful, disgust, surprised) <br /> 
emotional_intensity (normal, strong). NOTE: There is no strong intensity for the 'neutral' emotion <br />
statement ("Kids are talking by the door", "Dogs are sitting by the door") <br />
repetition (1st repetition, 2nd repetition) <br />
actor (01 to 24) <br />
sex (M, F) <br />
channels (number of channels; 1 for mono, 2 for stereo audio) <br />
sample_width (number of bytes per sample; 1 means 8-bit, 2 means 16-bit) <br />
frame_rate (frequency of samples used (in Hertz)) <br />
frame_width (Number of bytes for each frame. One frame contains a sample for each channel.) <br />
length_ms (audio file length (in milliseconds)) <br />
frame_count (the number of frames from the sample) <br />
intensity (loudness in dBFS (dB relative to the maximum possible loudness)) <br />
zero_crossings_sum (sum of the zero-crossing rate) <br />
'mean', 'std', 'min', 'max', 'kur', 'skew' (statistics of the original audio signal) <br />
mfcc_ 'mean', 'std', 'min', 'max' (statistics of the Mel-Frequency Cepstral Coefficients) <br />
sc_ 'mean', 'std', 'min', 'max', 'kur', 'skew' (statistics of the spectral centroid) <br />
stft_ 'mean', 'std', 'min', 'max', 'kur', 'skew' (statistics of the stft chromagram) <br />