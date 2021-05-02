# Movies-ETL

## Purpose
The purpose of this repository is to create an automated pipeline that takes in new data, performs the appropriate transformations of the dataset, and loads the data into existing tables. One function was created that takes in the three files: Wikipedia data, Kaggle metadata, and the MovieLens rating data and performs the ETL process by adding the data to a PostgreSQL database.

## Resources 
To load in the large ratings.csv file, lfs was utilized. LFS did not work on its own. The following code enabled the file to be pushed:

git config --global lfs.dialtimeout 60
git config --global lfs.transfer.maxretries 5
GIT_TRACE=1 GIT_CURL_VERBOSE=1 git push -u origin master

This code was received from https://github.com/git-lfs/git-lfs/issues/1581
