# Newest Development in Chess Theory - The Hokey Pokey Opening
## Follow progress on Lichess: [HokeyPokeyHero](https://lichess.org/@/HokeyPokeyHero)
# Motivation
Introducing a newly invented chess opening - it's called the "Hokey Pokey". 

https://user-images.githubusercontent.com/84434778/168507658-2098ced7-569d-4d34-bf2b-4085fd2a4a83.mp4

# How it Works
```
while(!threat):
  if Nf3:
    Ng1
  else:
    Nf3
  threat = isThereAThreat()
   
```
<p align="center">Not 100% right - Na3,Nc3,and Nh3 are also allowed. The goal is to keep moving the knight until risk is near-existential.</p>

Once a threat is posed, the strategy is abandoned. Against engines/good players, this is a horrible strategy to take because the opponent gets free moves. However, I intend to explore the following interesting properties this opening presents:
- Non-Committal Position: Since I do not make a committal move until far into the game, there is opportunity for the positions to reach very unique set-ups and potentially advantageous asymmetries. Frequent play of this opening leads to a knowledge disparity that might enable an edge.
- Lowered Guard: An opponent may play with less focus or over-extend. Since I convert to playing normally once a threat is posed, I may be able to surprise them.
- Time Advantage: Although marginal, a slight time advantage over my opponent due to my fast pre-moves plus whatever time they spend raising their eyebrows (see below). In some blitz games, this may prove decisive.
- Fun: Because this opening is kind of hokey (literally), it leads to very unique positions that *may* enable advantages.
<p align="center"><img width=220 height=270 src=https://user-images.githubusercontent.com/84434778/169719125-44f0e78d-00a1-4b00-ad83-adf8d38ecbe7.png><br>
  Example - Opponent is in significant time trouble, regardless of the material balance in the position</p>


# Goals
- Play some games with the opening (Lichess: [HokeyPokeyHero](https://lichess.org/@/HokeyPokeyHero))
- Analyze commonalities in how the opponent responds 
- Analyze performance results
- Have fun

# Predictions
- **Prediction 1**: Games until an opponent counter-Hokey-Pokies into a draw: Within first 300 games.
  - **Result**: None yet (73 of 300)
  - **Last Updated**: 05/25/22
- **Prediction 2**: Highest rated opponent defeated within first 300 games: 1500
  - **Result**: 2066.0 (73 of 300)
  - **Last Updated**: 05/25/22
- **Prediction 3**: Lowest rated opponent loss within first 300 games: 900
  - **Result**: 1018.0 (73 of 300)
  - **Last Updated**: 05/25/22
- **Prediction 4**: A deterministic loss sequence exists.
  - **Result**: None encountered yet.
  - **Last Updated**: 05/25/22


# Progress
- **Records** (Last Update: 05/25/22)
  - **Max Rating**: 1514 (73 games)
  - **Min Rating**: 1040 (73 games)
  - <a href=https://lichess.org/bLfpBhEo>**Max Poke Record**: 23</a>
  - <a href=https://lichess.org/uJ4TD3r4>**Shortest Game**: 0 (Win)</a>
  - <a href=https://lichess.org/eRlwkk4h>**Longest Game**: 132 (Loss)</a>
  - <a href=https://lichess.org/kPS2hXrY>**Highest Rated Win**: 2066.0</a>
  - <a href=https://lichess.org/GP0UDQnc>**Lowest Rated Loss**: 1018.0</a>

- **Opponent Rating vs. My Rating**

![Opponent Rating vs  HokeyPokeyHero Rating](https://user-images.githubusercontent.com/84434778/170411664-4f984a48-a4e7-45a2-b809-d736f3820c94.png)

- **My Rating vs. Game**
 
![Elo Rating vs  Game](https://user-images.githubusercontent.com/84434778/170409818-37cd70d7-ed18-4b8c-8174-aa926faa6493.png)


- **Cumulative WLD (+1,-1,+0.5)**
- 
![W+D-L vs  Game #](https://user-images.githubusercontent.com/84434778/170409827-56a53f2c-ac0d-43bb-ad01-e879fb4ac9bd.png)



- **Relations with No Correlation**

![Opponent Elo vs  Game Length](https://user-images.githubusercontent.com/84434778/170409797-af5275cf-117e-4fc3-bfad-92cb52cfa281.png)

![Pokes vs  Game Length](https://user-images.githubusercontent.com/84434778/170409841-e3e548fa-1f9c-47c4-9cae-691adadfcb18.png)

![Pokes vs  Opponent Elo Rating](https://user-images.githubusercontent.com/84434778/170409852-fcb1d121-5d60-4124-9b8b-3dc49afc5324.png)


- **Poke Distribution**

![Poke Distribution](https://user-images.githubusercontent.com/84434778/170409791-821b7db5-df3c-4a20-8767-908eb5348b1d.png)



# Notes
## Lichess Data
- Chess games are stored in a PGN file. This stands for "Portable Game Notation". As I make analysis tools, I will use this as the base data structure to parse/analyze.
