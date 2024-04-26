# MEG-EEG-pipeline

Plotting 2D sensor locations
![image](https://github.com/hzaatiti-NYU/MEG-EEG-pipeline/assets/29655962/b0b6393d-f36d-4e30-b653-a3b38895c2a2)


Plotting events
We used the function mne.viz.plot_events() which plot each event versus its time (we provide the sampling frequency, so that it plot them versus time in seconds):

![Figure_1](https://github.com/hzaatiti-NYU/MEG-EEG-pipeline/assets/29655962/337bc883-14e4-450a-ae49-285681dc29cf)

Compute the power spectral density (PSD) using Morlet wavelets
![Figure_1](https://github.com/hzaatiti-NYU/MEG-EEG-pipeline/assets/29655962/eb5bf5e9-fdd6-408d-bd0f-135e6cc76831)


Epochs objects have a built-in plotting method a plot_image, which shows each epoch as one row of an image map, with color representing signal magnitude; the average evoked response and the sensor location are shown below the image:
![image](https://github.com/hzaatiti-NYU/MEG-EEG-pipeline/assets/29655962/fe3e70c2-f20f-481f-870f-f4a7c353ad2b)
![image](https://github.com/hzaatiti-NYU/MEG-EEG-pipeline/assets/29655962/6d75f870-5cd8-4bb8-9458-78f7003e2ea4)

Average power of eyes closed and eyes open
![image](https://github.com/hzaatiti-NYU/MEG-EEG-pipeline/assets/29655962/71dad2e5-3515-4772-9931-40effb7e18ba)

Exploring the frequency content of our eyes closed epochs
![image](https://github.com/hzaatiti-NYU/MEG-EEG-pipeline/assets/29655962/c1814b86-25a6-432e-9ac6-c35ed89215c6)

Exploring the frequency content of our eyes open epochs
![image](https://github.com/hzaatiti-NYU/MEG-EEG-pipeline/assets/29655962/2b81da83-efc5-4d18-a88b-f3cba05fe6d7)


