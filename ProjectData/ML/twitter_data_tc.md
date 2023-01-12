### Project Description

> `Text Classification Algorithm For Twitter Data` is a simple `ML` project made using `LSTM` model. On given a query the our model tells us whether it is a `disaster` or not. Here I used Twitter tweets data in the `csv` format. 

> What all I used in this Project:-
> Language : `Python`
> ML Model : `LSTM`
> Packages / Libraries : `tensorflow`, `keras`, `pandas`, `numpy`, `pyplot`, `re`, `string`, `nltk`, `Counter`, `Tokenizer`, `pad_sequences`, `layers`

+ Firstly I imported the primary modules / libraries. Then I imported the dataset. Upon seeing the data info I removed the unnecessary columns.

+ Secondly I preprocessed the data using `re`, `string` for removing **urls** & **punctuations** as they are unnecessary for the model. Then using `nltk` library I removed the **stop words**.

> **Stop Words:** *A stop word is a commonly used word (such as “the”, “a”, “an”, “in”) that a search engine has been programmed to ignore, both when indexing entries for searching and when retrieving them as the result of a search query.*

+ Using `counter` I indexed the words in the query column.

+ Then I splitted the data set into `training`  and `validation` sets. 

+ Then I tokenized the text of the Query column using `Tokenizer` and added post padding using `pad_sequences` for having same length.

+ Next I created the LSTM Model for our project. The Structure of this Sequential Model is as given below :

```
Model: "sequential"
_________________________________________________________________
 Layer (type)                Output Shape              Param #   
=================================================================
 embedding (Embedding)       (None, 20, 32)            575072    
                                                                 
 lstm (LSTM)                 (None, 64)                24832     
                                                                 
 dense (Dense)               (None, 1)                 65        
                                                                 
=================================================================
Total params: 599,969
Trainable params: 599,969
Non-trainable params: 0
_________________________________________________________________
```

+ Then I trained the model using `training` dataset and validated the output.

+ The `python notebook` of this project is available in the Github Repository. The link to the Github Repo is [Twitter Data Analysis]