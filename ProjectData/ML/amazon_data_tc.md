### Project Description

> `Text Classification Algorithm For Twitter Data` is a simple `ML` project made using `CNN` model. On given a review it tells us the rating of it. Here I used Amazon reviews data in the `csv` format.

> What all I used in this Project:-
> + Language : `Python`
> + ML Model : `CNN`
> + Packages / Libraries : `tensorflow`, `keras`, `pandas`, `numpy`, `plotly`, `pyplot`, `re`, `string`, `nltk`, `Counter`, `Tokenizer`, `pad_sequences`, `layers`


+ Firstly I imported the primary modules / libraries. Then I imported the dataset.

+ Then I removed the duplicates and the null values from the dataset. An then visualized the data using `plotly` library.

+ Then I preprocessed the data using `re`, `string` for removing **urls** & **punctuations** as they are unnecessary for the model. Then using `nltk` library I removed the **stop words**.

> **Stop Words:** *A stop word is a commonly used word (such as “the”, “a”, “an”, “in”) that a search engine has been programmed to ignore, both when indexing entries for searching and when retrieving them as the result of a search query.*

+ Using `counter` I indexed the words in the review column. Then I splitted the data set into `training`  and `validation` sets.

+ Then I tokenized the text of the review column using `Tokenizer` and added post padding using `pad_sequences` for having same length.

+ Next I created the CNN Model for our project. The Structure of this Sequential Model is as given below :

![Image: CNN Model](https://user-images.githubusercontent.com/71878747/212282179-e451efec-10ba-4706-b6c2-f7357bcb8840.png)

+ Then I trained the model using `training` dataset and validated the output. And also plotted the `loss` and `accuracy` of the model.

+ The `python notebook` of this project is available in the Github Repository. The link to the Github Repo is [Amazon Data Analysis](https://github.com/mnk17arts/Text-Classification-Algorithm-for-analysing-Amazon-Reviews-data)

