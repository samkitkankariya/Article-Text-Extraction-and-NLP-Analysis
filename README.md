# Article-Text-Extraction-and-NLP-Analysis
This project involves extracting article text from URLs provided in an input Excel file, performing Natural Language Processing (NLP) analysis, and computing various textual metrics.

### Project Description
This project involves extracting article text from URLs provided in an input Excel file, performing Natural Language Processing (NLP) analysis, and computing various textual metrics. The project uses Python libraries such as BeautifulSoup for web scraping and NLTK for text analysis. The output is saved in a structured format as specified in an output Excel file.

### README File

# Article Text Extraction and NLP Analysis

## Project Overview
This project aims to extract textual data from a list of URLs provided in an input Excel file and perform comprehensive text analysis to compute various linguistic and readability metrics. The project leverages Python programming with libraries such as BeautifulSoup for web scraping and NLTK for text processing and analysis. The results are saved in an output Excel file in a specified structure.

## Table of Contents
- [Objective](#objective)
- [Data Extraction](#data-extraction)
- [Data Analysis](#data-analysis)
- [Installation](#installation)
- [Usage](#usage)
- [Output Variables](#output-variables)
- [Files](#files)
- [Technical Skills Demonstrated](#technical-skills-demonstrated)
- [Contributing](#contributing)

## Objective
The primary objective is to extract article texts from the given URLs, save the extracted articles in text files, and perform text analysis to compute several linguistic and readability metrics as outlined in the "Text Analysis.docx" document. The results are then saved in the specified format in the output Excel file.

## Data Extraction
### Input
- **Input.xlsx**: An Excel file containing the URLs of the articles to be scraped.
### Process
- For each URL in the input file, extract the article title and text, excluding website headers, footers, and other extraneous content.
- Save the extracted text in a text file named after the URL_ID.

## Data Analysis
### Process
- Perform textual analysis on each extracted article.
- Compute the following metrics:
  - POSITIVE SCORE
  - NEGATIVE SCORE
  - POLARITY SCORE
  - SUBJECTIVITY SCORE
  - AVG SENTENCE LENGTH
  - PERCENTAGE OF COMPLEX WORDS
  - FOG INDEX
  - AVG NUMBER OF WORDS PER SENTENCE
  - COMPLEX WORD COUNT
  - WORD COUNT
  - SYLLABLE PER WORD
  - PERSONAL PRONOUNS
  - AVG WORD LENGTH
- Save the computed metrics in the output Excel file.

## Installation
To set up the project environment, follow these steps:

1. **Clone the repository:**
    ```sh
    git clone <repository_url>
    cd <repository_directory>
    ```

2. **Install the required packages:**
    ```sh
    pip install -r requirements.txt
    ```

3. **Download NLTK data:**
    ```sh
    python -m nltk.downloader punkt
    ```

## Usage
### Step 1: Data Extraction
Run the script to extract article texts from the URLs provided in `Input.xlsx`:

```sh
python extract_articles.py
```

### Step 2: Data Analysis
Run the script to perform text analysis and compute the required metrics:

```sh
python analyze_texts.py
```

### Step 3: Review Output
The results will be saved in `Output Data Structure Self.xlsx`.

## Output Variables
- **URL_ID**
- **URL**
- **POSITIVE SCORE**
- **NEGATIVE SCORE**
- **POLARITY SCORE**
- **SUBJECTIVITY SCORE**
- **AVG SENTENCE LENGTH**
- **PERCENTAGE OF COMPLEX WORDS**
- **FOG INDEX**
- **AVG NUMBER OF WORDS PER SENTENCE**
- **COMPLEX WORD COUNT**
- **WORD COUNT**
- **SYLLABLE PER WORD**
- **PERSONAL PRONOUNS**
- **AVG WORD LENGTH**

## Files
- **Input.xlsx**: Input file containing URLs.
- **Output Data Structure.xlsx**: Template for the output data structure.
- **extract_articles.py**: Script for extracting articles from the URLs.
- **analyze_texts.py**: Script for performing text analysis.
- **StopWords**: Directory containing stop words files.
- **MasterDictionary**: Directory containing positive and negative word lists.

## Technical Skills Demonstrated
1. **Data Extraction**: Using BeautifulSoup for web scraping to extract article text.
2. **Data Preprocessing**: Cleaning and preparing text data for analysis.
3. **NLP Analysis**: Using NLTK for tokenization, sentiment analysis, and readability metrics.
4. **Data Management**: Handling input and output files, saving results to Excel.
5. **Python Programming**: Writing robust and efficient Python code for data extraction and analysis.

## Contributing
Contributions are welcome! Please follow these steps:
1. Fork the repository.
2. Create a new branch.
3. Make your changes.
4. Submit a pull request.
