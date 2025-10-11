# Getting the Data
1. Download the data from here: https://www.kaggle.com/datasets/tumanovalexander/nyt-articles-data
1. Open the zip file and save the `nyt_data.parquet` file into this folder. (`src/raw_data/nyt_data.parquet`)


# Discovery
There is a total of 17,370,913 articles.

## Year
- Range of articles is 1920-2020
- All years within the range are accounted for.

## Title
- There are 10,718,164 rows with the same title.
- Some of the articles have "No Title" in the title.
- Some articles aren't in english.

## Raw Data Format
This dataset in parquet format. For reading data use pd.read_parquet('nyt_data.parquet').

|Year|Title|Excerpt|
|---|---|---|
|The year the article was published|The title of the NYT article|An excerpt from the article|

