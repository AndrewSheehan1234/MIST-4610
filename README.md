
# MIST 4610 Group Project 1 – World Cup Queries

# Team Members
  - Grey Mendenhall @greym12
  - Andrew Sheehan @AndrewSheehan1234
  - Avery Carabajal @AveryCarabajal

# Scenario Description
Our World Cup Database models the FIFA World Cup tournaments and provides a  way to analyze each match, player, team, league, season, and goal data. The database captures information from both the 2018 and 2022 tournaments and links the matches to the teams, players, and goals involved. This data system supports queries to calculate goal averages, find top scorers, explore team and league performance, and analyze tournament statistics over time. This database can help fans, managers, analysts, and even coaches to find valuable information about each player, and specific data about each team.



# Explanation of Data Model

Our data model represents the  World Cup and is meant to capture an overall view of the tournament and teams. It stores information about leagues, seasons, teams, players, matches, and goals, which will help with analysis of specific attributes of the tournament.

The League entity contains league information about each team, and each league can have many teams. This is an example of a many to many relationship. 

The Team entity stores team names and stadiums and is linked back to the League. Each team has many players, represented by the Player entity, which captures first name, last name, position, and what team they are on.

The Season entity is used to separate the two tournaments (2018 and 2022) and is linked to the match entity, which stores match date, home and away teams, and the final score. Each match can have many Goal records, which store the player who scored, the minute the goal was scored, the team, and if a player had an assist. 

This model allows for many different queries, including  top goal scorers, average goals per match, the most common scorelines, and evaluating team or league performance.

<img width="920" height="791" alt="Screenshot 2025-09-23 at 7 35 53 AM" src="https://github.com/user-attachments/assets/ce767f58-e6a1-4523-a882-e61859198a0a" />


# Data Dictionary

<img width="408" height="104" alt="Screenshot 2025-09-22 at 10 59 21 PM" src="https://github.com/user-attachments/assets/cf4ca1a4-2d78-4e61-80c0-e163aca0e213" />

<img width="411" height="100" alt="Screenshot 2025-09-22 at 10 59 27 PM" src="https://github.com/user-attachments/assets/6da66c6d-f95a-4936-a781-0b1120158bf1" />


<img width="499" height="142" alt="Screenshot 2025-09-22 at 11 01 49 PM" src="https://github.com/user-attachments/assets/55efeb0a-b3a4-4043-b5d2-4d981263b47a" />


<img width="504" height="127" alt="Screenshot 2025-09-22 at 11 02 24 PM" src="https://github.com/user-attachments/assets/abdf485a-13cb-40cc-94f2-06b703324306" />

<img width="581" height="174" alt="Screenshot 2025-09-22 at 11 05 18 PM" src="https://github.com/user-attachments/assets/5ea4f7f5-c4c8-4cec-b2c4-2bca0dcdb12d" />

<img width="579" height="166" alt="Screenshot 2025-09-22 at 11 06 57 PM" src="https://github.com/user-attachments/assets/3d7b65b0-850a-4fb3-87a9-075b8130d9f4" />

# Queries

Query 1:
This query shows how many teams are not from the US. A soccer manager would care about this because different countries bring different styles of play, requiring a new tactical approach for each international team. A financial manager would care because playing away at an international club would require traveling and logistics costs, while also bringing the benefit of exposure to a new market.
<img width="829" height="299" alt="Screenshot 2025-09-22 at 11 08 54 PM" src="https://github.com/user-attachments/assets/7242d0e3-ae88-4a86-bfa1-6f3b2fc93659" />



Query 2: 
This query lists every team in the 2022 World Cup and shows the total number of goals they scored when playing at home. A manager would care about this because it allows them to compare home performance across all teams, identify which teams take the most advantage of home-field advantage, and adjust strategy accordingly. From a business perspective, this information can help organizers and analysts understand which teams produce the most exciting matches at home, which could influence scheduling decisions, marketing focus, and revenue forecasting for ticket sales, broadcasting, and merchandise.
<img width="842" height="334" alt="Screenshot 2025-09-22 at 11 09 22 PM" src="https://github.com/user-attachments/assets/2b7925fe-db09-4550-af8f-298450f745dd" />


