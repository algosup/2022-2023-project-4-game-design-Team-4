# Game Design technical specification

## Team

Author: [Alexis Lasselin](https://github.com/alexislasselin)
Other team members:

- [Laura-Lee Hollande](https://github.com/lauraleehollande);
- [Nicolas Mida](https://github.com/Nicolas-Mida);
- [Vivien Bistrel Tsangue](https://github.com/Bistrel2002)
- and [Robin Debry](https://github.com/robin-debry).

---

<details>
<summary>Table of Contents</summary>

- [Game Design technical specification](#game-design-technical-specification)
	- [Team](#team)
	- [1. Introduction](#1-introduction)
		- [1.1. Purpose of the document](#11-purpose-of-the-document)
		- [1.2. Purpose of the project](#12-purpose-of-the-project)
	- [2. Minimum System Requirements](#2-minimum-system-requirements)
	- [3. Graphics](#3-graphics)
	- [4. User Interface](#4-user-interface)
	- [5. Audio](#5-audio)
	- [6. Gameplay Features](#6-gameplay-features)
		- [6.1. Tower Types](#61-tower-types)
			- [Basic Tower - The Gunner](#basic-tower---the-gunner)
			- [Slow Tower - The Bitcoin Launcher](#slow-tower---the-bitcoin-launcher)
			- [Splash Tower - The Potato Gun](#splash-tower---the-potato-gun)
		- [6.2. Enemy Types](#62-enemy-types)
		- [6.3. Stages Types](#63-stages-types)
		- [6.4. Win/Lose Conditions](#64-winlose-conditions)
		- [6.5. Rewards](#65-rewards)
		- [6.6. Upgrades](#66-upgrades)
	- [7. Programming](#7-programming)
		- [7.1 Programming Languages](#71-programming-languages)
			- [Why did we choose Blueprints?](#why-did-we-choose-blueprints)
		- [7.2 Software](#72-software)
			- [Why did we choose Unreal Engine 4?](#why-did-we-choose-unreal-engine-4)
	- [8. Testing and Debugging](#8-testing-and-debugging)
	- [9. Deployment Distribution Services](#9-deployment-distribution-services)
	- [10. Glossary](#10-glossary)

</details>

---

## 1. Introduction

### 1.1. Purpose of the document

<!--  Purpose of the document -->

This document is a technical specification of the game we are going to create. It is a document that will be used by the team to guide the development of the game. It will be used to define the game's universe, the game's mechanics and the game's assets.

### 1.2. Purpose of the project

<!--  Purpose of the project -->

The purpose of this project is to create a fully working game using Unreal Engine 4. We are completely free to choose the theme of the game, the game mechanics and the game's universe.

Our group has chosen to create a Tower Defense game based on a bank universe

## 2. Minimum System Requirements

<!-- Specifications for the minimum and recommended system requirements for the game. -->

For the moment, we are not sure about the minimum and recommended system requirements for the game. We will update this section when we will have more information about the game's assets.

<!-- Here are the minimum and recommended system requirements for the game:

| **Name** | **Minimum** | **Recommended** |
|:--------:|:-----------:|:---------------:| -->

## 3. Graphics

<!-- Specifications for character models, environments, textures, lighting, special effects, and other graphical elements, such as resolution, level of detail, shaders, etc. -->

- **Character Models**: We will use character models for the game's enemies, the game's towers, the game's upgrades, etc.
- **Interface**: We will use interface for the game's menus, the game's UI, the game's levels, the game's win/lose conditions, the game's rewards, etc.
- **Particles**: We will use particles for the game's projectiles, the game's explosions, the game's bonuses, the game's ennemies (for example, the invisible version of the fast enemy), etc.

## 4. User Interface

<!-- Specifications for menus, buttons, icons, dialogue windows, progress indicators, progress bars, sliders, etc. -->

- **Main Menu**: Start Game, Tutorial, Options, Quit
- **In-game UI**: Tower selection, Upgrade, Pause
- **Dialogue Window**: "Congratulations, You Won!", "You Lost", "You Won the Level", "You Lost the Level", "You Won the Game", "You Lost the Game" and some explanations about the game in the tutorial.

## 5. Audio

<!-- Specifications for sound effects, music, voiceovers, etc. This includes sound quality, file format, audio channels, etc. -->

- **Sound Effects**: We will use sound effects for the game's menus (when a button is clicked), the game's towers (when you build them), the game's enemies (when they reach the vault), the game's projectiles, the game's upgrades, the game's win/lose conditions, the game's rewards, etc.
- **Music**: We will use music for the game's menus, the game's UI, the game's levels, the game's win/lose conditions, the game's rewards, etc.
- **Voiceovers**: We will probably not use voiceovers in the game.

## 6. Gameplay Features

<!-- Specifications for gameplay elements such as tower types, enemy types, level types, attack types, defense mechanisms, win/loss conditions, rewards, upgrades, bonuses, etc. -->

### 6.1. Tower Types

We will have 3 tower types: a basic tower, a slow tower and a splash tower (AOE).
All the statitics(*in italic*) of the towers given below are not final. They are just here to give you an idea of what we are thinking about.

#### Basic Tower - The Gunner

- **Description**: The basic tower is a tower that shoots dollars at the enemies. It is the most basic tower in the game.
- **Attack Type**: The basic tower shoots projectiles at the enemies. The projectiles are the most basic projectiles in the game, they deal damage to the enemies (*20 damage per projectile*) but the turret is the fastest turret in the game (*1 projectile per second*).

![The first design of the basic tower.](./../Images/Turrets/Gunner.png)

#### Slow Tower - The Bitcoin Launcher

- **Description**: The slow tower is a tower that shoots bitcoin at the enemies.
- **Attack Type**: The slow tower shoots projectiles at the enemies. The projectiles are the slowest projectiles in the game, they deal damage to the enemies (*15 damage per projectile*) and they slow the enemies (*20% slow for 2 seconds*). The turret get a medium speed (*1 projectile every 1.5 seconds*).

![The first design of the slow tower.](./../Images/Turrets/Bitcoin_Launcher.png)

#### Splash Tower - The Potato Gun

- **Description**: The splash tower is a tower that throws gold ingots at the enemies. The gold ingots explode when they hit an enemy.
- **Attack Type**: The splash tower is the one with the most damage in the game. The projectiles are the most powerful projectiles in the game, they deal damage to the enemies in a radius of 2X2 tiles (25 damage per projectile). To balance the tower, the turret is the slowest turret in the game (*1 projectile every 2 seconds*).

![The first design of the splash tower.](./../Images/Turrets/Potato_Gun.png)

### 6.2. Enemy Types

We will have 3 enemy types: a basic enemy, a fast enemy and a tank enemy. There will be different versions of each enemy type. For example, the fast enemy will have a version that is faster than the other versions of the fast enemy, or another version that can be invisible for a short period of time. There is also a boss enemy, which is a combination of the enemy types: fast and tanky.

### 6.3. Stages Types

Currently, we are thinking about having 2 stages: a tutorial level and the game in a bank universe.

### 6.4. Win/Lose Conditions

The player will win if he manages to kill all the enemies. The player will lose if he loses all his gold.

### 6.5. Rewards

The player will get rewards at the end of each level. The rewards will be gold, experience points, and some bonuses.

### 6.6. Upgrades

The player will be able to upgrade his towers. The upgrades will be: damage, range, attack speed, slow and AOE efficiency, income effect, etc.

## 7. Programming

<!-- Specifications for programming features such as scripts, modules, plugins, programming languages, libraries, etc. -->
### 7.1 Programming Languages

- **Blueprints** is the main programming language used in the project.
- **C++** is the secondary programming language used in the project.

#### Why did we choose Blueprints?

<!-- Why did we choose Blueprints? -->

We chose Blueprints because it is a very powerful programming language. It is very easy to use and it is very easy to learn. By using Unreal Engine 4 and Blueprints, we are able to create a working game in a very short time.

### 7.2 Software

- **Unreal Engine 4** is the main game engine used in the project. (Version 4.27)
- **Visual Studio 2019** is the main IDE used in the project.

#### Why did we choose Unreal Engine 4?

<!-- Why did we choose Unreal Engine 4? -->

We chose Unreal Engine 4 because it is a very powerful game engine. It is very easy to use and it is very easy to learn. The blueprints system help us a lot to create a game. With this game engine, we are able to create a working game with the short delay we have.s

## 8. Testing and Debugging

<!-- Specifications for quality and performance testing, test scenarios, debugging tools, bug reports, etc. -->

The game will be tested by our QA. The QA will test the game and report bugs. The QA will also test the game's performance and report any performance issues.

## 9. Deployment Distribution Services

<!-- Specifications for deployment platforms such as Steam, Google Play, Apple Store, etc. -->

At the moment, we are not sure about the deployment distribution service we will use. We will decide later. We were thinking about using Steam but the cost to publish a game on Steam is quite high for us, and the delay to publish a game on Steam is also quite long.

## 10. Glossary

| **Name** | **Abrevation** | **Definition** |
|:--------:|:--------------:|:--------------:|
| 2D isometric | 2D iso | [2D isometric](https://en.wikipedia.org/wiki/Isometric_graphics) is a 2D projection of a 3D scene onto a plane. |
| Area Of Effect | AOE | [Area of Effect](https://en.wikipedia.org/wiki/Glossary_of_video_game_terms#area_of_effect), commonly abbreviated as "AoE", refers to the range of an ability or attack that affects multiple targets within a specific area, rather than a single target. |
| Blueprints | BP | [Blueprints](https://docs.unrealengine.com/en-US/Engine/Blueprints/index.html) are visual scripting tools that allow you to create logic for your game without writing code. |
| C++ | C++ | [C++](https://en.wikipedia.org/wiki/C%2B%2B) is a general-purpose programming language created by Bjarne Stroustrup as an extension of the C programming language, or "C with Classes". |
| Steam | Steam | [Steam](https://store.steampowered.com/) is a digital distribution platform developed by Valve Corporation, which offers digital rights management (DRM), multiplayer gaming, video streaming and social networking services. |
| Tower Defense | TD | [Tower Defense](https://en.wikipedia.org/wiki/Tower_defense) is a subgenre of strategy video games in which the player must defend a particular location or path against waves of enemies by strategically placing defensive structures, such as towers or traps, along the path to defeat the enemies before they reach their destination. |
| Unreal Engine | UE | [Unreal Engine](https://www.unrealengine.com/en-US/) is a 3D computer graphics game engine developed by Epic Games. |
| Visual Studio | VS | [Visual Studio](https://visualstudio.microsoft.com/) is an integrated development environment (IDE) from Microsoft. It is used to develop computer programs, as well as websites, web apps, web services and mobile apps. Visual Studio uses Microsoft software development platforms such as Windows API, Windows Forms, Windows Presentation Foundation, Windows Store and Microsoft Silverlight. It can produce both native code and managed code. |

*All the links in this document are clickable and redirect to the source of our glossary.*
