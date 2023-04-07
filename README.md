# Wrangling and Visualizing Musical Data
## Description
Apply data-wrangling and visualization tools from the tidyverse to musical data. Find the most common chords and chord progressions in a sample of pop/rock music from the 1950s-1990s, and compare the styles of different artists. This project uses a parsed and cleaned version of the [McGill Billboard Dataset](https://ddmal.music.mcgill.ca/research/The_McGill_Billboard_Project_(Chord_Analysis_Dataset)/), version 2.0 (CC0 license).
## Usage
Clone this repository and open the Jupyter notebook file (`*.ipynb`) in a Jupyter environment with R kernel support. Make sure to install the required packages such as `tidyverse`. You can do this by running the following commands in a code cell within the notebook:
``` r
install.packages("tidyverse")
```
Once the packages are installed, run the code cells in the notebook to generate the plots and analyses.

If you don't have a Jupyter environment set up, you can install Jupyter Notebook and the R kernel using the following steps:

1. Install Jupyter Notebook by following the instructions on the [official Jupyter website](https://jupyter.org/install).

2. Install the R kernel for Jupyter Notebook by running the following commands in your R console:
``` r 
install.packages("IRkernel")
IRkernel::installspec()
```
After completing the installation, launch Jupyter Notebook, navigate to the folder containing the notebook file, and open it to begin running the analysis.