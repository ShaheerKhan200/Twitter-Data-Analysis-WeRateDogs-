# Twitter-Data-Analysis-WeRateDogs- Data Wrangling Project

## Following files are included in this repository:

### Files given/used:
* twitter_archive_enhanced.csv: file as given. This can be found [here](https://github.com/ShaheerKhan200/Twitter-Data-Analysis-WeRateDogs--Data-Wrangling-Project/blob/main/twitter-archive-enhanced.csv).
* image_predictions.tsv: file downloaded programmatically. This can be found [here](https://github.com/ShaheerKhan200/Twitter-Data-Analysis-WeRateDogs--Data-Wrangling-Project/blob/main/image-predictions.tsv).
* tweet_json.txt and tweet_json.json: file constructed via twitter API can be found [here](https://github.com/ShaheerKhan200/Twitter-Data-Analysis-WeRateDogs--Data-Wrangling-Project/blob/main/tweet_json.txt) and [here](https://github.com/ShaheerKhan200/Twitter-Data-Analysis-WeRateDogs--Data-Wrangling-Project/blob/main/tweet_json.json) respectively.

### Code
* wrangle_act.ipynb: code for gathering, assessing, cleaning, analyzing, and visualizing data, this file can be found [here](https://github.com/ShaheerKhan200/Twitter-Data-Analysis-WeRateDogs--Data-Wrangling-Project/blob/main/wrangle_act.ipynb).

### Result:
* twitter_archive_master.csv: This is the combined and cleaned data. This can be found [here](https://github.com/ShaheerKhan200/Twitter-Data-Analysis-WeRateDogs--Data-Wrangling-Project/blob/main/twitter_archive_master.csv).
* wrangle_report.pdf: documentation for data wrangling steps: gather, assess, and clean. This can be found [here](https://github.com/ShaheerKhan200/Twitter-Data-Analysis-WeRateDogs--Data-Wrangling-Project/blob/main/wrangle_report.pdf).
* act_report.pdf: documentation of analysis and insights into final data. This can be found [here](https://github.com/ShaheerKhan200/Twitter-Data-Analysis-WeRateDogs--Data-Wrangling-Project/blob/main/act_report.pdf).


## Dataset

> The dataset that I have wrangled, analyzed and visualized is the tweet archive of Twitter user [@dog_rates](https://twitter.com/dog_rates), also known as WeRateDogs. [WeRateDogs](https://en.wikipedia.org/wiki/WeRateDogs) is a Twitter account that rates people's dogs with a humorous comment about the dog. These ratings almost always have a denominator of 10. The numerators, almost always greater than 10. For example, 11/10, 12/10, 13/10, etc. WeRateDogs has over 8 million followers and has received international media coverage.

Feature Engineering was done to produce:
> * Rating Classification - rating_numerator_new less than and equals to 10 or more than 10 was categorized into 'Low Rating' or 'High Rating' (Categorical)
> * Retweet Count Classification - retweet counts was categorized into the following categories based on retweet count: 'Low Retweet Count', 'Moderate Retweet Count', 'High Retweet Count', 'Very High Retweet Count' (Categorical)
> * Favorite Count Classification - favorite counts was categorized into the following categories based on favorite count: 'Low Favorite Count', 'Moderate Favorite Count', 'High Favorite Count', 'Very High Favorite Count' (Categorical)

Following Variables were used in the analysis:
* retweet_count - Retweet Counts (Quantitative).
* favorite_count - Favorite Counts (Quantitative)
* rating_numerator_new - Numerator Rating (Quantitative)
* dog_stage - Dog Stages ie pupper, puppo, doggo, floofer (Categorical)
* Dog Breed - Breed of Dogs (Categorical)

## Summary of Findings

> There is a strong positive relationship between retweet counts and favorite counts.
> There is a weak positive/no relationship between retweet counts and numerator ratings.
> Puppo stage seems to be the most common highly rated dog stage whereas pupper seems to be the most common low rated dog stage.
> Most Common Dog Stage: pupper being the most common followed by, puppo, doggo and with floofer being the least common dog stage.

In the following categories the most common dog stage can be found below for respective Retweet Count Classification Categories:
> * Very High Retweet Count: Puppo (Most Common) and Floofer (Least Common)
> * High Retweet Count: Puppo (Most Common) and Floofer (Least Common)
> * Moderate Retweet Count: Pupper (Most Common) and Floofer (Least Common)
> * Low Retweet Count: Pupper (Most Common) and Doggo (Least Common)

In the following categories the most common dog stage can be found below for respective Favorite Count Classification Categories:
> * Very High Favorite Count: Puppo (Most Common) and Floofer (Least Common)
> * High Favorite Count: Puppo (Most Common) and Floofer (Least Common)
> * Moderate Favorite Count: Pupper (Most Common) and Floofer (Least Common)
> * Low Favorite Count: Pupper (Most Common) and Doggo (Least Common)

> Most Common Dog Breed: Golden Retriever being the most common followed by, Pembroke, Pug, Pomeranian, Labrador Retriever and with Samoyed being the least common dog breed.
> Pembroke breed seems to be the most common highly rated dog breed whereas Pug seems to be the most common low rated dog breed.

In the following categories the most common dog breed can be found below for respective Favorite Count Classification Categories:
> * Very High Favorite Count: Pembroke (Most Common)
> * High Favorite Count: Pembroke & Golden Retriever (Most Common)
> * Moderate Favorite Count: Pomeranian & Pug (Most Common)
> * Low Favorite Count: Golden Retriever (Most Common)


## References

[1] https://stackoverflow.com/questions/21702342/creating-a-new-column-based-on-if-elif-else-condition
[2] https://stackoverflow.com/questions/19937362/python-pandas-filter-string-data-based-on-its-string-length
[3] https://www.dataquest.io/blog/tutorial-add-column-pandas-dataframe-based-on-if-else-condition/
[4] https://stackoverflow.com/questions/17071871/how-to-select-rows-from-a-dataframe-based-on-column-values
[5] https://re-thought.com/pandas-value_counts/
[6] https://en.wikipedia.org/wiki/WeRateDogs
[7] https://twitter.com/dog_rates

Other References:
[8] https://www.shanelynn.ie/merge-join-dataframes-python-pandas-index-1/
[9] https://campus.datacamp.com/courses/analyzing-social-media-data-in-python/processing-twitter-text?ex=4
[10] https://www.w3schools.com/python/python_regex.asp
[11] https://stackoverflow.com/questions/36536495/capitalized-words-with-regular-expression?rq=1
