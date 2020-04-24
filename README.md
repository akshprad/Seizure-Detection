# Seizure-Detection
<b>Getting Started:</b>
<br>
Due to the size of these notebooks you may need to use nbviewer to view the notebooks. To do this all you need to do is copy the url for the notebook (e.g. https://github.com/akshprad/Seizure-Detection/blob/master/Pre_processing_%26_Feature_Engineering.ipynb) into the URL bar on the nbviewer website.
</br>

<b>Prerequisites:</b>
<br>
The easiest way of interacting with these notebooks is to use Google Colaboratory.
</br>

"Colaboratory allows you to use and share Jupyter notebooks with others without having to download, install, or run anything on your own computer other than a browser" (https://research.google.com/colaboratory/faq.html).

I recommend Google Colaboratory mostly because of the size of the RAM available and the access to GPU's via the cloud. When working on the later notebooks, which use the TensorFlow package, the notebook will be ran a tonne faster! You can open the notebook in Colaboratory by clicking on the "Open in Colab" button at the top of the notebook.
<br>

<b>Installing Packages:</b>
The notebooks start with a method to automatically install the required packages and data if using Google Colab. If working on these locally I encourage you to use a virtual environment. All you need to do is create a new environment and launch the Jupyter Notebook application from that environment (See http://docs.anaconda.com/anaconda/navigator/ for more information).

If you want to install the packages manually from command prompt (or Anaconda prompt) then install the following packages below.

<li>matplotlib</li>
<li>pandas</li>
<li>numpy</li>
<li>scipy</li>
<li>scikit-learn</li>
<li>umap-learn</li>
<li>imblearn</li>
<li>seaborn</li>
<li>mlxtend</li>
<li>mne</li>
<li>PyWavelets</li>
<li>Tensorflow</li>

<br>

<b>In this project 2 datasets have been used:</b>

1) <b><i>NEDC TUH Seizure Corpus:</b></i><br> The full TUH EEG corpus is the world’s largest publicly available corpus of clinical EEG data. The corpus contains 15,757 hours (56,726,510 secs) of EEG recordings from 13,539 patients. This paper uses a subset of the TUH corpus, the TUH EEG Seizure Corpus (v1.5.0), which has been manually annotated and separated into training and test sets, as well as split up into sessions with and without seizures1. The full training set contains 592 patients, 202 of which have seizures, for a total of 2370 seizures categorised into 9 types. The duration of all the seizures is 46.7 hours (168139.2295 secs) out of the full 752.3 hours (2708284 secs) of available EEG data. The test data is also large, with a total of 50 patients, 39 with seizures, 685 seizures (16.95hrs; 61036.8393 secs) and 170.34 hours (613232 secs) of data.

2) <b><i>The Epileptologie Database:</b></i><br> Five sets (denoted A–E) each containing 100 single-channel EEG segments of 23.6-sec duration, were composed for the study. These segments were selected and cut out from continuous multichannel EEG recordings after visual inspection for artifacts, e.g., due to muscle activity or eye movements. In addition, the segments had to fulfill a stationarity criterion described in detail in Sec. II B. Sets A and B consisted of segments taken from surface EEG recordings that were carried out on five healthy volunteers using a standardized electrode placement scheme. Volunteers were relaxed in an awake state with eyes open (A) and eyes closed (B) respectively. Sets C, D, and E originated from our EEG archive of presurgical diagnosis. For the present study EEGs from five patients were selected, all of whom had achieved complete seizure control after resection of one of the hippocampal formations, which was therefore correctly diagnosed to be the epileptogenic zone. Segments in set D were recorded from within the epileptogenic zone, and those in set C from the hippocampal formation of the opposite hemisphere of the brain. While sets C and D contained only activity measured during seizure free intervals, set E only contained seizure activity. Here segments were selected from all recording sites exhibiting ictal activity. All EEG signals were recorded with the same 128-channel amplifier system, using an average common reference [omitting electrodes containing pathological activity (C, D, and E) or strong eye movement artifacts (A and B)]. After 12 bit analog-to-digital conversion, the data were written continuously onto the disk of a data acquisition computer system at a sampling rate of 173.61 Hz. Band-pass filter settings were 0.53– 40 Hz (12 dB/oct.).  
