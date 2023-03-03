# 2022-2023 Project4 - Game Design - Group 4




___

<details>
<summary>Table of Contents</summary>

- [2022-2023 Project4 - Game Design - Group 4](#2022-2023-project4---game-design---group-4)
- [Project Team](#project-team)
- [Stakeholders](#stakeholders)
- [1. Introduction](#1-introduction)
  - [1.1. Purpose of the document](#11-purpose-of-the-document)
  - [1.2. Purpose of the project](#12-purpose-of-the-project)
- [2. Goal of the project](#2-goal-of-the-project)
  - [2.1. In scope](#21-in-scope)
  - [2.2. Out of scope](#22-out-of-scope)
  - [2.3. Future updates](#23-future-updates)
  - [2.4. Deadlines](#24-deadlines)
- [3. The Game](#3-the-game)
- [3.1. The Opponents](#31-the-opponents)
- [3.2. The Towers](#32-the-towers)
- [4. Personas](#4-personas)
  - [4.1. The Gamer : Ethan](#41-the-gamer--ethan)
  - [4.2. The Worker : John](#42-the-worker--john)
  - [4.3. The Passionate : Chris](#43-the-passionate--chris)
  - [4.4. The Involved : Marie](#44-the-involved--marie)
- [5. Glossary](#5-glossary)
</details>

___


# Project Team

| Name                   | Role              |
| ---------------------- | ----------------- |
| Laura-Lee HOLLANDE     | Project Manager   |
| Nicolas MIDA           | Program Manager   |
| Alexis LASSELIN        | Tech Lead         |
| Vivien Bistrel TSANGUE | Software Engineer |
| Robin DEBRY            | QA                |

# Stakeholders

- ALGOSUP 
- Users

# 1. Introduction

## 1.1. Purpose of the document

This document is the functional specification of the game. It describes the game's features and the rules that govern them. It is intended for the development team, the testers and the players.

## 1.2. Purpose of the project 

The purpose of this project is to create a fully working game using Unreal Engine 4. We are completely free to choose the theme of the game, the game mechanics and the game's universe.

Our group has chosen to create a Tower Defense game based on a bank universe


# 2. Goal of the project

The goal of the project is to design, code, and produce a full game using Unreal Engine 4. It will, of course, be a small but polished game. Design, UI/UX, and testing are crucial. 

The final game will have to feature some sort of gameplay innovation, and be as bug-free as possible, as well as a polished, fun, thoroughly tested and iterated upon project. 

## 2.1. In scope

// TODO

## 2.2. Out of scope

A mobile version of the game is not planned for the moment. The game will be available on PC only.

Also, the game will be exclusively in English for the moment, a French translation will be added later.

A multiplayer mode is not planned for the moment.


## 2.3. Future updates

The game will be updated regularly with new features such as the current out of scope features, new maps, new opponents, new towers, new skins, etc... 

If the project is a success, we will also consider to publish the game on platforms such as Steam or Epic Games Store.

## 2.4. Deadlines

| Date       | Deliverable            | Description |
| ---------- | ---------------------- | ----------- |
| 2023-03-03 | One sheet document     |             |
| 2023-03-10 | Working Prototype      |             |
| 2023-03-24 | Demo / Vertical Slice  |             |
| 2023-04-07 | Final Game, Final Test |             |

Here's the workshop game pipeline:

Game Idea → Game Concept → One Sheet and Final Game Idea → Pitch → Prototype → Demo and/or Vertical Slice → Testing & Iterating → Final Game

# 3. The Game

Our game is a Tower Defense PC game based on a bank universe where the player has to defend his bank from different types of criminals thanks to several types of towers.

# 3.1. The Opponents

Here is a table of the different types of opponents that the player will have to face in the game :

| Opponent | Description | Health | Speed | Damage | Reward |
| -------- | ----------- | ------ | ----- | ------ | ------ |
| Thief    | A thief is a small opponent that will try to steal money from the bank. He will be able to steal money from the bank's vault. | X | X | X | X |
| Warrior | A warrior is a medium opponent  | X | X | X | X |
| Boss | A boss is a big opponent  | X | X | X | X |

# 3.2. The Towers

To defend the bank, the player will have to place towers on the map. Here is a table of the different types of towers that the player will be able to place :

| Tower | Type | Description | Damage | Range | Fire Rate | Cost |
| ----- | ---- | ----------- | ------ | ----- | --------- | ---- |
| Gunner | X | X | X | X | X | X |
| X | AOE | X | X | X | X | X |
| X | Slow | X | X | X | X | X |
| X | Burst | X | X | X | X | X |
| Banker | Income | X | X | X | X | X |




# 4. Personas

## 4.1. The Gamer : Ethan

<div align="center">
  <img src="./../Images/Personas/jeune1.jpeg" width="128">
</div>

Ethan is a 15 year old French student who loves playing all kinds of video games. He is currently studying in a high school, specifically in the computer science branch. He often visits the Steam shop to find new games because he is often bored with his games. Recently, he saw the release of our new game 


## 4.2. The Worker : John

<div align="center">
  <img src="./../Images/Personas/homme1.jpeg" width="128">
</div>

John is a 33 years old worker who works as a game designer in a video game company for 7 years. He likes to play some games in his free time and he is looking for a new game to play. His friend, Mike, a coworker, told him about our game.

## 4.3. The Passionate : Chris

<div align="center">
  <img src="./../Images/Personas/jeune2.jpeg" width="128">
</div>

Chris is a 24 year old game developer with a passion for video games, particularly tower defense games. He's in relationship with Marie, a 23 year old nurse. 

He really likes to finish every game he starts, especially collecting all the achievements. While he was on Github, he saw our game's repository and is really interested in it.

## 4.4. The Involved : Marie

<div align="center">
  <img src="./../Images/Personas/femme1.jpeg" width="128">
</div>

Marie is a 23 year old nurse who works in a hospital. She is in a relationship with Chris, a 24 year old game developer. She doesn't play video games at all, but she likes to watch Chris playing them. 

During a conversation with Chris, he told her about the game and she told him that she would like to try it.

<sub> All the profile pictures are from [Generated photo](https://generated.photos/faces/)</sub>

# 5. Glossary

| **Name** | **Abrevation** | **Definition** |
|:--------:|:--------------:|:--------------:|
| Area Of Effect | AOE | [Area of Effect](https://en.wikipedia.org/wiki/Glossary_of_video_game_terms#area_of_effect), commonly abbreviated as "AoE", refers to the range of an ability or attack that affects multiple targets within a specific area, rather than a single target. |
| Blueprints | BP | [Blueprints](https://docs.unrealengine.com/en-US/Engine/Blueprints/index.html) are visual scripting tools that allow you to create logic for your game without writing code. |
| C++ | C++ | [C++](https://en.wikipedia.org/wiki/C%2B%2B) is a general-purpose programming language created by Bjarne Stroustrup as an extension of the C programming language, or "C with Classes". |
| Steam | Steam | [Steam](https://store.steampowered.com/) is a digital distribution platform developed by Valve Corporation, which offers digital rights management (DRM), multiplayer gaming, video streaming and social networking services. |
| Tower Defense | TD | [Tower Defense](https://en.wikipedia.org/wiki/Tower_defense) is a subgenre of strategy video games in which the player must defend a particular location or path against waves of enemies by strategically placing defensive structures, such as towers or traps, along the path to defeat the enemies before they reach their destination. |
| Unreal Engine | UE | [Unreal Engine](https://www.unrealengine.com/en-US/) is a 3D computer graphics game engine developed by Epic Games. |
| Visual Studio | VS | [Visual Studio](https://visualstudio.microsoft.com/) is an integrated development environment (IDE) from Microsoft. It is used to develop computer programs, as well as websites, web apps, web services and mobile apps. Visual Studio uses Microsoft software development platforms such as Windows API, Windows Forms, Windows Presentation Foundation, Windows Store and Microsoft Silverlight. It can produce both native code and managed code. |

*All the links in this document are clickable and redirect to the source of our glossary.*

<sub>Created on 2023-02-28 by [Nicolas MIDA](https://www.linkedin.com/in/nicolas-mida/) </sub> 