# Factors Influencing Video Game Perception


## Table of Contents
* [Power BI Dashboard](#Power-BI-dashboard)
* [Motivation](#motivation)
* [Question](#Data-Question)
* [Normalizing the Data](#normaling-the-data)
* [Problems and Hurdles](#problems-and-hurdles)
* [Technologies Used](#technologies-used)
* [Data Sources](#sources)
* [Conclusion](#conclusion)

## Power BI Dashboard:
Link:

## Motivation:
My goal with this project is to have a fun and unique insight into what influences a users perception of a game and the console. These insights will then be presented to the game development leads for the new Next Generation Xbox with the goal being to influence the strategic direction of game development pre-release. 

Factors to be Analyzed Include:
- Original release vs sequel
- Genre
- Critic reviews
- Difference between expected release date and the actual release date
- Company i.e. Nintendo, PlayStation, etc
- Primary console the game was intended for and/or released on
- Number of consoles sold
- Number of platforms available to be played on
- Astrological sign of the main character.

## Data Question:
What factors consciously or subconsciously affect users perception of a game? I have chosen to look at a select 19 platforms released between 1989 and 2025.

## Normalizing the Data
The datasets I utilized were initially pulled in full, unless possible to filter on platformid. The 19 platforms were selected based on popularity and brand_name, as well as to provide a picture of these trends over multiple decades. Once the full data sets were brought in, a list of games is compiled primarily utilizing game ids of the most reviewed games as well as the highest and lowest average star review. Additionally studys on consoles for average star rating of total games. The list of games previously mentioned allows the game id to be called which includes genre ids, allowing a look at user reviews by game based on genre.

## Problems and Hurdles
The largest issue so far is extracting the data, due to the limitations of the API. It allows for 200 calls to each id per hour, and limits the results of each call to a max of 100. This means 20000 is the max results per hour. This is a doable process, but involves a lot of additional time dedicated to waiting for the next hour to draw results, and quite specific code.

The other slight challenge is a lack of unique ids to link on. While there are a lot of datasets with unique ids, they often do not join in with the games or platforms id. The factors listed under “Data Question” all appear accessible to analyze, until the data is retrieved it will be difficult to know for sure.

## Technologies Used
1) Python / pandas - for exploration, normalizing and aggregation of the dataset
2) Python / matplotlib - for initial mapping and understanding of the data
3) Python / requests, time, BeautifulSoup - for calling GiantBomb's API and extracting the data used
4) Git - for version control
5) Power BI - for generating consistently branded and entertaining visuals, as well as a dashboard to further inspect specific games and consoles.
6) Canva - to create the presentation

## Data Sources
To answer the above questions I used the following sources to collect datasets for my analysis

1) API designed for developers and analysts who are interested in all things gaming.
https://www.giantbomb.com/api/

## Conclusion
Unknown