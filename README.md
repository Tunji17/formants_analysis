# Formant Analysis with Python and Praat

## Data structure

The code expects a specific organization of your data. It expects that:

1) Each recording is a phonetically-balanced sentence. You are to record 3 sentences in the language of your choice.

2) You have created a folder for each of your audio recordings, formant files, f0 files and text files.
 
3) You have one textgrid file per recording, and the textgrid file has the same name as the corresponding utterance (excluding the extension).

4) All of your textgrid files have at least one phoneme tier. The name depends on your recording method.

5) You collected the formants and f0 following the process that was shown to you in class.

6) You have one formants file and one f0 file per recording stored as a csv file, and the files are named similar to the audio files in their respective folders.

7) The data is stored in the following directory structure. **If it is not your case, the code will not work**. You will have to make the necessary changes to make it work.

    ```
   speech_corpora
   ├── Formants_Analysis.ipynb
   ├── README.md
   ├── data
   │   ├── audio
   │   │   ├── ara.wav
   │   │   ├── iri.wav
   │   │   └── uru.wav
   │   ├── formants
   │   │   ├── ara.txt
   │   │   ├── iri.txt
   │   │   └── uru.txt
   │   ├── pitch
   │   │   ├── ara.txt
   │   │   ├── iri.txt
   │   │   └── uru.txt
   │   ├── text
   │   │   ├── ara.txt
   │   │   ├── iri.txt
   │   │   └── uru.txt
   │   └── textgrid
   │       ├── ara.TextGrid
   │       ├── iri.TextGrid
   │       └── uru.TextGrid
   └── requirements.txt
    ```


## How to run?

1) Create a virtual environment to separate the packages used in this project. To use venv, run

    ```bash
        >> python3 -m venv .speech_corpora_env
    ```

    To use conda, run

    ```bash
        >> conda create -n "speech_corpora" python=3.8
    ```

1) Activate your virtual environment:

    Linux and Mac:

    ```bash
    >> source .speech_corpora_env/bin/activate
    ```

    Windows:

    ```bash
    >> .\.speech_corpora_env\Scripts\activate
    ```

    if using conda;

    ```bash
    >> conda activate speech_corpora
    ```

2) Install the requirements:

    ```bash
    >> pip3 install -r requirements.txt
    ```

3) Fire up jupyter notebooks and open the Formants_Analysis.ipynb notebook

    ```bash
    >> jupyter notebook
    ```

4) Run the notebook.
