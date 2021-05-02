# Movies-ETL

## Purpose
The purpose of this repository is to create an automated pipeline that takes in new data, performs the appropriate transformations of the dataset, and loads the data into existing tables. One function was created that takes in the three files: Wikipedia data, Kaggle metadata, and the MovieLens rating data and performs the ETL process by adding the data to a PostgreSQL database.

## Resources 
To load in the large ratings.csv file, lfs was utilized. LFS did not work on its own. The following code was utilized to push the file:

git config --global lfs.dialtimeout 60 <br/>
git config --global lfs.transfer.maxretries 5<br/>
GIT_TRACE=1 GIT_CURL_VERBOSE=1 git push -u origin master<br/>

This code was found on https://github.com/git-lfs/git-lfs/issues/1581
