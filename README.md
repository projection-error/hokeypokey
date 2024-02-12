# Newest Development in Chess Theory - 
# The Hokey Pokey Opening
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
  - **Result**: None yet (425 of 300)
  - **Last Updated**: 06/10/22
- **Prediction 2**: Highest rated opponent defeated within first 300 games: 1500
  - **Result**: 2311.0 (425 of 300)
  - **Last Updated**: 06/10/22
- **Prediction 3**: Lowest rated opponent loss within first 300 games: 900
  - **Result**: 976.0 (425 of 300)
  - **Last Updated**: 06/10/22
- **Prediction 4**: A deterministic loss sequence exists.
  - **Result**: None encountered yet.
  - **Last Updated**: 06/10/22



# Records (Last Update: 06/10/22)
  - **Max Rating**: 1646 (425 games)
  - **Min Rating**: 1040 (425 games)
  - <a href=https://lichess.org/IzSMbpTY>**Max Poke w/ Win Record**: 23</a>
  - <a href=https://lichess.org/UTc9KIXJ>**Max Poke Record**: 34.0</a>
  - <a href=https://lichess.org/uJ4TD3r4>**Shortest Game**: 0 (Win)</a>
  - <a href=https://lichess.org/hxJhZhah>**Longest Game**: 160 (Loss)</a>
  - <a href=https://lichess.org/qpUAMkG6>**Highest Rated Win**: 2311.0</a>
  - <a href=https://lichess.org/CnTGE0pW>**Lowest Rated Loss**: 976.0</a>

- **Opponent Rating vs. My Rating**

![Opponent Rating vs  HokeyPokeyHero Rating](https://user-images.githubusercontent.com/84434778/173174149-ae16598b-c753-49c4-9531-79cca6ec0b82.png)



- **HokeyPokeyHero Rating vs. Game**
 

![Elo Rating vs  Game](https://user-images.githubusercontent.com/84434778/173174161-42974b2c-796f-4e59-a2f8-0e7a2f7b1719.png)



- **Cumulative WLD (+1,-1,+0.5)**


![W+D-L vs  Game #](https://user-images.githubusercontent.com/84434778/173174167-9d23d130-d203-47cd-a3a6-aef6864b66cb.png)



- **Correlations (or lack thereof)**

![Opponent Elo vs  Game Length](https://user-images.githubusercontent.com/84434778/173174169-432b441b-bc21-4646-986b-2b06a6c0156a.png)

![Pokes vs  Game Length](https://user-images.githubusercontent.com/84434778/173174180-7c4359bd-537c-4d7c-b1e9-0b42044c71ea.png)

![Pokes vs  Opponent Elo Rating](https://user-images.githubusercontent.com/84434778/173174188-0f790207-3dae-45d0-8479-04cd6178e09f.png)


- **Poke Distribution**

![Poke Distribution](https://user-images.githubusercontent.com/84434778/173174173-58d8a515-6aa1-4c74-8a98-7cc126524328.png)




# Notes
## Lichess Data
- Chess games are stored in a PGN file. This stands for "Portable Game Notation". As I make analysis tools, I will use this as the base data structure to parse/analyze.
