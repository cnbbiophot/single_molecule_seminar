# Single-Molecule Tracking Analysis. Telling molecular diffusional regimes apart.

This exercise is part of the *Técnicas Experimentales Avanzadas en Nanofísica y Biofísica* course of the *Máster Universitario en Física de la Materia Condensada y de los Sistemas Biológicos*.

The point of this exercise is to explore how different physical mechanisms can give the same $(D, \alpha)$. In doing so, you will learn about additional observables that can help you tell the different diffusional regimes apart.

We will use the models provided by the [2nd AnDi Challenge](https://github.com/AnDiChallenge) to simulate different diffusing scenarios.  

This practical was prepared by Jose Requejo Isidro.  
Centro Nacional de Biotecnología (CNB, CSIC). Madrid

## Set up
You can either run locally on your laptop using VSCode (or your preferred IDE) on a Conda environment, or use a Kaggle account and run the notebook online. Please choose one of the options and follow the instructions before the seminar:

**Option 1: Run on Kaggle (online):**  
Go to: https://www.kaggle.com/ 

1.    Create an account.
2.    Required: To gain access to the Internet and GPU resources, verify your phone number:
3.    Your Work (Left menu, at the bottom) → Settings → Phone Verification
4.    Create a new notebook by clicking "+ Create" on the top-left corner. In the notebook settings (right menu, bottom), configure:
5.    Session Options → Internet: On

**Option 2: Local Installation with Conda and VSCode:**  
Create an environment using the following sequence of commands from the terminal (Linux) or Anaconda prompt (Windows). Do not despair, solving dependencies may take a while (sometimes more than 5 min) (note: SMS stands for *Single-Molecule Spectroscopy).

`conda create -n SMS -c conda-forge python=3.11 matplotlib numpy "ipykernel<7" -y`  
`conda activate SMS`  
`python -m pip install "andi-datasets>=2.1"`

Note: Always install packages through Conda before using `pip`. If you need to install additional Conda packages after using `pip`, it is generally best to delete the environment and start from scratch to avoid dependency conflicts.

To remove the environment just type: `conda remove -n SMS –all`

