# INFR11182-2019
This is the repository for the Second (graded) Assignment for IAML 2019.

**N.B.: This is the Level 11 version of the course: if you are an undergraduate student, then you should go to the Level 10 version, [here](https://github.com/michael-camilleri/INFR10069-2019).**

## Repository Contents

 * `conda.req`: This is the list of packages you need to complete the assignment
 * `style.tex`: This is the style file for the Assignment Template. **DO NOT MODIFY** this file in any way.
 * `Assignment_2.tex`: This is the template you should modify to writeup your assignment.
 * `Instructions.pdf`: This is the pdf with the question-sheet for the Assignment.
 * `Data`: This is a directory (folder) which contains all the data you need to complete the assignment.

## Setting up your environment

These instructions are a summary of the more detailed [Readme](https://github.com/amosstorkey/iaml-labs) in the Lab Setup. Note that for this assignment, you should use the **provided** requirements file in **this** repository and not the one in the lab repository.

#### (a) Install Conda
If you do not have conda, install it: otherwise skip this step:

 1. Download Conda from `https://docs.conda.io/en/latest/miniconda.html`
 2. Install: ```bash Miniconda3-latest-Linux-x86_64.sh```

#### (b) Create a NEW environment
**N.B. You must do this step! you cannot use the same environment as for the Labs!**

 1. Create Environment: ```conda create --name iamlassignment2 python=3.6```
 2. Activate environment: ```source activate iamlassignment2```
 3. Install the required libraries: ```conda install --file conda.req```

#### (c) Install the mpctools library

We have provided this set of tools to aid in the coding up of the solutions. Make sure you have the above environment active

 1. Download or clone the repository from `https://github.com/michael-camilleri/mpctools`: e.g. ```git clone https://github.com/michael-camilleri/mpctools.git```
 2. From within the downloaded directory execute:
    ```
    python setup.py sdist --format=tar
    pip install dist/mpctools-0.3.10.tar --user
    ```