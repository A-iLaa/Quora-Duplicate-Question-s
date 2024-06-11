# Quora Duplicate Questions

## Introduction
Welcome to the Quora Duplicate Questions repository! This project aims to identify duplicate questions on Quora using various natural language processing techniques. By leveraging machine learning and feature engineering, we can determine if two questions are similar or not.

## Features
The dataset has undergone initial cleaning and TF-IDF encoding. Additionally, several features have been extracted from the data set, including:
- Length of questions
- Number of words
- Total number of unique words from the two questions
- Number of common words
- Word share (ratio of common words to total number of words)
- Token features:
  - CWC_min: Ratio of number of common words to the minimum of the lengths of the questions
  - CWC_max: Ratio of number of common words to the maximum of the lengths of the questions
  - CSC_min: Number of common stop words divided by the minimum number of stop words in the two questions
  - CSC_max: Number of common stop words divided by the maximum number of stop words in the two questions
  - CTC_min: Number of common tokens divided by the minimum number of tokens in the two questions
  - CTC_max: Number of common tokens divided by the maximum number of tokens in the two questions
- Last_word_eq: Checks whether the last words of the questions are equal or not
- First_word_eq: Checks whether the first words of the questions are equal or not
- Length features:
  - Difference in lengths of the questions
  - Mean of lengths of the questions
  - Ratio of the longest common substring to the minimum of the lengths of the questions plus one
- Fuzzy features: Utilizes fuzzy string matching techniques (refer to [this link](https://chairnerd.seatgeek.com/fuzzywuzzy-fuzzy-string-matching-in-python/) for more information)

## Usage
To use this project, follow these steps:
1. Clone the repository: `git clone https://github.com/A-iLaa/Quora-Duplicate-Questions.git`
2. Install the necessary dependencies: `pip install -r requirements.txt`
3. Run the main script: `python main.py`
4. Provide your own dataset or use the default dataset provided in the repository.
5. Observe the results and analyze the duplicate question pairs identified.

## Contributing
Contributions to this project are welcome! If you would like to contribute, please follow these guidelines:
- Fork the repository and create a new branch.
- Make your changes and test them thoroughly.
- Submit a pull request describing your changes and their purpose.

## License
This project is licensed under the [MIT License](LICENSE).

## Acknowledgments
- The Quora Duplicate Questions dataset: https://www.kaggle.com/c/quora-question-pairs
- FuzzyWuzzy library for fuzzy string matching

## Contact
For any questions or inquiries, please contact p.p.akhila1999@gmail.com
