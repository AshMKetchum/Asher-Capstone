# Factors Influencing Video Game Perception


## Table of Contents
* [Canva Dashboard](#Canva-dashboard)
* [Motivation](#motivation)
* [Question](#Data-Question)
* [Normalizing the Data](#normaling-the-data)
* [Problems and Hurdles](#problems-and-hurdles)
* [Technologies Used](#technologies-used)
* [Data Sources](#sources)
* [Conclusion](#conclusion)

## Canva Dashboard:
Link: https://www.canva.com/design/DAGwicSYNlQ/c4peS2KBP7OJMsSzDICEyg/edit?utm_content=DAGwicSYNlQ&utm_campaign=designshare&utm_medium=link2&utm_source=sharebutton

## Motivation:
Video game culture has changed many times over in my lifetime. From platformers and RPGs, to first person shooters, to online competition, it seems we are nearing the limit of creative and design abilities, so what comes next? This analysis hopes to provide insights for the "new Xbox release," Xbox Series X/S (released 2020). Specifically, the goal to provide a recommendation for a game-release that can increase market share.

Factors to be Analyzed Include:
- Genre
- Critic and User reviews
- Console
- Sales by Region
- Publisher
- Themes

## Data Question:
What style of game should Xbox develop and market as a headliner for the new Xbox Series X/S (2020), in order to increase market share?

## Normalizing the Data
The datasets I utilized were initially pulled in full, unless possible to filter on platformid. Every game's data across 19 consoles (selected based on popularity and brand_name) was drawn. Unfortunately, this process took multiple days, and it was not until after that I realized pulling the review data from giantbomb would take far too long, as it would not allow multiple game_ids to be searched for at a time, thus returning far fewer reviews per call than would have been necessary. In order to supplement the data from giantbomb with reviews, a datasource from Kaggle titled Video Game Sales with Ratings was used. Because of this, review data is only available through 2016.

## Problems and Hurdles
The largest challenge by far was realizing the limitations in the API. My goal in the beginning was to include multiple other factors, like max and min players, whether it's a sequel or an original, whether the character was popularized before or not, the astrological sign of main characters, etc. It was just too difficult and time consuming to utilize the game_ids to draw this information. In hinesight, it may have been a good idea to, early on in the process, have searched for a different API and/or drastically reduced the number of game ids used.

## Technologies Used
1) Python / pandas - for exploration, normalizing and aggregation of the dataset
2) Python / matplotlib - for initial mapping and understanding of the data
3) Python / requests, time, BeautifulSoup - for calling GiantBomb's API and extracting the data used
4) Python / ast, rapidfuzz - for joining datasets
4) Git - for version control
5) Power BI - for generating consistently branded and entertaining visuals, as well as a dashboard to further inspect specific games and consoles.
6) Canva - to create the presentation

## Data Sources
To answer the above questions I used the following sources to collect datasets for my analysis

Primary: https://www.giantbomb.com/api/
API designed for developers and analysts who are interested in all things gaming.

Supplementary: https://www.kaggle.com/datasets/jahnavipaliwal/video-game-reviews-and-ratings?resource=download
Dataset created by Jahnavi Paliwal using data drawn from Metacritic and VGChartz

## Conclusion
Xbox should seek partnership with the well known and respected publisher Squre Enix, based out of Japan. The focus should be an anime style RPG headline release, published by Square Enix, exclusively releasedon Xbox with the new Xbox Series X/S.