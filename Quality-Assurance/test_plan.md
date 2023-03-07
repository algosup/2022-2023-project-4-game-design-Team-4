# Test plan for game design project

## Introduction

This document is the test plan for this project. This document will list all the tests made on the project, when they were made and if they were successfull or not.

Author: [Robin DEBRY](https://github.com/robin-debry)

<details>

<summary> Table of content </summary>

- [Test plan for game design project](#test-plan-for-game-design-project)
  - [Introduction](#introduction)
  - [1 Resources](#1-resources)
    - [1.1 Team: The team will consist of the following members](#11-team-the-team-will-consist-of-the-following-members)
    - [1.2 Tools: The tools used for the project will be](#12-tools-the-tools-used-for-the-project-will-be)
      - [1.2.1 Hardware](#121-hardware)
      - [1.2.2 Software](#122-software)
  - [2 Scope of testing](#2-scope-of-testing)
  - [3 Test Strategy](#3-test-strategy)
    - [3.1 Scope of testing](#31-scope-of-testing)
    - [3.2 Out of scope testing](#32-out-of-scope-testing)
  - [4 Test Environment](#4-test-environment)
  - [5 Primary User test](#5-primary-user-test)
    - [5.1 Define primary users](#51-define-primary-users)
    - [5.2 Example of a primary tester](#52-example-of-a-primary-tester)
  - [5 Testing](#5-testing)
  - [6 Glossary](#6-glossary)

</details>

## 1 Resources

### 1.1 Team: The team will consist of the following members

```md
- Project manager
- Program manager
- Tech lead
- Software engineer
- QA
```

The team members will contribute to reporting bugs when found.
The lead tester/QA will be responsible for insuring that the found bugs are written down and that the team is aware of them.

### 1.2 Tools: The tools used for the project will be

#### 1.2.1 Hardware

```sh
- 3 MacBook Air M1 running on macOS Monterey
- 2 Lenovo ThinkBook running on Windows 11 Pro
- 1 WhiteBoard
```

#### 1.2.2 Software

```sh
- Visual Studio Comunity 2022
- Github
- Unreal Engine
- C++
```

## 2 Scope of testing

The goal of the project is to create a game in C++. We will use Unreal Engine to create the game. For the test part we need to test each case of the game to be sure that the game is working as intended.
All the test provided should pass and the game should be playable.

## 3 Test Strategy

### 3.1 Scope of testing

The first step will be to pass the tests of documentation. After that I need to test the basics of the game so if the enemies follow the good way or not. Also the shooting of the tower. Then we will test the part more specific of the game like the movement of the tower and the part of the game where the tower can be upgraded, and the part where the base can be destroyed.

Then, we will use our test to check if the game is what we expected. We will also test the game with other people to see if they can play it without any problem.

Then we will test the part of the game like the part where the ennemies can be upgraded and destroyed. Also test the part to know if the game is over or not.

The last part of the game will be the part where the game is saved and loaded. We will test if the game is saved and loaded correctly.

### 3.2 Out of scope testing

The out of scope testing will be the part of the game that is not implemented yet. We will not test the part of the game in each platform because we don't have the time to do it.

The last part of the game will be the part where the game is saved and loaded. We will test if the game is saved and loaded correctly.

## 4 Test Environment

All the test are going to be run on Mac M1 with the M1 chip directly on the game. We will also test the game on a Windows computer with the same version of the game.

## 5 Primary User test

### 5.1 Define primary users

To make sure that something is working, there is nothing better than multiple testers.
As FABGen is an open source repository, outside developers will be asked to test it and give their feedback. They will be asked to test the installation and the usage of the bindings. They will be asked to test the examples. We will call them Primary Users.

The Primary users are developers that create bindings in Rust. They are supposed to be familiar with Rust and/or Python as well as to be able to use the bindings without any help.
They are expected to pass all phases of the usage easily :

- Installation
  - Github repository download
  - Installation of Unreal Engine
  - Execution of the project
- Usage
  - Build the project
  - Run the project

### 5.2 Example of a primary tester

```md
  - Name: Johnny Marson
  - Age: 35 years old
  - Education: Master's degree in History of Art
  - Experience in gaming : 10 years of experience in gaming  
  - Job: Teacher (Senior)
  - Why ? : He love to play games especially tower defense games. He want a new game to play.
  - Acceptance criteria : He is able to install the game and play it without any problem.
```

```md
  - Name: Christina Smith
  - Age: 15 years old
  - Education: High School
  - Experience in gaming: 2 years of experience in gaming
  - Job: Student (Junior)
  - Why ? : She plays occasionally to games and she doesn't know a lot of games. She wants to play a new game.
  - Acceptance criteria : She is able to install the game and play it during a little period of time per day.
```

```md
  - Name: Thomas Anderson
  - Age: 23
  - Education: Bachelor's degree in Computer Science
  - Experience: Never played a game
  - Job: Software Engineer (Junior)
  - Why ? : He never played a game and he wants to try it.
  - Acceptance criteria : He need a tutorial to know how to play the game.
```

## 5 Testing

To test our game we will use the test plan and the test cases. We will use the test plan to know what we need to test and the test cases to know how we will test it.

## 6 Glossary

- **Unreal Engine:** Unreal Engine is a proprietary video game engine developed by Epic Games.
- **Epic Games:** Epic Games is an American video game and software developer.
- **C++:** C++ is a general-purpose programming language created by Bjarne Stroustrup as an extension of the C programming language, or "C with Classes".
- **Github:** GitHub is a web-based hosting service for version control using Git.
- **Visual Studio:** Visual Studio is an integrated development environment (IDE) from Microsoft.
