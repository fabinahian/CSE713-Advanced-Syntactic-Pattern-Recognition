# Gutenberg Dataset Analysis

This repository is dedicated to developing a machine learning project focused on text analysis for authorship attribution. It utilizes the Gutenberg Dataset, which contains phrases from famous literary works made available by Project Gutenberg. The dataset's structure and processing details are attributed to its original creators.

## Dataset Description

The Gutenberg Dataset involves phrases extracted from texts by six distinguished authors, representing a wide range of cultures and historical periods. The original dataset creators have provided the following processing steps:

### Text Processing
- Punctuation was removed.
- Letters with diacritics were converted to their base letters.
- "Structure" words like 'Chapter', 'Scene', 'Prologue' were removed.

### Sequence Creation
- Sequences consisting of three consecutive words, each ranging from 3 to 6 letters, were extracted.
- Words were padded to 6 characters and concatenated to form an 18-character string.

### Image Encoding
- Images represent these strings with the x-axis indicating each character's index and the y-axis showing the corresponding letter (A-Z, with space represented below 'Z').

### Data Format and Distribution
- Data is in a channels-first format: (n, 1, 27, 18)
- Training set: 45,000 samples
- Validation set: 15,000 samples
- Testing set: 6,000 samples

### Classes and Labels
The dataset includes six classes, each associated with an author:
- **0**: Aquinas
- **1**: Confucius
- **2**: Hawthorne
- **3**: Plato
- **4**: Shakespeare
- **5**: Tolstoy

Each class contains 11,000 examples evenly distributed across the subsets.

## Data Files

The dataset is stored in NumPy (.npy) format and can be accessed using the Python NumPy library. The metadata file provides additional information and is accessible with standard text editors.

## Citing the Dataset

When using this dataset in your research or applications, please cite it as follows:

> Towers, David; Geada, Rob; Atapour-Abarghouei, Amir; McGough, Andrew Stephen (2023). Gutenberg Dataset. Newcastle University. Dataset. https://doi.org/10.25405/data.ncl.24574753.v1

## Usage Example

```python
import numpy as np

# Load the dataset
data = np.load('path_to_your_dataset_file.npy')

# Example of accessing data
sample = data[0]  # Access the first sample from the dataset
print(sample)
```

## Contributions

We welcome contributions. Please ensure any enhancements or modifications adhere to the original dataset's terms of use and copyright guidelines.
