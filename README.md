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
  - **Result**: None yet (51 of 300)
  - **Last Updated**: 05/21/22
- **Prediction 2**: Highest rated opponent defeated within first 300 games: 1500
  - **Result**: 2066 (51 of 300)
  - **Last Updated**: 05/21/22
- **Prediction 3**: Lowest rated opponent loss within first 300 games: 900
  - **Result**: 1018 (51 of 300)
  - **Last Updated**: 05/21/22
- **Prediction 4**: A deterministic loss sequence exists.
  - **Result**: None encountered yet.
  - **Last Updated**: 05/21/22


# Progress
- **Records** (Last Update: 05/22/22)
  - **Max Rating**: 1514 (51 games)
  - **Min Rating**: 1040 (51 games)
  - <a target="_blank" href=https://lichess.org/a3NNJvc3>**Max Poke Record (Resulting in a Win)**: 18</a>
  - <a target="_blank" href=https://lichess.org/uJ4TD3r4>**Shortest Game**: 0 (Win)</a>
  - <a target="_blank" href=https://lichess.org/RaDCMY6C>**Longest Game**: 131 (Win)</a>
  - <a target="_blank" href=https://lichess.org/kPS2hXrY>**Highest Rated Win**: 2066.0</a>
  - <a target="_blank" href=https://lichess.org/GP0UDQnc>**Lowest Rated Loss**: 1018.0</a>

- **Opponent Rating vs. My Rating**

![RatingJourney](https://user-images.githubusercontent.com/84434778/169716949-64eb0d7c-e372-434f-9d42-291a46352c67.png)

- **My Rating vs. Game**

![Elo Rating vs Time](https://user-images.githubusercontent.com/84434778/169717417-a1bc7c7e-895e-4f9a-ae6a-df36c7c018d5.png)

- **Cumulative WLD (+1,-1,+0.5)**

![WLD](https://user-images.githubusercontent.com/84434778/169716952-8f3b0c3b-d173-4678-a8e0-40549ac36cdf.png)

- **Relations with No Correlation**

![ElovGameLength](https://user-images.githubusercontent.com/84434778/169716968-b84ddcec-58ce-43b6-af2f-f89a0880fd5a.png)
![PokesvsElo](https://user-images.githubusercontent.com/84434778/169716975-71979702-1142-4811-818d-a22e22ee54a4.png)
![PokesvsGameLength](https://user-images.githubusercontent.com/84434778/169716976-3f664fb1-2c3b-44da-9dd5-78c382ae5b6f.png)

- **Poke Distribution**

![PokeDistribution](https://user-images.githubusercontent.com/84434778/169716945-951ebb04-b660-44b7-b129-2fe49a3c5723.png)


# Notes
## Lichess Data
- Chess games are stored in a PGN file. This stands for "Portable Game Notation". As I make analysis tools, I will use this as the base data structure to parse/analyze.
