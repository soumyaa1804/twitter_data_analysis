# twitter_data_analysis

The `network analysis` notebook does the following tasks:

1. Use Twitter API to collect 1000 tweets in which keyword ‘narendra modi’ appears, save the collected tweets in nm.txt

2. Convert the collected tweets into BoW vectors and find cosine similarity of a pair of tweets and print the top-10 most similar tweet pairs, print these pairs

3. Do the same using TF-IDF vectors

4. Find out unique users (N) who have posted these 1000 tweets. (N <= 1000)
    U1, u2, ….., uN
5. Find the followers and followee of each user from the N users obtained before
    * u1 - [followers list] [followee list]
    * u2 - [followers list] [followee list]
    * .
    * .
    * uN - [followers list] [followee list]
6. Followers and followees are also users, so create a follower-followee directed graph among them, G. (ui → uj) iff ui is followed by uj
7. Find popular users in this G based on 
    * Degree centrality
    * Betweeness centrality
    * Closeness centrality


## Run notebooks on local machine:

Create a twitter developer account from [here](https://developer.twitter.com/en/apply-for-access)

`cd` to the repository and create a virtual environment and activate it:

```
virtualenv -p usr/bin/python3.8 env
source env/bin/activate
```

Install the libraries from requirements.txt:

`pip install -r requirements.txt`

Create a file by the name `secrets.py` and copy the content of `secrets_template.py` to `secrets.py`. Add your secret keys, which you got by creating an app on twitter developers account, in `secrets.py` file.

Run `jupyter notebook` to run all notebooks inside this repository locally.

----

