---
layout: post
title: Shot Charts in iPython (Module Nightmares)
---



```python
%matplotlib inline
```


```python
import requests
import matplotlib.pyplot as plt
import pandas as pd
import seaborn as sns
shot_chart_url = 'http://stats.nba.com/stats/shotchartdetail?CFID=33&CFPAR'\
                'AMS=2014-15&ContextFilter=&ContextMeasure=FGA&DateFrom=&D'\
                'ateTo=&GameID=&GameSegment=&LastNGames=0&LeagueID=00&Loca'\
                'tion=&MeasureType=Base&Month=0&OpponentTeamID=0&Outcome=&'\
                'PaceAdjust=N&PerMode=PerGame&Period=0&PlayerID=201935&Plu'\
                'sMinus=N&Position=&Rank=N&RookieYear=&Season=2014-15&Seas'\
                'onSegment=&SeasonType=Regular+Season&TeamID=0&VsConferenc'\
                'e=&VsDivision=&mode=Advanced&showDetails=0&showShots=1&sh'\
                'owZones=0'
```


```python
# Get the webpage containing the data
response = requests.get(shot_chart_url)
# Grab the headers to be used as column headers for our DataFrame
headers = response.json()['resultSets'][0]['headers']
# Grab the shot chart data
shots = response.json()['resultSets'][0]['rowSet']
```


```python
shot_df = pd.DataFrame(shots, columns=headers)
# View the head of the DataFrame and all its columns
from IPython.display import display
with pd.option_context('display.max_columns', None):
    display(shot_df.head())
```


<div>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>GRID_TYPE</th>
      <th>GAME_ID</th>
      <th>GAME_EVENT_ID</th>
      <th>PLAYER_ID</th>
      <th>PLAYER_NAME</th>
      <th>TEAM_ID</th>
      <th>TEAM_NAME</th>
      <th>PERIOD</th>
      <th>MINUTES_REMAINING</th>
      <th>SECONDS_REMAINING</th>
      <th>EVENT_TYPE</th>
      <th>ACTION_TYPE</th>
      <th>SHOT_TYPE</th>
      <th>SHOT_ZONE_BASIC</th>
      <th>SHOT_ZONE_AREA</th>
      <th>SHOT_ZONE_RANGE</th>
      <th>SHOT_DISTANCE</th>
      <th>LOC_X</th>
      <th>LOC_Y</th>
      <th>SHOT_ATTEMPTED_FLAG</th>
      <th>SHOT_MADE_FLAG</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>Shot Chart Detail</td>
      <td>0021400003</td>
      <td>18</td>
      <td>201935</td>
      <td>James Harden</td>
      <td>1610612745</td>
      <td>Houston Rockets</td>
      <td>1</td>
      <td>9</td>
      <td>58</td>
      <td>Missed Shot</td>
      <td>Jump Shot</td>
      <td>3PT Field Goal</td>
      <td>Right Corner 3</td>
      <td>Right Side(R)</td>
      <td>24+ ft.</td>
      <td>22</td>
      <td>226</td>
      <td>39</td>
      <td>1</td>
      <td>0</td>
    </tr>
    <tr>
      <th>1</th>
      <td>Shot Chart Detail</td>
      <td>0021400003</td>
      <td>39</td>
      <td>201935</td>
      <td>James Harden</td>
      <td>1610612745</td>
      <td>Houston Rockets</td>
      <td>1</td>
      <td>8</td>
      <td>25</td>
      <td>Missed Shot</td>
      <td>Layup Shot</td>
      <td>2PT Field Goal</td>
      <td>Restricted Area</td>
      <td>Center(C)</td>
      <td>Less Than 8 ft.</td>
      <td>2</td>
      <td>-15</td>
      <td>15</td>
      <td>1</td>
      <td>0</td>
    </tr>
    <tr>
      <th>2</th>
      <td>Shot Chart Detail</td>
      <td>0021400003</td>
      <td>41</td>
      <td>201935</td>
      <td>James Harden</td>
      <td>1610612745</td>
      <td>Houston Rockets</td>
      <td>1</td>
      <td>8</td>
      <td>21</td>
      <td>Made Shot</td>
      <td>Jump Shot</td>
      <td>3PT Field Goal</td>
      <td>Above the Break 3</td>
      <td>Left Side Center(LC)</td>
      <td>24+ ft.</td>
      <td>25</td>
      <td>-232</td>
      <td>110</td>
      <td>1</td>
      <td>1</td>
    </tr>
    <tr>
      <th>3</th>
      <td>Shot Chart Detail</td>
      <td>0021400003</td>
      <td>95</td>
      <td>201935</td>
      <td>James Harden</td>
      <td>1610612745</td>
      <td>Houston Rockets</td>
      <td>1</td>
      <td>4</td>
      <td>32</td>
      <td>Missed Shot</td>
      <td>Jump Shot</td>
      <td>2PT Field Goal</td>
      <td>Mid-Range</td>
      <td>Left Side Center(LC)</td>
      <td>16-24 ft.</td>
      <td>19</td>
      <td>-146</td>
      <td>135</td>
      <td>1</td>
      <td>0</td>
    </tr>
    <tr>
      <th>4</th>
      <td>Shot Chart Detail</td>
      <td>0021400003</td>
      <td>120</td>
      <td>201935</td>
      <td>James Harden</td>
      <td>1610612745</td>
      <td>Houston Rockets</td>
      <td>1</td>
      <td>2</td>
      <td>38</td>
      <td>Made Shot</td>
      <td>Driving Layup Shot</td>
      <td>2PT Field Goal</td>
      <td>Restricted Area</td>
      <td>Center(C)</td>
      <td>Less Than 8 ft.</td>
      <td>2</td>
      <td>-8</td>
      <td>22</td>
      <td>1</td>
      <td>1</td>
    </tr>
  </tbody>
</table>
</div>



```python
sns.set_style("white")
sns.set_color_codes()
plt.figure(figsize=(12,11))
plt.scatter(shot_df.LOC_X, shot_df.LOC_Y)
plt.show()
```

    /Library/Frameworks/Python.framework/Versions/3.5/lib/python3.5/site-packages/matplotlib/collections.py:590: FutureWarning: elementwise comparison failed; returning scalar instead, but in the future will perform elementwise comparison
      if self._edgecolors == str('face'):



![png](/img/output_4_1.png)



```python

```
