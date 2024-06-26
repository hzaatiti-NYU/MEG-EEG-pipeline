![MNE-Python Logo](https://mne.tools/stable/_static/mne_logo.svg "MNE-Python")

# MEG-EEG-pipeline


## Preparations

You need to set up a Python environment with a number of dependencies. The following instructions will guide you through the process.

### Download & install Anaconda

We work with the Anaconda Python distribution.

- [Installation instructions for Windows](https://docs.continuum.io/anaconda/install/windows/)
- [Installation instructions for macOS](https://docs.continuum.io/anaconda/install/mac-os/)
- [Installation instructions for Linux](https://docs.continuum.io/anaconda/install/linux/)

### Install MNE-Python

- [Open an Anaconda prompt](https://docs.continuum.io/anaconda/install/verify-install/#conda)
- Follow the [MNE-Python installation instructions for your operating system](https://mne.tools/stable/install/mne_python.html#for-3d-plotting-and-source-analysis)
- Activate your newly-installed MNE-Python environment by typing into the Anaconda prompt:
  ```
  conda activate mne
  ```
- Verify your MNE-Python installation by running in the Anaconda prompt:
  ```
  mne sys_info
  ```
  The output should look similar to the following:
  ```
    Platform:      macOS-10.15.7-x86_64-i386-64bit
    Python:        3.8.5 (default, Sep  4 2020, 02:22:02)  [Clang 10.0.0 ]
    Executable:    /Users/richard/miniconda3/envs/mne-new/bin/python
    CPU:           i386: 4 cores
    Memory:        8.0 GB

    mne:           0.21.1
    numpy:         1.19.2 {blas=mkl_rt, lapack=mkl_rt}
    scipy:         1.5.2
    matplotlib:    3.3.2 {backend=MacOSX}

    sklearn:       0.23.2
    numba:         0.51.2
    nibabel:       3.2.0
    cupy:          Not found
    pandas:        1.1.3
    dipy:          1.3.0
    mayavi:        4.7.2
    pyvista:       0.27.2 {pyvistaqt=0.2.0, OpenGL 4.1 INTEL-14.7.8 via Intel HD Graphics 5000 OpenGL Engine}
    vtk:           9.0.1
    PyQt5:         5.13.2
    ```

### Install JupyterLab

We will use the Jupyter Lab environment to run our notebooks. Inside the Anaconda prompt, run:
```
conda activate mne
conda install -y jupyterlab
```

Then, run:
```
jupyter lab
```
If the installation was successful, your browser should open. You may close it again, and stop the JupyterLab process in the Anaconda prompt by pressing the keys `Ctrl` and `C` simultaneously and then enterying `y` when asked if you're sure.


## Pipline summary

The pipline cover a broad range of topics to help you get to know all essential parts for conducting MEG and EEG data analysis:

- loading, filtering, and inspecting raw data
- epoching and artifact correction
- creating and visualizing evoked responses (ERP / ERF)
- decoding neural responses (machine learning)
- performing time-frequency analysis
- estimating and visualizing cortical sources (source localization)
