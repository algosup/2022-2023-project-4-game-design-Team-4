# Test Cases for the game design project with Unreal Engine

With this document, we will describe the test cases that we will use to test our game. We will describe the test cases and the expected result. We will also describe the pre-conditions and the conditions for the test.

<details>
<summary> Table of content </summary>

- [Test Cases for the game design project with Unreal Engine](#test-cases-for-the-game-design-project-with-unreal-engine)
  - [1.Test the Documentation](#1test-the-documentation)
    - [1.1.Objective for the documentation test](#11objective-for-the-documentation-test)
    - [1.2.Pre-Conditions for the documentation test](#12pre-conditions-for-the-documentation-test)
    - [1.3.Condition for the test](#13condition-for-the-test)
    - [1.4.Steps for the documentation test](#14steps-for-the-documentation-test)
  - [2.Test the idle part of the game](#2test-the-idle-part-of-the-game)
    - [2.1.Objective for the idle part of the game](#21objective-for-the-idle-part-of-the-game)
    - [2.2.Pre-Conditions for the idle part of the game](#22pre-conditions-for-the-idle-part-of-the-game)
    - [2.3.Conditions for the idle part of the game](#23conditions-for-the-idle-part-of-the-game)
    - [2.4.Steps for the idle part of the game](#24steps-for-the-idle-part-of-the-game)
  - [3.Test camera](#3test-camera)
    - [3.1.Objective for the camera test](#31objective-for-the-camera-test)
    - [3.2.Pre-Conditions for the camera test](#32pre-conditions-for-the-camera-test)
    - [3.3.Conditions for the camera test](#33conditions-for-the-camera-test)
    - [3.4.Steps for the camera test](#34steps-for-the-camera-test)
  - [4.Enemies Test](#4enemies-test)
    - [4.1.Objective for the enemies test](#41objective-for-the-enemies-test)
    - [4.2.Pre-Conditions for the enemies test](#42pre-conditions-for-the-enemies-test)
    - [4.3.Conditions for the enemies test](#43conditions-for-the-enemies-test)
    - [4.4.Steps for the enemies test](#44steps-for-the-enemies-test)
  - [5.Tower Test](#5tower-test)
    - [5.1.Objective for the tower test](#51objective-for-the-tower-test)
    - [5.2.Pre-Conditions for the tower test](#52pre-conditions-for-the-tower-test)
    - [5.3.Conditions for the tower test](#53conditions-for-the-tower-test)
    - [5.4.Steps for the tower test](#54steps-for-the-tower-test)
  - [6.Money Test](#6money-test)
    - [6.1.Objective for the money test](#61objective-for-the-money-test)
    - [6.2.Pre-Conditions for the money test](#62pre-conditions-for-the-money-test)
    - [6.3.Conditions for the money test](#63conditions-for-the-money-test)
    - [6.4.Steps for the money test](#64steps-for-the-money-test)
  - [7.Achievement Test](#7achievement-test)
    - [7.1.Objective for the achievement test](#71objective-for-the-achievement-test)
    - [7.2.Pre-Conditions for the achievement test](#72pre-conditions-for-the-achievement-test)
    - [7.3.Conditions for the achievement test](#73conditions-for-the-achievement-test)
    - [7.4.Steps for the achievement test](#74steps-for-the-achievement-test)
  - [8.Player stat Test](#8player-stat-test)
    - [8.1.Objective for the player stat test](#81objective-for-the-player-stat-test)
    - [8.2.Pre-Conditions for the player stat test](#82pre-conditions-for-the-player-stat-test)
    - [8.3.Conditions for the player stat test](#83conditions-for-the-player-stat-test)
    - [8.4.Steps for the player stat test](#84steps-for-the-player-stat-test)
  - [9.Bestiary Test](#9bestiary-test)
    - [9.1.Objective for the bestiary test](#91objective-for-the-bestiary-test)
    - [9.2.Pre-Conditions for the bestiary test](#92pre-conditions-for-the-bestiary-test)
    - [9.3.Conditions for the bestiary test](#93conditions-for-the-bestiary-test)
    - [9.4.Steps for the bestiary test](#94steps-for-the-bestiary-test)
  - [10.Settings Test](#10settings-test)
    - [10.1.Objective for the settings test](#101objective-for-the-settings-test)
    - [10.2.Pre-Conditions for the settings test](#102pre-conditions-for-the-settings-test)
    - [10.3.Conditions for the settings test](#103conditions-for-the-settings-test)
    - [10.4.Steps for the settings test](#104steps-for-the-settings-test)
  - [11.Pause Test](#11pause-test)
    - [11.1.Objective for the pause test](#111objective-for-the-pause-test)
    - [11.2.Pre-Conditions for the pause test](#112pre-conditions-for-the-pause-test)
    - [11.3.Conditions for the pause test](#113conditions-for-the-pause-test)
    - [11.4.Steps for the pause test](#114steps-for-the-pause-test)
  - [12.Main Menu Test](#12main-menu-test)
    - [12.1.Objective for the main menu test](#121objective-for-the-main-menu-test)
    - [12.2.Pre-Conditions for the main menu test](#122pre-conditions-for-the-main-menu-test)
    - [12.3.Conditions for the main menu test](#123conditions-for-the-main-menu-test)
    - [12.4.Steps for the main menu test](#124steps-for-the-main-menu-test)
  - [13.Tutorial Test](#13tutorial-test)
    - [13.1.Objective for the tutorial test](#131objective-for-the-tutorial-test)
    - [13.2.Pre-Conditions for the tutorial test](#132pre-conditions-for-the-tutorial-test)
    - [13.3.Conditions for the tutorial test](#133conditions-for-the-tutorial-test)
    - [13.4.Steps for the tutorial test](#134steps-for-the-tutorial-test)
  - [14.Audio test](#14audio-test)
    - [14.1.Objective for the audio test](#141objective-for-the-audio-test)
    - [14.2.Pre-Conditions for the audio test](#142pre-conditions-for-the-audio-test)
    - [14.3.Conditions for the audio test](#143conditions-for-the-audio-test)
    - [14.4.Steps for the audio test](#144steps-for-the-audio-test)
  - [15.Performance Test](#15performance-test)
    - [15.1.Objective for the performance test](#151objective-for-the-performance-test)
    - [15.2.Pre-Conditions for the performance test](#152pre-conditions-for-the-performance-test)
    - [15.3.Conditions for the performance test](#153conditions-for-the-performance-test)
    - [15.4.Steps for the performance test](#154steps-for-the-performance-test)
  - [16.Prestige Test](#16prestige-test)
    - [16.1.Objective for the prestige test](#161objective-for-the-prestige-test)
    - [16.2.Pre-Conditions for the prestige test](#162pre-conditions-for-the-prestige-test)
    - [16.3.Conditions for the prestige test](#163conditions-for-the-prestige-test)
    - [16.4.Steps for the prestige test](#164steps-for-the-prestige-test)
  - [17.Tree of skills Test](#17tree-of-skills-test)
    - [17.1.Objective for the tree of skills test](#171objective-for-the-tree-of-skills-test)
    - [17.2.Pre-Conditions for the tree of skills test](#172pre-conditions-for-the-tree-of-skills-test)
    - [17.3.Conditions for the tree of skills test](#173conditions-for-the-tree-of-skills-test)
    - [17.4.Steps for the tree of skills test](#174steps-for-the-tree-of-skills-test)
  - [18.End Game Test](#18end-game-test)
    - [18.1.Objective for the end-game test](#181objective-for-the-end-game-test)
    - [18.2.Pre-Conditions for the end-game test](#182pre-conditions-for-the-end-game-test)
    - [18.3.Conditions for the end-game test](#183conditions-for-the-end-game-test)
    - [18.4.Steps for the end-game test](#184steps-for-the-end-game-test)

</details>

## 1.Test the Documentation

### 1.1.Objective for the documentation test

Ensure that the documentation is well-written and understandable.

### 1.2.Pre-Conditions for the documentation test

Read the documentation

### 1.3.Condition for the test

|ID|Action|Expected result|Pass/Fail|
|---|---|---|---|
|1|Correct the grammar or vocabulary mistakes|The documentation is well written and understandable|Fail|

### 1.4.Steps for the documentation test

1. Read the documentation
2. Correct the grammar or vocabulary mistakes
3. Verify that the documentation is well written and understandable

## 2.Test the idle part of the game

### 2.1.Objective for the idle part of the game

To ensure that is possible for the game to be in an idle state.
So continue if the player is not doing anything.

### 2.2.Pre-Conditions for the idle part of the game

Create a little cookie clicker game

### 2.3.Conditions for the idle part of the game

|ID|Action|Expected result|Pass/Fail|
|---|---|---|---|
|2|Do nothing|The game continue to run and gain money|Fail|
|3|Quit the game|The game continue to run and gain money|Fail|

### 2.4.Steps for the idle part of the game

1. Create a little cookie clicker game
2. Try to do nothing
3. Verify that the game continues to run and gain money
4. Quit the game
5. Verify that the game continues to run and gain money

## 3.Test camera

### 3.1.Objective for the camera test

To ensure that the tower is working as intended.

### 3.2.Pre-Conditions for the camera test

Create a camera object.
Put the camera into the scene.

### 3.3.Conditions for the camera test

|ID|Action|Expected result|Pass/Fail|
|---|---|---|---|
|4|Nothing|Camera stay at is place|Pass|

### 3.4.Steps for the camera test

1. Put the camera into the scene
2. Code in C++ to zoom in on the camera
3. Code in C++ to zoom out the camera
4. Verify that the output for the zoom-in is as expected
5. Verify that the output for the zoom-out is as expected

## 4.Enemies Test

### 4.1.Objective for the enemies test

To ensure that the enemy they are different depending on their class(different life, different movement speed, and different aspect). Also, enemies can move, receive damage and die.
Also, ensure that the enemy can collect gold from the base of the player.

### 4.2.Pre-Conditions for the enemies test

Create the different enemies.
Create the path.

### 4.3.Conditions for the enemies test

|ID|Action|Expected result|Pass/Fail|
|---|---|---|---|
|5|Launch the wave|the enemies arrived|Fail|
|6|When the enemies arrived they follow the path created|The enemies follow the path|Fail|
|7|the enemies arrived with life|The enemies arrived with the correct life|Fail|
|8|the enemies arrived with move speed|The enemies arrived with the correct move speed|Fail|
|9|The turret attack the enemies|The enemies lose life|Fail|
|10|When the enemies lose all their life|The enemies die|Fail|
|11|When the enemies die|The enemies are not in the scene|Fail|
|12|The enemies arrive at the base of the player|The enemies collect gold|Fail|

### 4.4.Steps for the enemies test

1. Create the enemies in the scene
2. Create a map with a path in the scene
3. Launch the wave
4. Verify that the enemies arrived
5. Verify that the enemies follow the path
6. Verify that the enemies arrived with the correct life
7. Verify that the enemies arrived with the correct moving speed
8. Verify that the enemies lose life when the turret attacks them
9. Verify that the enemies collect gold when they arrive at the base of the player
10. Verify that the enemies die when they lose all their life
11. Verify that the enemies are not in the scene when they die

## 5.Tower Test

### 5.1.Objective for the tower test

To ensure that the different towers can shoot except for the income tower and the tower can be upgraded.

### 5.2.Pre-Conditions for the tower test

Create the different towers

### 5.3.Conditions for the tower test

ID|Action|Expected result|Pass/Fail|
|---|---|---|---|
|13|Drag and drop on the correct zone to place the tower|Create the tower|Fail|
|14|When the players have enough money|The tower is build|Fail|
|15|When the players have not enough money|The tower is not build|Fail|
|16|When the tower is build|The tower can be upgraded|Fail|
|17|When the tower is upgraded|The tower can be upgraded again|Fail|
|18|When the players click to sell the tower|The tower is sold|Fail|
|19|When the tower is sold|The tower is not in the scene|Fail|
|20|When the tower is sold|The players collect the money divided by 2 of the tower|Fail|
|21|When the tower is sold|The tower can be build again|Fail|
|22|When an enemies is in the range of a turret|Turret target the first enemy|Fail|
|23|When an enemies is target|Turret turn to the enemy|Fail|
|24|When an enemies is target|Turret shoot at the enemy|Fail|
|25|When the turret shoot at the enemy|The enemy lose life|Fail|

### 5.4.Steps for the tower test

1. Create the different towers in the scene
2. Create different enemies in the scene
3. Create a different path in the scene
4. Launch the wave
5. Verify that the tower is built when the players have enough money
6. Verify that the tower is not built when the players do have not enough money
7. Verify that the tower is not built when it is not in the correct zone
8. Verify that the tower is not built when it is already built in the same zone
9. Verify that the tower can be upgraded when the tower is build
10. Verify that the tower can be upgraded again when the tower is upgraded
11. Verify that the tower is sold when the players click to sell the tower
12. Verify that the tower is not in the scene when the tower is sold
13. Verify that the players collect the money divided by 2 of the tower when the tower is sold
14. Verify that the tower can be built again when the tower is sold
15. Verify that the turret target the first enemy when an enemy is in the range of a turret
16. Verify that the turret turns to the enemy when an enemy is Target
17. Verify that the turret shoots at the enemy when an enemy is Target
18. Verify that the turret has a cooldown between each shot depending on the type of the turret
19. Verify that the enemy loses life when the turret shoot at the enemy depending on the type of the turret
20. Verify that the turret can shoot multiple enemies at the same time depending on the type of the turret
21. Verify that the turret can slow the enemies depending on the type of the turret
22. Verify that the turret can burst the enemies depending on the type of the turret
23. Verify that the turret can stun the enemies depending on the type of the turret
24. Verify that the turret can earn money depending on the type of the turret

## 6.Money Test

### 6.1.Objective for the money test

To ensure that the player can collect money from the enemies or when he sells a tower.

### 6.2.Pre-Conditions for the money test

Create the enemies
Create the different towers

### 6.3.Conditions for the money test

|ID|Action|Expected result|Pass/Fail|
|---|---|---|---|
|26|When the enemies is kill|The player collect money|Fail|
|27|When the tower is sold|The player collect money|Fail|
|28|When the tower is upgraded|The player lose money|Fail|
|29|When the tower is build|The player lose money|Fail|

### 6.4.Steps for the money test

1. Create the different enemies in the scene
2. Create the different towers in the scene
3. Create a different path in the scene
4. Launch the wave
5. Verify that the player collect money when the enemy is killed
6. Verify that the player collect money when the tower is sold
7. Verify that the player loses money when the tower is upgraded
8. Verify that the player loses money when the tower is built

## 7.Achievement Test

### 7.1.Objective for the achievement test

To ensure that the player can unlock the achievement when he reaches a certain amount of money or a certain wave.

### 7.2.Pre-Conditions for the achievement test

Create the different enemies

### 7.3.Conditions for the achievement test

|ID|Action|Expected result|Pass/Fail|
|---|---|---|---|
|30|When the player reach a certain wave|The player unlock an achievement|Fail|
|31|When the player reach a certain amount of money|The player unlock an achievement|Fail|
|32|When the player unlock an achievement|The player can see the achievement in the achievement menu|Fail|
|33|Create the different enemies|When the player reach kill a certain enemy|The player unlock an achievement|Fail|
|34|When the make a certain prestige|The player unlock an achievement|Fail|

### 7.4.Steps for the achievement test

1. Create the different enemies in the scene
2. Create the different towers in the scene
3. Create a different path in the scene
4. Launch the wave
5. Verify that the player unlocks an achievement when the player reaches a certain wave
6. Verify that the player unlocks an achievement when the player reaches a certain amount of money
7. Verify that the player can see the achievement in the achievement menu when the player unlocks an achievement
8. Verify that the player unlocks an achievement when the player reaches kill a certain enemy
9. Verify that the player unlocks an achievement when the player makes a certain prestige

## 8.Player stat Test

### 8.1.Objective for the player stat test

To ensure that the player can see his stat in the menu.

### 8.2.Pre-Conditions for the player stat test

Create the stat menu

### 8.3.Conditions for the player stat test

|ID|Action|Expected result|Pass/Fail|
|---|---|---|---|
|35|When the player click on the stat menu|The player can see his stat|Fail|
|36|When the player click on his stat|The player see the total of enemies kill|Fail|
|37|When the player click on his stat|The player see the total of boss kill|Fail|
|38|When the player click on his stat|The player see the total of money collect|Fail|
|39|When the player click on his stat|The player see the total of special enemies kill|Fail|
|40|When the player click on his stat|The player see the total of wave reach|Fail|
|41|When the player click on his stat|The player see the maximum of wave reach|Fail|

### 8.4.Steps for the player stat test

1. Create the different enemies in the scene
2. Create the different towers in the scene
3. Create a different path in the scene
4. Launch the wave
5. Verify that the player can see his stat when the player clicks on the stat menu
6. Verify that the player sees the total of enemies killed when the player clicks on his stat
7. Verify that the player sees the total of a boss kill when the player clicks on his stat
8. Verify that the player sees the total money collect when the player clicks on his stat
9. Verify that the player sees the total of special enemies killed when the player clicks on his stat
10. Verify that the player sees the total wave reach when the player clicks on his stat.

## 9.Bestiary Test

### 9.1.Objective for the bestiary test

To ensure that the player can see the different enemies in the bestiary.

### 9.2.Pre-Conditions for the bestiary test

Create the bestiary menu

### 9.3.Conditions for the bestiary test

|ID|Action|Expected result|Pass/Fail|
|---|---|---|---|
|42|When the player click on the bestiary menu|The player can see the different enemies encounter|Fail|
|43|When the player click on the bestiary menu|The player can see the different boss encounter|Fail|
|44|When the player click on the bestiary menu|The player can see the different special enemies encounter|Fail|

### 9.4.Steps for the bestiary test

1. Create the different enemies in the scene
2. Create the different towers in the scene
3. Create a different path in the scene
4. Launch the wave
5. Verify that the player can see the different enemies encounter when the player clicks on the bestiary menu.
6. Verify that the player can see the different boss encounters when the player clicks on the bestiary menu.
7. Verify that the player can see the different special enemies encounter when the player clicks on the bestiary menu.

## 10.Settings Test

### 10.1.Objective for the settings test

To ensure that the player can change the settings of the game.

### 10.2.Pre-Conditions for the settings test

Create the settings

### 10.3.Conditions for the settings test

|ID|Action|Expected result|Pass/Fail|
|---|---|---|
|45|When the player click on the settings menu|The player can change the volume of the game|Fail|
|46|When the player click on the settings menu|The player can change the resolution of the game|Fail|

### 10.4.Steps for the settings test

1. Create a Settings menu
2. Verify that the player can change the volume of the game when the player clicks on the settings menu
3. Verify that the player can change the resolution of the game when the player clicks on the settings menu

## 11.Pause Test

### 11.1.Objective for the pause test

To ensure that the player can pause the game.

### 11.2.Pre-Conditions for the pause test

Create the pause part.

### 11.3.Conditions for the pause test

|ID|Action|Expected result|Pass/Fail|
|---|---|---|---|
|47|When the player click on the pause button|The game is paused|Fail|

### 11.4.Steps for the pause test

1. Create a pause button
2. Verify that the game is paused when the player clicks on the pause button

## 12.Main Menu Test

### 12.1.Objective for the main menu test

To ensure that the player can access the different menus of the game.

### 12.2.Pre-Conditions for the main menu test

Create the main menu.

### 12.3.Conditions for the main menu test

|ID|Action|Expected result|Pass/Fail|
|---|---|---|---|
|48|When the player click on the play button|The player can access to the game|Fail|
|49|When the player click on the settings button|The player can access to the settings menu|Fail|

### 12.4.Steps for the main menu test

1. Create a main menu
2. Verify that the player can access the game when the player clicks on the play button
3. Verify that the player can access the settings menu when the player clicks on the settings button

## 13.Tutorial Test

### 13.1.Objective for the tutorial test

To ensure that the player can access the tutorial of the game.

### 13.2.Pre-Conditions for the tutorial test

Create the tutorial.

### 13.3.Conditions for the tutorial test

|Action|Expected result|Pass/Fail|
|---|---|---|---|
|50|When the player click on the start is first game|The player directly access to the tutorial|Fail|
|51|When the player haver already a game save|The player can't access to the tutorial|Fail|

### 13.4.Steps for the tutorial test

1. Create a tutorial
2. Verify that the player directly access to the tutorial when the player clicks on the start is first game
3. Verify that the player can't access to the tutorial when the player haver already a game save

## 14.Audio test

### 14.1.Objective for the audio test

To ensure that the player can hear the different sounds of the game.

### 14.2.Pre-Conditions for the audio test

Create the different sounds of the game.
Create tower and enemies.

### 14.3.Conditions for the audio test

|ID|Action|Expected result|Pass/Fail|
|---|---|---|---|
|52|When the player click on the play button|The player can hear the sound of the game|Fail|
|53|When a wave arrived|The player can hear the sound of a bank alarm|Fail|
|54|When the player click on the pause button|The sound of the game stop|Fail|
|55|When the player click on the resume button|The sound of the game resume|Fail|

### 14.4.Steps for the audio test

1. Create the different sounds of the game
2. Create tower and enemies
3. Verify that the player can hear the sound of the game when the player clicks on the play button
4. Verify that the player can hear the sound of a bank alarm when a wave arrives
5. Verify that the sound of the game stop when the player clicks on the pause button
6. Verify that the sound of the game resume when the player clicks on the resume button

## 15.Performance Test

### 15.1.Objective for the performance test

To ensure that the game is playable on a computer with low specifications.

### 15.2.Pre-Conditions for the performance test

Create the different enemies in the scene
Create the different towers in the scene
Create a different path in the scene

### 15.3.Conditions for the performance test

|ID|Action|Expected result|Pass/Fail|
|---|---|---|---|
|56|When the player launch the game|The game is playable on a computer with low specifications|Fail|
|57|Memory usage of the game|The game doesn't crash because of the memory usage|Fail|

### 15.4.Steps for the performance test

1. Create the different enemies in the scene
2. Create the different towers in the scene
3. Create a path in the scene
4. Verify that the game is playable on a computer with low specifications when the player launch the game

## 16.Prestige Test

### 16.1.Objective for the prestige test

To ensure that the player can prestige.

### 16.2.Pre-Conditions for the prestige test

Create the prestige menu
Player arrived at certain wave to prestige

### 16.3.Conditions for the prestige test

|ID|Action|Expected result|Pass/Fail|
|---|---|---|---|
|58|When the player click on the prestige button|The player can prestige|
|59|When the player click on the prestige button|The player can see the different rewards of the prestige|

### 16.4.Steps for the prestige test

1. Create the prestige menu
2. Verify that the player can prestige when the player clicks on the prestige button
3. Verify that the player can see the different rewards of the prestige when the player clicks on the prestige button

## 17.Tree of skills Test

### 17.1.Objective for the tree of skills test

To ensure that the player can access the tree of skills.

### 17.2.Pre-Conditions for the tree of skills test

Create the tree of skills menu
Create the different skills of the tree of skills
Create the different levels of the tree of skills
Player have to have prestige points to upgrade a skill in the tree of skills

### 17.3.Conditions for the tree of skills test

|ID|Action|Expected result|Pass/Fail|
|---|---|---|---|
|60|When the player click on the tree of skills button|The player can access the tree of skills|Fail|
|61|When the player click on the tree of skills button|The player can see the different skills of the tree of skills|Fail|
|62|When the player click on the tree of skills button|The player can see the current level of the tree of skills and the level after|Fail|
|63|When the player click on the tree of skills button|The player can see the different costs of the tree of skills|Fail|
|64|When the player click on the skills into the tree of skills|The player can see the different descriptions of the tree of skills|Fail|
|65|If the player have enough prestige points|The player can upgrade a skill in the tree of skills|Fail|
|66|If the player haven't enough prestige points|The player can't upgrade a skill in the tree of skills|Fail|

### 17.4.Steps for the tree of skills test

1. Create the tree of skills menu
2. Create the different skills of the tree of skills
3. Create the different levels of the tree of skills
4. Verify that the player can access the tree of skills when the player clicks on the tree of skills button
5. Verify that the player can see the different skills of the tree of skills when the player clicks on the tree of skills button
6. Verify that the player can see the current level of the tree of skills and the level after when the player clicks on the tree of skills button
7. Verify that the player can see the different costs of the tree of skills when the player clicks on the tree of skills button
8. Verify that the player can see the different descriptions of the tree of skills when the player clicks on the skills into the tree of skills
9. Verify that the player can upgrade a skill in the tree of skills when the player have enough prestige points
10. Verify that the player can't upgrade a skill in the tree of skills when the player haven't enough prestige points

## 18.End Game Test

### 18.1.Objective for the end-game test

Ensure that the player cannot access the end-game menu because it's an infinite game.

### 18.2.Pre-Conditions for the end-game test

Lose all your health points

### 18.3.Conditions for the end-game test

|ID|Action|Expected result|Pass/Fail|
|---|---|---|---|
|67|When the player reach lose game|The player cannot access to the end game menu|Fail|
|68|When the lose the game|The game re-launch at the previous wave|Fail|

### 18.4.Steps for the end-game test

1. Lose all your health points
2. Verify that the player cannot access to the end game menu when the player reach lose game
3. Verify that the game re-launch at the previous wave when the player lose the game
