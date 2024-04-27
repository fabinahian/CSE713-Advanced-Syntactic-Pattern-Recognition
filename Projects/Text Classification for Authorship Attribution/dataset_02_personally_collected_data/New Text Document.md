# Text Classification for Author Attribution

This repository hosts the data and code for the "Text Classification for Author Attribution" project. Our aim is to develop a machine learning model capable of attributing texts to their respective authors based on textual content. The data consists of texts from Project Gutenberg, manually processed to enhance usability for this project.

## Data Source

The data for this project has been sourced from [Project Gutenberg](https://www.gutenberg.org/), which provides free access to a large collection of literary works in the public domain. We specifically downloaded the "Plain Text UTF-8" format of each book.

## Data Selection

We selected three books from each of ten different authors, aiming for a diverse representation of genres and writing styles. The selected works and their corresponding authors are:

- **James Joyce**
  - *A Portrait of the Artist as a Young Man*
  - *Dubliners*
  - *Ulysses*
- **Mark Twain**
  - *Adventures of Huckleberry Finn*
  - *The Adventures of Tom Sawyer (Parts 1-8)*
  - *The Tragedy of Pudd'nhead Wilson*
- **William Shakespeare**
  - *All's Well That Ends Well*
  - *Macbeth*
  - *The Merry Wives of Windsor*
- **Oscar Wilde**
  - *An Ideal Husband*
  - *The Importance of Being Earnest: A Trivial Comedy for Serious People*
  - *The Picture of Dorian Gray*
- **Jane Austen**
  - *Emma*
  - *Pride and Prejudice*
  - *Sense and Sensibility*
- **Charles Dickens**
  - *Great Expectations*
  - *Oliver Twist*
  - *Sketches of Young Couples*
- **Joseph Conrad**
  - *Heart of Darkness*
  - *Lord Jim*
  - *The Rover*
- **George Eliot**
  - *Middlemarch*
  - *Silas Marner*
  - *The Mill on the Floss*
- **Virginia Woolf**
  - *Mrs Dalloway*
  - *Night and Day*
  - *The Voyage Out*
- **F. Scott Fitzgerald**
  - *The Beautiful and Damned*
  - *The Great Gatsby*
  - *This Side of Paradise*

## Data Preprocessing

The preprocessing involved manually opening each text file to remove non-essential content such as headers, footers, and any text not authored by the book's author. This step was critical in ensuring the text data mainly contains the author's original words, although it does not guarantee absolute cleanliness. The goal was to minimize noise and non-authorial text that could affect the accuracy of author attribution.

## File Naming Convention

Each book's text was saved in a .txt file named according to the format:
```
authorfirstname_authorlastname-booknamefirstword_booknamesecondword.txt
```
This naming convention aids in quick identification of files without dealing with spaces or ambiguous titles.

## Project Structure

- `/data`: This folder contains the cleaned text files.
- `README.md`: Provides an overview and detailed description of the data.