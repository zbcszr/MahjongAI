# MahjongAI

A side product of my exploration to Mahjong AI agent, implemented in Python. Because many factors need to be considered in a good Mahjong AI agent, I want to first break down the problem by separating decision process into different parts and make them into an extension that aid user while playing Riichi Mahjong. 

## Modes



## Why AI agent is complicated

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
This is a pure algorithm exploration of Mahjong AI. Many open source project uses machine learning instead. For future, I am hoping to take the reinforcement learning course at school and look into Mahjong AI using deep reinforcement learning [here](https://arxiv.org/abs/2003.13590).


## Reference



This repo is an extended project of [Mahjong](https://github.com/zbcszr/Mahjong). 
