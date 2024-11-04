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


 | URL_ID | URL                                                                 | POSITIVE SCORE | NEGATIVE SCORE | POLARITY SCORE | SUBJECTIVITY SCORE | AVG SENTENCE LENGTH | COMPLEX WORD COUNT | PERCENTAGE OF COMPLEX WORDS | FOG INDEX | AVG NUMBER OF WORDS PER SENTENCE | COMPLEX WORD COUNT | WORD COUNT | SYLLABLE PER WORD | PERSONAL PRONOUNS | AVG WORD LENGTH   
 |
|--------|---------------------------------------------------------------------|----------------|----------------|-----------------|--------------------|----------------------|--------------------|------------------------------|-----------|---------------------------------|--------------------|------------|------------------|-------------------|-----------------|
| 0      | https://insights.blackcoffer.com/ml-and-ai-bas...                  | 34.0           | 8.0            | 0.619048        | 0.078212          | 40.294118           | 249               | 36.350365                     | 30.657793 | 40.294118                      | 249               | 451        | 1569             | 1                 | 6.093431       |
| 1      | https://insights.blackcoffer.com/streamlined-i...                  | 1.0            | 0.0            | 0.999999        | 0.043478          | 20.000000           | 5                 | 25.000000                     | 18.000000 | 20.000000                      | 5                 | 16         | 41               | 0                 | 5.900000       |
| 2      | https://insights.blackcoffer.com/efficient-dat...                  | 1.0            | 0.0            | 0.999999        | 0.055556          | 19.000000           | 4                 | 21.052632                     | 16.021053 | 19.000000                      | 4                 | 13         | 35               | 0                 | 5.105263       |
| 3      | https://insights.blackcoffer.com/effective-man...                  | 1.0            | 0.0            | 0.999999        | 0.045455          | 21.000000           | 5                 | 23.809524                     | 17.923810 | 21.000000                      | 5                 | 15         | 38               | 0                 | 5.333333       |
| 4      | https://insights.blackcoffer.com/streamlined-t...                  | 1.0            | 0.0            | 0.999999        | 0.043478          | 20.000000           | 6                 | 30.000000                     | 20.000000 | 20.000000                      | 6                 | 16         | 42               | 0                 | 6.050000       |

Then finally I saved the data in a csv file.

