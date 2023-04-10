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
## Contents
1. **Introduction:** This section covers the process of loading the McGill Billboard chord dataset and the required packages (dplyr, readr, and ggplot2). It demonstrates how to read in 'datasets/bb_chords.csv' using read_csv and assign it to bb, and displays the first rows of bb.

2. **The most common chords:** In this section, we find the most common chords in the McGill Billboard Dataset by counting the occurrences of each raw chord type in the dataset and sorting them in descending order. The top 20 most common chords are displayed.

3. **Visualizing the most common chords:** This section shows how to create a flipped bar plot of the top 20 chords, displaying the percentage of occurrences for each chord type.

4. **Chord "bigrams":** This part explains how to create a count of chord bigrams by adding new columns to bb and counting the occurrences of each bigram type. The top 20 most common chord bigrams are displayed.

5. **Visualizing the most common chord progressions:** This section demonstrates how to create a flipped bar plot for the 20 most common chord bigrams by modifying the code from Step 3 and adjusting the plot labels.

6. **Finding the most common artists:** In this section, we find the 30 artists with the most songs in the McGill Billboard Dataset by isolating the artist and title columns, removing duplicates, and counting the number of songs per artist.

7. **Tagging the corpus:** This part details how to add a new column 'instrument' to bb, including "piano" or "guitar" for piano- and guitar-driven songs, and displays the new data frame 'bb_tagged'.

8. **Comparing chords in piano-driven and guitar-driven songs:** This section explains how to create a faceted plot comparing the frequency of the most common chords in songs by piano- and guitar-driven artists.

9. **Comparing chord bigrams in piano-driven and guitar-driven songs:** In this section, we create a faceted plot comparing the frequency of the most common chord bigrams in songs by piano- and guitar-driven artists by modifying the code from Task 4 and Task 8.

10. **Conclusion:** This final section focuses on determining the validity of the hypothesis that guitar-driven and piano-driven songs have different chord tendencies and whether further data analysis is needed to draw a conclusion.