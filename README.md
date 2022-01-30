# Data-Science-Final-Project

My research question: Is it possible to predict the amount of actions per seconds of a CPU by its parameters?


In the research we will try to predict:

the exact amount of actions per seconds with Linear regression

whether a random CPU can pass a low threshold of that amount of actions per second parameter, with Logistic regression


Crawling on wikipedia: I used a built-in function from the Pandas Python library, which detects all of the tables in a webpage and save it into a list of DataFrames.

Merging the dataframes: 
Every wikipedia webpage crawl returns a list of all of the tables found in that page.
so we get list of tables lists!

Duplicates: We expect for duplicates as we might crawl the same CPU model twice, because there are some pages that covers the same CPU models.



We started with 500K, and we finished with around 60K.


Outliars: The outliars found are shown in graphs in the EDA section.
Because there are a lot of important information of records that filled with missing value defaults, I decided to keep those values, and locate them in the graphs, in order to improve the Models.


ML: My first model is a Linear regression model, which predicts the exact amount of actions per seconds of a CPU, based on its own parameters.

Sometimes Software engineerings are interested in a minimum value of actions per second, and not the exact number.
So the second model is a Logistic regression one, which predicts whether a CPU can reach and pass a minimum low threshold of actions per seconds.
