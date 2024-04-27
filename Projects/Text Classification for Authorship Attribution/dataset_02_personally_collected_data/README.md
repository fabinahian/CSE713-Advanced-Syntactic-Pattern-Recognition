# Text Classification for Author Attribution Data Repository

## Introduction

This repository houses the text data for a project on text classification aimed at authorship attribution. The dataset comprises a selection of literary works manually downloaded and preprocessed from Project Gutenberg. These works have been chosen from a variety of authors to train machine learning models that can predict the author of a given text snippet.

## Data Acquisition

The text data was sourced from [Project Gutenberg](https://www.gutenberg.org/), which provides free eBooks of literary works that are no longer under U.S. copyright protection. We selected a minimum of three books per author for a set of 10 authors, totaling 39 texts.

## Preprocessing

The following preprocessing steps were carried out to ensure the data is more conducive for our analysis:

1. **Manual Download**: Each book was downloaded in the "Plain Text UTF-8" format.
2. **Header and Footer Removal**: Manual inspection and removal of Gutenberg's headers and footers, along with any content not directly part of the original book or authored by the respective author, was conducted. This step is crucial to reduce the noise in the data that could potentially affect our analysis and modeling.
3. **File Naming**: The cleaned text files were saved following a consistent naming convention to facilitate easy reference and organization:
   - Format: `authorfirstname_authorlastname-booknamefirstword_booknamesecondword.txt`
   - Example: `jane_austen-pride_and_prejudice.txt`
   - Note: Spaces and apostrophes have been removed from names and titles.

## Dataset Structure

The dataset, post-cleaning, consists of 39 `.txt` files, each corresponding to a different literary work. These files are prepared with the intention of creating a structured `.csv` file for further data processing and analysis in a Jupyter notebook.

## Project Outline

- `/data`: Contains the preprocessed `.txt` files of the literary works.
- `README.md`: Describes the dataset.

## Future Work

The next phase will involve extensive data analysis in Jupyter notebooks, where we will:
- Convert the `.txt` files into a structured `.csv` format.
- Perform exploratory data analysis to understand the characteristics of each author's writing style.
- Develop and train machine learning models for authorship attribution.
- Validate and test the models to ensure robustness and accuracy.

## Citation and Acknowledgments

This project utilizes data obtained from Project Gutenberg. We express our gratitude to the contributors and maintainers of Project Gutenberg for providing open access to these literary works.

When referencing the data used in this project, please cite:
```
Project Gutenberg. (n.d.). Retrieved from https://www.gutenberg.org/
```
