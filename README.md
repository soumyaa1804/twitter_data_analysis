# twitter_data_analysis

The `network analysis` notebook takes a keyword and extracts 1000 most recent tweets containing that keyword. It then finds similar tweet-pairs using `Cosine-Similarity` once using `Bag-of-Words` vector and other time `TF-IDF` vector.


The notebook also creates the graph of followers and following relationship of the unique authors of those 1000 tweets.


## To be done:

Find popular users in the graph based on 
    * Degree centrality
    * Betweeness centrality
    * Closeness centrality


## Run on local machine:

1. Create a twitter developer account from [here](https://developer.twitter.com/en/apply-for-access)

2. `cd` to the repository and create a virtual environment and activate it:

```
virtualenv -p usr/bin/python3.8 env
source env/bin/activate
```

3. Install the libraries from requirements.txt:

`pip install -r requirements.txt`

4. Create a file by the name `secrets.py` and copy the content of `secrets_template.py` to `secrets.py`. Add your secret keys, which you got by creating an app on twitter developers account, in `secrets.py` file.

5. Run `jupyter notebook` to run all notebooks inside this repository locally.

----

