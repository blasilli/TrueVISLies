# Twitter Misleading Visualizations Dataset

This dataset contains tweets that have been classified based on the presence of misleading visualizations. The tweets are labeled as either positive (misleading) or negative (not misleading), and they include various types of errors related to data visualization practices. 

The dataset is balanced, with an equal number of positive (misleading) and negative (not misleading) tweets.

## General Overview

- **Total number of tweets**: 2336

## Class Distribution

The dataset is labeled with the following sentiment classes:

- **Positive tweets (misleading)**: 1168
- **Negative tweets (not misleading)**: 1168

## Columns in the Dataset

The error columns are boolean flags indicating the presence of specific types of misleading visualizations in the tweet. Each tweet can have multiple errors flagged. The `class` column indicates whether the tweet is positive (misleading) or negative (not misleading).

Errors have been identified by: 
> Maxim Lisnic, Cole Polychronis, Alexander Lex, and Marina Kogan. 2023. Misleading Beyond Visual Tricks: How People Actually Lie with Charts. In Proceedings of the 2023 CHI Conference on Human Factors in Computing Systems (CHI '23). Association for Computing Machinery, New York, NY, USA, Article 817, 1–21. https://doi.org/10.1145/3544548.3580910

The dataset contains the following columns:

- `tweet_id`
- `class` negative/positive
- `error[Truncated axis]` boolean, indicating whether the tweet contains a misleading visualization with this error.
- `error[Dual axis]` boolean, indicating whether the tweet contains a misleading visualization with this error.
- `error[Value as area/volume]` boolean, indicating whether the tweet contains a misleading visualization with this error.
- `error[Inverted axis]` boolean, indicating whether the tweet contains a misleading visualization with this error.
- `error[Uneven binning]` boolean, indicating whether the tweet contains a misleading visualization with this error.
- `error[Unclear encoding]` boolean, indicating whether the tweet contains a misleading visualization with this error.
- `error[Inappropriate encoding]` boolean, indicating whether the tweet contains a misleading visualization with this error.
- `error[Cherry-picking]` boolean, indicating whether the tweet contains a misleading visualization with this error.
- `error[Setting an arbitrary threshold]` boolean, indicating whether the tweet contains a misleading visualization with this error.
- `error[Causal inference]` boolean, indicating whether the tweet contains a misleading visualization with this error.
- `error[Issues with data validity]` boolean, indicating whether the tweet contains a misleading visualization with this error.
- `error[Failure to account for statistical nuance]` boolean, indicating whether the tweet contains a misleading visualization with this error.
- `error[Misrepresentation of scientific studies]` boolean, indicating whether the tweet contains a misleading visualization with this error.
- `error[Incorrect reading of chart]` boolean, indicating whether the tweet contains a misleading visualization with this error.


## Dataset Folder Structure

The dataset folder contains the following structure:

- `index.csv`: A CSV file with metadata and error classifications for each tweet.
- `data/`: A folder containing one JSON file per tweet, with detailed information.
- `texts/`: A folder containing one plain text file per tweet, with the tweet content.
- `images/`: A folder containing one PNG image per tweet, corresponding to the tweet content.

## Fields in the JSON Files

Each JSON file in the `data/` folder contains the following fields:

- `id`: The unique identifier of the tweet.
- `author`: The name or handle of the user who posted the tweet.
- `date`: The timestamp when the tweet was published (in ISO 8601 format).
- `text`: The content of the tweet as plain text.
- `tweet_url`: The URL pointing to the tweet on Twitter.
- `image_url`: The URL pointing to the image embedded in the tweet, hosted on Twitter.
- `image_png_base64`: The PNG image embedded in the tweet, encoded in base64 format.

Each JSON file and PNG image file is named using the tweet ID, following the pattern `<tweet_id>.json` and `<tweet_id>.png`.



