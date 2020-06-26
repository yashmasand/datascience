Data Analysis on Renting Options in Sydney: Airbnb
===

Created by: **Yash Masand**


We obtained our dataset from [Airbnb Data](http://insideairbnb.com/get-the-data.html) for Sydney. The csv file that we have used is named as ![#c5f015](https://placehold.it/15/c5f015/000000?text=+) `listings` and it contains _38080 rows and 106 columns_. 
This data is quite untidy and there are a number of columns which are not required as part of our analysis, so we have dropped those columns and are only working on 50 columns. 
## Data Cleaning ## 
As part of our data cleaning activity, We have updated various variable types and have handled boolean type values for some columns. Mapping of string to numerical categorical values have been addressed. The column __`amenities`__  was a list displaying the number of amenities provided in each listing .We have splitted that list and printed out the total number of amenities for each listing as a numerical value. After splitting we have created a new column called __`amenities_count`__ that holds numerical values of data so that it's easier to plot them later on. For further detailed analysis about Data Cleaning, please refer to `project.ipynb` file.

## Data Analysis ##
_`WordCloud implementation`_ on the column `house_rules`

__Brief about Wordcloud__ - It is a data visualization technique that is used for representing text data in which the size of each word indicates its frequency or importance.

__`Project Implementation`__ - We worked on the column `house_rules` that has holds comments from the hosts regarding house rules for any particular listing. The necessary libraries imported were:

`from matplotlib import rcParams`<br>
`from wordcloud import WordCloud, STOPWORDS`<br>
`from nltk.corpus import stopwords`<br>
`import collections`<br>

__`Conclusion on WordCloud`__ - After performing this analysis, we derived the conclusion that in most of the listings there was a very frequent word `smoking` from which we concluded that majority of the listings don't allow smoking.



