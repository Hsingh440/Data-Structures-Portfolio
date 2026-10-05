 # YouTube Video Analysis

## Research Question

How do YouTube video categories differ in views, likes, and comments among popular videos in the United States?

## Data Source

The dataset was collected using the YouTube Data API v3. The API provides information about YouTube videos, including video categories, views, likes, comments, and publication dates. The analysis focuses on popular videos returned for the United States.

## Unit of Analysis

The unit of analysis is one popular YouTube video returned by the YouTube Data API for the United States.

## Variables

The analysis uses five research variables:

1. **Video Category** — the category assigned to each YouTube video.
2. **Views** — the number of times a video has been viewed.
3. **Likes** — the number of users who liked a video.
4. **Comments** — the number of comments associated with a video.
5. **Published Date** — the date and time when the video was published.

## Dataset

The final dataset contains 50 popular YouTube videos and 5 research variables.

The dataset contains:

- 50 rows
- 5 columns
- 0 missing values after cleaning
- 0 duplicate rows

The video categories in the dataset include Gaming, Music, Film & Animation, Entertainment, People & Blogs, and Comedy.

## Data Cleaning

The data was checked for missing values, duplicate rows, and appropriate data types. Views, likes, and comments were converted to numeric values, while the published date was converted to a datetime format. YouTube category IDs were converted into category names using the YouTube Data API.

## Analysis

The analysis compares the number of popular videos in each category and calculates average views, likes, and comments by category.

The results show differences among categories. Film & Animation had the highest average views in this dataset. Music had the highest average likes, while Gaming had the highest average comments.

Because the categories contain different numbers of videos, the category averages should be interpreted as descriptions of this particular sample rather than as representative values for all YouTube videos.

## Limitations and Ethics

This dataset contains only 50 popular YouTube videos collected for the United States, so the results should not be generalized to all YouTube videos.

The categories are also unevenly represented. Gaming had 18 videos, while Comedy had only 1 video. This means averages for categories with fewer observations may be less stable.

Views, likes, and comments measure engagement but do not explain why a video received a particular level of engagement. Factors such as channel size, video length, audience demographics, recommendations, trends, and publication timing are not included in this analysis.

The analysis uses aggregate video-level statistics rather than information about individual viewers. The API data also represents a particular point in time, and engagement counts can change after collection.

## Code and Transparency

The analysis was completed in Python using pandas, requests, python-dotenv, and matplotlib. The data was collected through the YouTube Data API v3.

The Jupyter Notebook containing the code, data preparation, analysis, and visualizations is:

[View the Jupyter Notebook](youtube_video_analysis.ipynb)

The API key is stored in a local `.env` file and is not included in the GitHub repository.

ChatGPT was used as an AI assistance tool to help brainstorm the research question, explain API documentation, suggest code structure, troubleshoot coding steps, and help draft documentation. The code was run and checked in the Jupyter Notebook, and API information was checked against Google's official YouTube Data API documentation.

## References

Google for Developers. (n.d.). *YouTube Data API*. https://developers.google.com/youtube/v3

Hussain, K., Nusair, K., Junaid, M., & Aman, W. (2024). A two-actor model for understanding user engagement with content creators: Applying social capital theory. *Computers in Human Behavior, 156*, 108237. https://doi.org/10.1016/j.chb.2024.108237

Khan, M. L. (2017). Social media engagement: What motivates user participation and consumption on YouTube? *Computers in Human Behavior, 66*, 236–247. https://doi.org/10.1016/j.chb.2016.09.024

Liikkanen, L. A., & Salovaara, A. (2015). Music on YouTube: User engagement with traditional, user-appropriated and derivative videos. *Computers in Human Behavior, 50*, 108–124. https://doi.org/10.1016/j.chb.2015.01.067
