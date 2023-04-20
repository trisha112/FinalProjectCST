# Bias in Headlines About Women
Group: CST

Team Members: Trisha Agrawal, Surya Brunton, Claudia Pascual, Islam Dafaalla 
## Disclaimer: The [headlines.csv file](https://www.kaggle.com/datasets/thedevastator/women-in-headlines-bias?select=headlines.csv) (99 MB) was too large to upload in the archive folder. The other files used are included in the archive folder above. 

# Link to dataset: https://www.kaggle.com/datasets/thedevastator/women-in-headlines-bias
# Link to presentation: https://docs.google.com/presentation/d/1EzwyXSvR4GYqZhzN7EtAlNp57MjtEDvoiB0QrVytSP8/edit?usp=sharing
# Info: 
We chose this data set because we want to analyze the words that are used in articles about women in different countries. The predictor we build could be in the format of giving the algorithm the word and the year from a headline and having the algorithm guess which country the headline was most likely to come from. 

# Hypothesis:
There is a difference in the levels of bias observed in headlines about women amongst the four countries in the dataset and over the 12 years in the dataset. 

# Data Cleaning Process:
Data cleaning consisted of removing unnecessary columns or rows based on values.

# Algorithms Used:
- Naive Bayes' Algorithm
- Decision Tree
- Logistic Regression
- Random Forest Classifier
- KNN

# Description:
For our project we have decided to use the dataset ‘Women in Headlines: Bias’. This dataset contains headlines published between 2010 and 2020 in four countries, the US, the UK, India and South Africa. Two dictionaries were created using these headlines: gendered words about women and cultural stereotypes about women. 

We want to use this dataset to investigate the correlation between the gendered words about women and cultural stereotypes about women and identify any biases that may exist, specifically the differences between the four countries in different years. 

We could use the file headlines_reduced_temporal.csv which contains the columns:
Headline_no_site - the headline of the article 
Time - The time the article was published
Country - The country the article was published in
Bias - The bias score of the article. The bias score was calculated using the Gender Bias Taxonomy V1.0. Bias is represented as a float on a scale from 0 to 1, with 1 as least biased and 1 as most biased. 
Year - The year the article was published
This file has 1879 entries. 

We could also use the file country_time_freqrank.csv which contains frequency of words in published headlines grouped by country and year. The file contains many columns, most useful: year, country, word and frequency (of word in published headlines). This file has 7619 entries and 127 unique words. 
We can use the bias, headline and word information to create a predictive algorithm that would predict the country and the year the headline was published. 

As extra ideas: 
We could also use the word_dictionary used for identifying biases and use it to create our own bias calculation (by including other bias words)  and compare it to the bias generated by the author.
We could also use the word_themes.csv file where a predictive algorithm can classify a word to be of a specific theme based on a word that is given to the algorithm. This could suggest whether or not specific themes are more common in specific countries or years. An example could be when words in the “empowerment” theme were more commonly used in headlines during election years or other important political events.
Generate a neutral headline for articles. 
Add a neutral category in the word dictionary

# Running it:
1. Download archieve and insert into google drive under My drive path.
2. When runinng it make sure to allow acess to the folder.
3. It might take a long time (1hr), so to skip the tree uncomment ln:23 to shorten the randometree data inputs.
(Note the file uploaded has ran through everything)
