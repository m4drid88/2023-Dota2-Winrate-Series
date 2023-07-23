# 2023-Dota2-Winrate-Series
winrate por series de equipos de Dota2 en 2023

The data was extracted from the STRATZ API https://stratz.com/welcome. 

Using GraphQL API you can get the same information:

```
{
  leagues(request: {leagueIds: [15438,15251,15089,15196,15439]}) {
    id
    displayName
    series (take: 100,) {
      id
      type
      leagueId
      lastMatchDateTime
      teamOne {
        id
        name
      }
      teamTwo {
        id
        name
      }
      teamOneWinCount
      teamTwoWinCount
      winningTeamId
    }
  }}

  
```
Take into account:
* Lima Major 2023
* Berlin Major 2023
* Bali Major 2023
* Riyadh Masters 2023

Dreamleague season 19 and 20 were not considered.
  
