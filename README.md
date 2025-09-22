
# MIST 4610 Group Project 1 – World Cup Queries

# Team Members
  - Grey Mendenhall @greym12
  - Andrew Sheehan
  - Avery Carabajal

# Scenario Description
Our World Cup Database models the FIFA World Cup tournaments and provides a  way to analyze each match, player, team, league, season, and goal data. The database captures information from both the 2018 and 2022 tournaments and links the matches to the teams, players, and goals involved. This data system supports queries to calculate goal averages, find top scorers, explore team and league performance, and analyze tournament statistics over time. This database can help fans, managers, analysts, and even coaches to find valuable information about each player, and specific data about each team.

# Data model


# Explanation of Data Model

Our data model represents the  World Cup and is meant to capture an overall view of the tournament and teams. It stores information about leagues, seasons, teams, players, matches, and goals, which will help with analysis of specific attributes of the tournament.

The League entity contains league information about each team, and each league can have many teams. This is an example of a many to many relationship. 

The Team entity stores team names and stadiums and is linked back to the League. Each team has many players, represented by the Player entity, which captures first name, last name, position, and what team they are on.

The Season entity is used to separate the two tournaments (2018 and 2022) and is linked to the match entity, which stores match date, home and away teams, and the final score. Each match can have many Goal records, which store the player who scored, the minute the goal was scored, the team, and if a player had an assist. 

This model allows for many different queries, including  top goal scorers, average goals per match, the most common scorelines, and evaluating team or league performance.

PICTURE


## 📝 Queries

### Query 1 – [Title]
**Description:** [Explain in natural language what the query does.]  
**Managerial Justification:** [Explain why a manager would care about this information.]  

**SQL Code:**
```sql



