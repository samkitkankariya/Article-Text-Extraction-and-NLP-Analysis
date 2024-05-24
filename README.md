# Comprehensive NLP Analysis of Web Articles

## Project Description
This project involves extracting article text from URLs provided in an input Excel file, performing Natural Language Processing (NLP) analysis, and computing various textual metrics. The project uses Python libraries such as BeautifulSoup for web scraping and NLTK for text analysis. The output is saved in a structured format as specified in an output Excel file.

## Table of Contents
- [Objective](#objective)
- [Data Extraction](#data-extraction)
- [Data Analysis](#data-analysis)
- [Installation](#installation)
- [Usage](#usage)
- [Output Metrics Explained](#output-metrics-explained)
- [Files](#files)
- [Technical Skills Demonstrated](#technical-skills-demonstrated)
- [Contributing](#contributing)
- [License](#license)

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
### Step 1: Data Extraction & Data Analysis
Run the Colab Notebook  to extract article texts from the URLs provided in `Input.xlsx` and  perform text analysis and compute the required metrics:

### Step 2: Review Output
The results will be saved in `Output Data Structure Self.xlsx`.

## Output Metrics Explained
- **POSITIVE SCORE**: The count of positive words in the article based on a predefined list of positive words.
- **NEGATIVE SCORE**: The count of negative words in the article based on a predefined list of negative words.
- **POLARITY SCORE**: The ratio of the difference between positive and negative scores to the sum of positive and negative scores, indicating the overall sentiment of the text.
- **SUBJECTIVITY SCORE**: The ratio of the sum of positive and negative scores to the total number of words, indicating the degree of subjectivity in the text.
- **AVG SENTENCE LENGTH**: The average number of words per sentence in the article.
- **PERCENTAGE OF COMPLEX WORDS**: The proportion of complex words (words with more than two syllables) to the total number of words.
- **FOG INDEX**: A readability metric calculated using the formula: 0.4 * (average sentence length + percentage of complex words).
- **AVG NUMBER OF WORDS PER SENTENCE**: Another measure of average sentence length in the article.
- **COMPLEX WORD COUNT**: The total number of complex words in the article.
- **WORD COUNT**: The total number of words in the article.
- **SYLLABLE PER WORD**: The average number of syllables per word in the article.
- **PERSONAL PRONOUNS**: The count of personal pronouns (e.g., I, we, my, ours, us) in the article.
- **AVG WORD LENGTH**: The average length of words in the article.

## Files
- **Input.xlsx**: Input file containing URLs.
- **Output Data Structure.xlsx**: Template for the output data structure.
- **article_text_extraction.ipynb**: Jupyter Notebook for extracting articles from the URLs.
- **text_analysis.ipynb**: Jupyter Notebook for performing text analysis.
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
