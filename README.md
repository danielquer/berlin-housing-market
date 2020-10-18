  # Ironhack-project-1 - NBA

## NBA 1984-2018: How the game changed in 30 years 

Data Thieves Project by:

* Victoria Essien
* Caner Bulut
* Daniel Quer

### Goals of the project
* As NBA fans, we have seen how the game has become more dynamic, points, point and shooting guards have become the dominators in the court. 
* We wanted to see how data backed this feeling, from two angles: 
* The performance angle: how many of the points are scored from beyond the 7.25 line. Are topscorers nowadays the 3- point shooters? 
* The economic angle: how much better paid are topscorers vs the rest of the team and compared to the 80s?


#### Data - sources, problems and limitations

#### We used three different data sources:
* Stats.nba.com API : we obtained here data for the performance of NBA players from 1984 to 2018. Format: JSON files
* Data World : (https://data.world/datadavis/nba-salaries) : we obtained here data for the salaries of players from 1984 to 2018. Format: 2 csv files
* We eventually had to use a [package] provided by a Git user to solve a referential integrity problem. Format: dictionary.

#### Data - sources, problems and limitations
* Data proved to be very clean, but one of the datasets contained a couple of limitations:
* 1. The Dataworld dataset was incomplete for seasons 1986-87 and 1989-90. We had to remove these seasons from the 
scope of our exercise, as they biased conclusions on:

* Salaries
* Positions of the players in the court

* 2. Some players that the NBA stats service recognized as active (because they had at least one minute played in a game during the season) were not present in the Dataworld dataset. These players were removed when grouping players by position and salary.

#### Project learnings
###### Stats API: 
* session = requests.Session()
* session.headers.update({'User-Agent': 'Custom user agent'})
* response = session.get(url)
* Working on GitHub together
* Merging dataframes and data wrangling
* Creating lookup values in data frames
* Plotting and combo colors