Query 3:
This query lists all matches, including the date, home team, away team, and final score. A soccer manager would care about this because it lets them quickly review past results, identify what matches were wins, losses, or draws. A financial manager would care because it provides insight into match results that could affect ticket sales, sponsorship deals, and marketing campaigns. For example, a high scoring or close match might be used in promotional material to attract fans.
<img width="879" height="474" alt="Screenshot 2025-09-22 at 11 09 43 PM" src="https://github.com/user-attachments/assets/6a96797e-aa8f-4b16-9a92-bc5340c6bf2c" />



Query 4: 
This query would rank the top goalscorers in the league by the amount of goals them have descending. Soccer managers would care about this because it would allow them to identify players who drive attacks and use their goalscoring chances well. Financial managers would care about this because top goalscorers are usually stars and faces of the league, which would allow them to properly allocate marketing and sponsorship resources to players who would get them the most out of it
<img width="855" height="384" alt="Screenshot 2025-09-22 at 11 10 06 PM" src="https://github.com/user-attachments/assets/5d406978-2084-4a26-8a40-84d938de94a1" />



Query 5:
This query shows the amount of matches played in November and December. A soccer manager would care about this because this info is vital for planning training and rest days in order to not fatigue their players for the real matches. A financial manager would care about these because it would help them budget for staffing and advertisement costs, as these would probably go up or down depending on the amount of games played
<img width="872" height="339" alt="Screenshot 2025-09-22 at 11 10 25 PM" src="https://github.com/user-attachments/assets/65e4fda9-e91b-44bd-97f5-c045ffab600b" />



Query 6: 
This query shows the amount of teams who have an above average home goal record. A soccer manager would care about this because it would affect their tactics, such as playing more defensive against a team who is known to score a lot at home. A financial manager would care about this because home goals would create excitement for home fans because it would be an entertaining match, which in turn would give them more leverage from broadcasting deals since their matches are in high demand.

<img width="858" height="467" alt="Screenshot 2025-09-22 at 11 24 51 PM" src="https://github.com/user-attachments/assets/aeba10c8-5e30-49b5-82fa-50a8e60c37fe" />



Query 7:
This query would just list every team and their stadium. Soccer managers would care about this because they can use it to see metrics like stadium capacity, distance from their own stadium and other things that can indirectly affect their players performance. Financial managers would care about this because if they were looking to start a new team, they could use this info for picking a spot that isn't already saturated with another team
<img width="890" height="429" alt="Screenshot 2025-09-22 at 11 10 58 PM" src="https://github.com/user-attachments/assets/83343931-878b-4b38-9b41-69c54258f5fe" />



Query 8:
This query would show the average goals per match in the 2018 world cup. A soccer manager would care about this because it helps them analyze whether highly aggressive teams performed well if the average was high, or if highly defensive teams performed better if the average was low. A financial manager would care about this because knowing the average goals per match could help them predict how engaged fans would be with the team, driving merchandise sales and repeat ticket purchases.
<img width="884" height="359" alt="Screenshot 2025-09-22 at 11 11 14 PM" src="https://github.com/user-attachments/assets/5277062d-da03-48eb-9a8b-538b108118c4" />



Query 9:
This query would show the most common scoreline in all the matches played in our data set. A soccer manager would care about this because it would show offensive and defensive trends, such as if 0-0 was the most common scoreline they would know most games are extremely defensive and could plan for that. A financial manager would care because it would allow them to forecast ticket and merchandise sales, as boring games would require the prices of tickets to be lowered and exciting games would allow them to raise prices for a high demand product.
<img width="873" height="424" alt="Screenshot 2025-09-22 at 11 11 43 PM" src="https://github.com/user-attachments/assets/dafbc16c-3c4f-46e8-ad42-e2140dc3d2c6" />


Query 10:
This query would simply count all the players who play on team France. A soccer manager would care about this because it shows the depth of the team and would help with smart substitutions and tactics. A financial manager would care about this because the total number of players affects payroll, and the allocation of resources as a bigger squad would require more staff for nearly everything, allowing the manager to make smart budgets.
<img width="864" height="342" alt="Screenshot 2025-09-22 at 11 13 06 PM" src="https://github.com/user-attachments/assets/59aca72d-b871-4457-8fe7-803a68314e47" />


# Database Information

<img width="1251" height="216" alt="Screenshot 2025-09-22 at 11 26 03 PM" src="https://github.com/user-attachments/assets/60da4756-5b01-42d5-9cc3-84d545def62c" />

Name of the database: br_glm11679








