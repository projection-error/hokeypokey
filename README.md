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
  - **Result**: None yet (112 of 300)
  - **Last Updated**: 05/26/22
- **Prediction 2**: Highest rated opponent defeated within first 300 games: 1500
  - **Result**: 2253.0 (112 of 300)
  - **Last Updated**: 05/26/22
- **Prediction 3**: Lowest rated opponent loss within first 300 games: 900
  - **Result**: 1018.0 (112 of 300)
  - **Last Updated**: 05/26/22
- **Prediction 4**: A deterministic loss sequence exists.
  - **Result**: None encountered yet.
  - **Last Updated**: 05/26/22




- **Records** (Last Update: 05/26/22)
  - **Max Rating**: 1526 (112 games)
  - **Min Rating**: 1040 (112 games)
  - <a href=https://lichess.org/bLfpBhEo>**Max Poke w/ Win Record**: 23</a>
  - <a href=https://lichess.org/TxYEDFpd>**Max Poke Record**: 30.0</a>
  - <a href=https://lichess.org/uJ4TD3r4>**Shortest Game**: 0 (Win)</a>
  - <a href=https://lichess.org/eRlwkk4h>**Longest Game**: 132 (Loss)</a>
  - <a href=https://lichess.org/qVoLY73R>**Highest Rated Win**: 2253.0</a>
  - <a href=https://lichess.org/GP0UDQnc>**Lowest Rated Loss**: 1018.0</a>

- **Opponent Rating vs. My Rating**

![Opponent Rating vs  HokeyPokeyHero Rating](https://user-images.githubusercontent.com/84434778/170628341-bfa0a355-cb39-4aa4-bc29-c2c582e3dad9.png)


- **My Rating vs. Game**
 
![Elo Rating vs  Game](https://user-images.githubusercontent.com/84434778/170628352-a4a4441d-cfd0-48ec-b16b-fb254f04f7b4.png)




- **Cumulative WLD (+1,-1,+0.5)**

![W+D-L vs  Game #](https://user-images.githubusercontent.com/84434778/170628357-e4831079-c156-431e-8a82-a9f3d17618ee.png)



- **Relations with No Correlation**

![Pokes vs  Game Length](https://user-images.githubusercontent.com/84434778/170628386-e287cd79-fffe-4d68-ad83-e030c49ab0c4.png)


![Opponent Elo vs  Game Length](https://user-images.githubusercontent.com/84434778/170628378-4892e4d1-a2f4-47d8-a032-434e77652628.png)



- **Poke Distribution**

![Poke Distribution](https://user-images.githubusercontent.com/84434778/170628423-506978c8-d28f-404c-94ef-bda67e0f1532.png)




# Notes
## Lichess Data
- Chess games are stored in a PGN file. This stands for "Portable Game Notation". As I make analysis tools, I will use this as the base data structure to parse/analyze.
