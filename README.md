# Spotify AWS ETL pipeline


### Introduction
In this pipeline we build an ETL using spotify API. THe pipeline will retriee data from the spotify API and then transform it to a desired format and then load it into an AWS data store

### Architecture
![](https://github.com/ansel9618/AWS-ETL-Data-pipeline/blob/main/images/2.0_architecture.png)

### Dataset/API
This spotify api will contain info about music artist,albums,songs - [GitHub Pages](https://developer.spotify.com/documentation/web-api)

### Services used
![](https://github.com/ansel9618/AWS-ETL-Data-pipeline/blob/main/images/3.0_.png)
![](https://github.com/ansel9618/AWS-ETL-Data-pipeline/blob/main/images/4.0_.png)

### Packages installed
```
pip install numpy
pip install pandas
pip install spotipy
```
### Project Execution Flow

* Integrating with Spotify API and extracting Data
* Deploying code on AWS Lambda for Data Extraction
* Adding trigger to run the extraction automatically
* Writing transformation function
* Building automated trigger on transformation function
* Store files on S3 properly
* Building Analytics Tables on data files using Glue and Athena

Extract data from API -> Lambda Trigger (every 1 hour) -> Run extract code -> Store raw data ->trigger transform function -> transform data and load it -> Query using Athena
