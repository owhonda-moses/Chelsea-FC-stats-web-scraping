# <img src="image/cfc_logo.png" width="40" height="40" /> Web Scraping of Chelsea FC Stats under Thomas Tuchel



## Dataset

> I'm a huge soccer fan and Chelsea FC supporter, and following the sack of [Thomas Tuchel](https://www.chelseafc.com/en/news/article/chelsea-football-club-part-company-with-thomas-tuchel) as Chelsea head coach, I wanted to see stats of his performance at the club. I found this [website](https://fbref.com/en/squads/cff3d9bb/2021-2022/Chelsea-Stats) that logs detailed soccer stats for all soccer clubs. Using BeautifulSoup and request libraries, I scraped data for the three seasons Thomas was head coach at Chelsea and subset the data to matches he coached. The following is a glossary of column headers in the dataframe as provided by StatsBomb and Data Sports Group -
- Date -- _Date listed is local to the match_
- Time -- _Time listed is local to the match venue in the 24-hour notation_
- Comp -- _Competition_
- Round -- _Round or Phase of Competition_
- Day -- _Day of week_
- GF -- _Goals For_
- GA -- _Goals Against_
- xG -- _Expected Goals (xG totals include penalty kicks, but do not include penalty shootouts unless otherwise noted)_
- xGA -- _Expected Goals Allowed (xG totals include penalty kicks, but do not include penalty shootouts unless otherwise noted)_
- Poss -- _Possession (calculated as the percentage of passes attempted)_
- Formation -- _Number of players in each row from defenders to forwards, not including the goalkeeper_

After gathering the data, I did some preliminary data pre-processing which reduced the variables to 12 with a total of 100 matches, and then, carried out exploratory analysis and stored the clean data in csv format.


## Key Findings

From the analysis:

- Thomas Tuchel was Chelsea head coach for exactly 100 games, winning a total of 63 matches or 63% of all games with 47 clean sheets. 18% ended in a loss and 19% were draws, and most matches were played on Home ground.
- Chelsea played in a total of six official competitions under Tuchel. He lost two FA Cup and one EFL Cup finals and won one UEFA Champions League final, one FIFA Club World Cup, and one UEFA Super Cup.
- Chelsea never lost to Tottenham or Crystal Palace under Thomas Tuchel and he conceded the most goals in a single match against Premier league side, West Bromwich Albion.
- On estimated average, Chelsea scored two goals per match and conceded one goal per match under Tuchel.
- Although Chelsea used the 3-4-3 formation 67% of the time under Tuchel, the midfield seemed to have better ball possession when using the 3-4-1-2 formation.
- The 4-2-2-2 formation was rarely used by Tuchel, however the 4-4-2 was the least used formation by Tuchel and was only used once just days before his contract termination at Chelsea.
- N'Golo Kanté in the midfield and as Chelsea captain always ended in a win for Chelsea under Tuchel.

###### _It could have been better but his performance stats at Chelsea isn't too shabby._

>>>_PS: I selected a dark background for the viz because I use a dark theme in my Jupyter notebook._

#### PACKAGES USED:

- Pandas
- NumPy
- BeautifulSoup
- request
- Matplotlib
- Seaborn

_References for this repo include:_
- https://www.transfermarkt.com
- https://en.wikipedia.org/wiki/Thomas_Tuchel
- https://stackoverflow.com/
