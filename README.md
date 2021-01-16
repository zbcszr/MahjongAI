# MahjongAI

An exploration to Mahjong AI agent implemented using Python.

## Modes
Self-defined numbers of users
User can choose to play against 3 difficulty levels of AI:
- The easy level is very predictable and risk averse.
- The medium level uses 
- The hard level 

## Background

Unlike perfect-infomation games such as Go and chess, Mahjong is a multi-player incomplete-information game. An incomplete information game has certain portions of information which is private to other players and cannot be viewed by them. Mahjong AI agent is harder to develop comparing to many existing board games for three main reasons:

- Mahjong has a huge number of possible winning hands. Those winning hands can be very different from each other, and different hands result in different winning round scores of the round. A professional player needs to carefully choose what kind of winning hand to form in order to trade off the winning probability and winning score of the round.
- Each player has up to 13 private tiles in his/her hand
which are not visible to other players, and there are 14 titles in the dead wall,
which are invisible to all the players throughout the game, and 70 tiles in the
live wall, which will become visible once they are drawn and discarded by the
players. As a result, on average, for each information set (a decision point of
a player), there are more than 1048 hidden states that are indistinguishable to
him/her.
- the playing rule of Mahjong is complex: (1) there are different types
of actions including Riichi, Chow, Pong, Kong, discard, and (2) the regular order
of plays can be interrupted when making a meld (Pong or Kong), going Mahjong
(declaring a winning hand), or robbing a Kong. Because each player can have
up to 13 private tiles, it is hard to predict those interruptions, and therefore
we even cannot build a regular game tree.

## Topic under exploration
- 


## Reference

[Server endpoint](www.logos.t.u-tokyo.ac.jp/mjai/)

[Suphx: Mastering Mahjong with deep reinforcement learning](https://arxiv.org/pdf/2003.13590.pdf)

[Open sourced opponents1](https://github.com/gimite/mjai-manue)

[Open sourced opponents2](https://github.com/wistery-k/mjai-silica)


This repo acts as an extended project of [Mahjong](https://github.com/zbcszr/Mahjong). 
