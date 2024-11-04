# Random-kaggle-project

This is an assignment project I did for a company called Blackcoffer. 

Company link: https://blackcoffer.com/

It includes:

Created a web scraper that extracts text from articles on a website and saves them to individual text files.
Then I took a list of URLs from an Excel file, extracted article content from those URLs, and saved the extracted data into a new CSV file. I obtained URL_ID,	Title, Article_text as the features of the csv file.
Then I performed sentiment analysis on the dataset of text articles. It reads the text data, preprocesses it by removing stop words, and calculates sentiment scores based on the presence of positive and negative words. 
A file containing stop words and a file containing negative and positive words was already provided.
Then based on different criterias and definitions new numerical features were created.
Then finally I removed the textual features that is Title and Article_text from the dataframe.

My new dataset looks something like this:


|    | Column                           | Non-Null Count | Dtype    |
|---:|:---------------------------------|---------------:|:---------|
|  0 | URL_ID                          |           147 | object   |
|  1 | URL                             |           147 | object   |
|  2 | POSITIVE SCORE                  |           147 | float64  |
|  3 | NEGATIVE SCORE                  |           147 | float64  |
|  4 | POLARITY SCORE                  |           147 | float64  |
|  5 | SUBJECTIVITY SCORE              |           147 | float64  |
|  6 | AVG SENTENCE LENGTH             |           147 | float64  |
|  7 | COMPLEX WORD COUNT              |           147 | int64    |
|  8 | PERCENTAGE OF COMPLEX WORDS     |           147 | float64  |
|  9 | FOG INDEX                       |           147 | float64  |
| 10 | AVG NUMBER OF WORDS PER SENTENCE |           147 | float64  |
| 11 | COMPLEX WORD COUNT              |           147 | int64    |
| 12 | WORD COUNT                      |           147 | int64    |
| 13 | SYLLABLE PER WORD               |           147 | int64    |
| 14 | PERSONAL PRONOUNS               |           147 | int64    |
| 15 | AVG WORD LENGTH                 |           147 | float64  |

Then finally I saved the data in a csv file.

