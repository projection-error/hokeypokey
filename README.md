# Newest Development in Chess Theory - The Hokey Pokey Opening
## Follow progress on Lichess: [HokeyPokeyHero](https://lichess.org/@/HokeyPokeyHero)
# Motivation
I have invented a new chess opening- it's called the "Hokey Pokey" opening. 

https://user-images.githubusercontent.com/84434778/168507658-2098ced7-569d-4d34-bf2b-4085fd2a4a83.mp4

# How it Works
```
while(!threat):
  threat = isThereAThreat()
  if Nf3 is True:
    Ng1
  else:
    Nf3
   
```


Once the threat is posed, I convert to my normal play strength (~1700-1800 bullet/blitz). Against engines/good players, this is a horrible strategy for me to take because I'm essentially wasting time. However, I intend to explore the following interesting properties it presents:
- Non-Committal Position: Since I do not make a committal move until far into the game, there is opportunity for the positions to reach very unique set-ups. These positions could prove advantageous to me.
- Lowered Guard: An opponent may play with less focus or over-extend. Since I convert to playing normally once a threat is posed, I may be able to surprise them.
- Time Advantage: Although marginal, I will achieve a slight time advantage over my opponent due to my fast pre-moves plus whatever time they spend raising their eyebrows. In some blitz games, this may prove decisive.

# Goals
- Play some games with the opening (Lichess: [HokeyPokeyHero](https://lichess.org/@/HokeyPokeyHero))
- Analyze commonalities in how the opponent responds 
- Analyze performance results
- Have fun

# Predictions
- **Prediction 1**: Games until an opponent counter-Hokey-Pokies into a draw: Within first 300 games.
  - **Result**: None yet (10 games)
- **Prediction 2**: Highest rated opponent defeated within first 300 games: 1500
  - **Result**: 1163 (10 of 300 games)
- **Prediction 3**: Lowest rated opponent loss within first 300 games: 900
  - **Result**: 1096 (10 of 300 games)
- **Prediction 4**: A deterministic loss sequence exists.
  - **Result**: None encountered yet.


# Progress
- 5/15/22: 
  - 10 games played. 5W/5L, 1217 (provisional) rating
  - First draw (Game 13)
  - 20 games played. 12W/6L/2D, 1383 rating

# Notes
## Lichess Data
- Lichess data is available at the link: >https://lichess.org/games/export/UserNameHere?since=1525132800000
- Chess games are stored in a PGN file. This stands for "Portable Game Notation". As I make analysis tools, I will use this as the base data structure to parse/analyze.
