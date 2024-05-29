## Text Analysis Project

This personal project was created to explore and learn about text analysis techniques using Python. It focuses on analyzing textual content from Blackcoffer Insights articles, extracting various linguistic features, and calculating readability scores to assess the complexity and sentiment of the text.

### Dependencies

* bs4
* requests
* pandas
* nltk
* string
* os
* pathlib

### Files

* **BlackCoffer.py:** Contains the Python code for web scraping, text cleaning, feature extraction, and score calculation.
* **Input.xlsx:** An Excel file containing the URLs of Blackcoffer Insights articles.
* **MasterDictionary:** A folder containing positive-words.txt and negative-words.txt for sentiment analysis.
* **StopWords:** A folder containing text files with lists of stop words in various languages.

### Functionality

1. **Web Scraping:** The script fetches articles from the provided URLs and extracts the title and main content.
2. **Text Cleaning:** It removes stop words, punctuation, and performs other cleaning operations to prepare the text for analysis.
3. **Feature Extraction:** The script calculates the following features for each article:
    * Positive Score: Number of positive words present.
    * Negative Score: Number of negative words present.
    * Polarity Score: The overall sentiment of the text, ranging from -1 (negative) to +1 (positive).
    * Subjectivity Score: The degree to which the text expresses personal opinions or beliefs, ranging from 0 (objective) to 1 (subjective).
    * Average Sentence Length: The average number of words per sentence.
    * Percentage of Complex Words: The percentage of words with more than two syllables.
    * Fog Index: A readability score indicating the number of years of formal education needed to understand the text.
    * Average Number of Words Per Sentence:  Same as Average Sentence Length.
    * Complex Word Count:  Same as the number of complex words.
    * Word Count: Total number of words in the text.
    * Syllable Per Word: Average number of syllables per word. 
    * Personal Pronouns: Number of personal pronouns (I, we, my, ours, us) present. 
    * Average Word Length:  Average number of characters per word.

4. **Output:** The extracted features and scores are saved to an Output.csv file.

### How to Run

1. **Set up the required dependencies.**
2. **Place the Input.xlsx file, MasterDictionary folder, and StopWords folder in the same directory as the script.**
3. **Run the script:** `python BlackCoffer.py`
4. **The Output.csv file will be generated containing the analysis results.**

