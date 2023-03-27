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
  - [2.Test camera](#2test-camera)
    - [2.1.Objective for the camera test](#21objective-for-the-camera-test)
    - [2.2.Pre-Conditions for the camera test](#22pre-conditions-for-the-camera-test)
    - [2.3.Conditions for the camera test](#23conditions-for-the-camera-test)
    - [2.4.Steps for the camera test](#24steps-for-the-camera-test)
  - [3.Enemies Test](#3enemies-test)
    - [3.1.Objective for the enemies test](#31objective-for-the-enemies-test)
    - [3.2.Pre-Conditions for the enemies test](#32pre-conditions-for-the-enemies-test)
    - [3.3.Conditions for the enemies test](#33conditions-for-the-enemies-test)
    - [3.4.Steps for the enemies test](#34steps-for-the-enemies-test)
  - [4.Tower Test](#4tower-test)
    - [4.1.Objective for the tower test](#41objective-for-the-tower-test)
    - [4.2.Pre-Conditions for the tower test](#42pre-conditions-for-the-tower-test)
    - [4.3.Conditions for the tower test](#43conditions-for-the-tower-test)
    - [4.4.Steps for the tower test](#44steps-for-the-tower-test)
  - [5.Money Test](#5money-test)
    - [5.1.Objective for the money test](#51objective-for-the-money-test)
    - [5.2.Pre-Conditions for the money test](#52pre-conditions-for-the-money-test)
    - [5.3.Conditions for the money test](#53conditions-for-the-money-test)
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
  - [9.Settings Test](#9settings-test)
    - [9.1.Objective for the settings test](#91objective-for-the-settings-test)
    - [9.2.Pre-Conditions for the settings test](#92pre-conditions-for-the-settings-test)
    - [9.3.Conditions for the settings test](#93conditions-for-the-settings-test)
    - [9.4.Steps for the settings test](#94steps-for-the-settings-test)
  - [10.Pause Test](#10pause-test)
    - [10.1.Objective for the pause test](#101objective-for-the-pause-test)
    - [10.2.Pre-Conditions for the pause test](#102pre-conditions-for-the-pause-test)
    - [10.3.Conditions for the pause test](#103conditions-for-the-pause-test)
    - [10.4.Steps for the pause test](#104steps-for-the-pause-test)
  - [11.Main Menu Test](#11main-menu-test)
    - [11.1.Objective for the main menu test](#111objective-for-the-main-menu-test)
    - [11.2.Pre-Conditions for the main menu test](#112pre-conditions-for-the-main-menu-test)
    - [11.3.Conditions for the main menu test](#113conditions-for-the-main-menu-test)
    - [11.4.Steps for the main menu test](#114steps-for-the-main-menu-test)
  - [12.Tutorial Test](#12tutorial-test)
    - [12.1.Objective for the tutorial test](#121objective-for-the-tutorial-test)
    - [12.2.Pre-Conditions for the tutorial test](#122pre-conditions-for-the-tutorial-test)
    - [12.3.Conditions for the tutorial test](#123conditions-for-the-tutorial-test)
    - [12.4.Steps for the tutorial test](#124steps-for-the-tutorial-test)
  - [13.Audio test](#13audio-test)
    - [13.1.Objective for the audio test](#131objective-for-the-audio-test)
    - [13.2.Pre-Conditions for the audio test](#132pre-conditions-for-the-audio-test)
    - [13.3.Conditions for the audio test](#133conditions-for-the-audio-test)
    - [13.4.Steps for the audio test](#134steps-for-the-audio-test)
  - [14.Performance Test](#14performance-test)
    - [14.1.Objective for the performance test](#141objective-for-the-performance-test)
    - [14.2.Pre-Conditions for the performance test](#142pre-conditions-for-the-performance-test)
    - [14.3.Conditions for the performance test](#143conditions-for-the-performance-test)
    - [14.4.Steps for the performance test](#144steps-for-the-performance-test)
  - [15 Third character test](#15-third-character-test)
    - [15.1 Objective for the third character test](#151-objective-for-the-third-character-test)
    - [15.2 Pre-Conditions for the third character test](#152-pre-conditions-for-the-third-character-test)
    - [15.3 Conditions for the third character test](#153-conditions-for-the-third-character-test)
  - [16.End Game Test](#16end-game-test)
    - [16.1.Objective for the end-game test](#161objective-for-the-end-game-test)
    - [16.2.Pre-Conditions for the end-game test](#162pre-conditions-for-the-end-game-test)
    - [16.3.Conditions for the end-game test](#163conditions-for-the-end-game-test)
    - [16.4.Steps for the end-game test](#164steps-for-the-end-game-test)

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

## 2.Test camera

### 2.1.Objective for the camera test

To ensure that the tower is working as intended.

### 2.2.Pre-Conditions for the camera test

Create a camera object.
Put the camera into the scene.

### 2.3.Conditions for the camera test

|ID|Action|Expected result|Pass/Fail|
|---|---|---|---|
|2|Nothing|Camera stay at is place|Pass|

### 2.4.Steps for the camera test

1. Put the camera into the scene
2. Code in C++ to zoom in on the camera
3. Code in C++ to zoom out the camera
4. Verify that the output for the zoom-in is as expected
5. Verify that the output for the zoom-out is as expected

## 3.Enemies Test

### 3.1.Objective for the enemies test

To ensure that the enemy they are different depending on their class(different life, different movement speed, and different aspect). Also, enemies can move, receive damage and die.
Also, ensure that the enemy can collect gold from the base of the player.

### 3.2.Pre-Conditions for the enemies test

Create the different enemies.
Create the path.

### 3.3.Conditions for the enemies test

|ID|Action|Expected result|Pass/Fail|
|---|---|---|---|
|3|Nothing begin the game|the enemies arrived|Pass|
|4|When the enemies arrived they follow the path created|The enemies follow the path|Pass|
|5|the enemies arrived with life|The enemies arrived with the correct life|Pass|
|6|the enemies arrived with move speed|The enemies arrived with the correct move speed|Pass|
|7|The turret attack the enemies|The enemies lose life|Pass|
|8|When the enemies lose all their life|The enemies die|Pass|
|9|When the enemies die|The enemies are not in the scene|Pass|
|10|When the enemies die|The enemies make an animation of death|Pass|

### 3.4.Steps for the enemies test

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
12. Verify that the enemies die with an animation

## 4.Tower Test

### 4.1.Objective for the tower test

To ensure that the different towers can shoot except for the income tower and the tower can be upgraded.

### 4.2.Pre-Conditions for the tower test

Create the different towers

### 4.3.Conditions for the tower test

ID|Action|Expected result|Pass/Fail|
|---|---|---|---|
|11|Click on a slot|Display the choice of the turret |Pass|
|12|Choose a turret|Create a turret on the slot|Pass|
|13|When the players have enough money|The tower is build|Pass|
|14|When the players have not enough money|The tower is not build|Pass|
|15|When the tower is build|The tower can be upgrade|Pass|
|16|When the tower is upgraded|The tower can be upgrade again|Pass|
|17|When the tower is upgraded twice|The tower can't be upgrade again|Pass|
|18|When the players click to sell the tower|The tower is sold|Pass|
|19|When the tower is sold|The tower is not in the scene|Pass|
|20|When the tower is sold|The players collect the money divided by 2 of the tower|Fail|
|21|When the tower is sold|The tower can be build again|Pass|
|22|When an enemies is in the range of a turret|Turret target the first enemy|Pass|
|23|When an enemies is target|Turret turn to the enemy|Pass|
|24|When an enemies is target|Turret shoot at the enemy|Pass|
|25|When the turret shoot at the enemy|The enemy lose life|Pass|
|26|When you click on the turret|Display the range of the turret|Pass|

### 4.4.Steps for the tower test

1. Create the different towers in the scene
2. Create different enemies in the scene
3. Create a different path in the scene
4. Launch the wave
5. Verify that the tower is built when the players have enough money
6. Verify that the tower is not built when the players do have not enough money
7. Verify that the tower is not built when it is not in the correct zone
8. Verify that the tower is not built when it is already built in the same zone
9. Verify that the tower can be upgrade when the tower is build
10. Verify that the tower can be upgrade again when the tower is upgrade
11. Verify that the tower upgrade twice can't be upgrade again
12. Verify that the tower is sold when the players click to sell the tower
13. Verify that the tower is not in the scene when the tower is sold
14. Verify that the players collect the money divided by 2 of the tower when the tower is sold
15. Verify that the tower can be built again when the tower is sold
16. Verify that the turret target the first enemy when an enemy is in the range of a turret
17. Verify that the turret turns to the enemy when an enemy is Target
18. Verify that the turret shoots at the enemy when an enemy is Target
19. Verify that the turret has a cooldown between each shot depending on the type of the turret
20. Verify that the enemy loses life when the turret shoot at the enemy depending on the type of the turret
21. Verify that the turret can shoot multiple enemies at the same time depending on the type of the turret
22. Verify that the turret can slow the enemies depending on the type of the turret
23. Verify that the turret can burst the enemies depending on the type of the turret
24. Verify that the turret can stun the enemies depending on the type of the turret
25. Verify that the turret can earn money depending on the type of the turret
26. Verify the range of the turret is displayed when you click on the turret

## 5.Money Test

### 5.1.Objective for the money test

To ensure that the player can collect money from the enemies or when he sells a tower.

### 5.2.Pre-Conditions for the money test

Create the enemies
Create the different towers

### 5.3.Conditions for the money test

|ID|Action|Expected result|Pass/Fail|
|---|---|---|---|
|27|When the enemies is kill|The player collect money|Pass|
|28|When the tower is sold|The player collect money|Pass|
|29|When the tower is upgrade|The player lose money|Pass|
|30|When the tower is build|The player lose money|Pass|

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
|31|When the player reach a certain wave|The player unlock an achievement|Fail|
|32|When the player reach a certain amount of money|The player unlock an achievement|Fail|
|33|When the player unlock an achievement|The player can see the achievement in the achievement menu|Fail|
|34|When the player reach kill a certain enemy|The player unlock an achievement|Fail|

### 7.4.Steps for the achievement test

1. Create the different enemies in the scene
2. Create the different towers in the scene
3. Create a different path in the scene
4. Launch the wave
5. Verify that the player unlocks an achievement when the player reaches a certain wave
6. Verify that the player unlocks an achievement when the player reaches a certain amount of money
7. Verify that the player can see the achievement in the achievement menu when the player unlocks an achievement
8. Verify that the player unlocks an achievement when the player reaches kill a certain enemy

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
|39|When the player click on his stat|The player see the total of wave reach|Fail|
|40|When the player click on his stat|The player see the maximum of wave reach|Fail|

### 8.4.Steps for the player stat test

1. Create the different enemies in the scene
2. Create the different towers in the scene
3. Create a different path in the scene
4. Launch the wave
5. Verify that the player can see his stat when the player clicks on the stat menu
6. Verify that the player sees the total of enemies killed when the player clicks on his stat
7. Verify that the player sees the total of a boss kill when the player clicks on his stat
8. Verify that the player sees the total money collect when the player clicks on his stat
9. Verify that the player sees the total wave reach when the player clicks on his stat.

## 9.Settings Test

### 9.1.Objective for the settings test

To ensure that the player can change the settings of the game.

### 9.2.Pre-Conditions for the settings test

Create the settings

### 9.3.Conditions for the settings test

|ID|Action|Expected result|Pass/Fail|
|---|---|---|
|41|When the player click on the settings button|The player can change the volume of the music in the game|Fail|
|42|When the player click on the settings butto,|The player can change the resolution of the game|Fail|

### 9.4.Steps for the settings test

1. Create a Settings menu
2. Verify that the player can change the volume of the game when the player clicks on the settings menu
3. Verify that the player can change the resolution of the game when the player clicks on the settings menu

## 10.Pause Test

### 10.1.Objective for the pause test

To ensure that the player can pause the game.

### 10.2.Pre-Conditions for the pause test

Create the pause part.

### 10.3.Conditions for the pause test

|ID|Action|Expected result|Pass/Fail|
|---|---|---|---|
|43|When the player click on the setting button|The game is paused|Fail|

### 10.4.Steps for the pause test

1. Create a pause button
2. Verify that the game is paused when the player clicks on the pause button

## 11.Main Menu Test

### 11.1.Objective for the main menu test

To ensure that the player can access the different menus of the game.

### 11.2.Pre-Conditions for the main menu test

Create the main menu.

### 11.3.Conditions for the main menu test

|ID|Action|Expected result|Pass/Fail|
|---|---|---|---|
|44|When the player click on the play button in the main menu|The player can access to the game|Pass|
|45|When the player click on the settings button in the main menu|The player can access to the settings menu|Pass|

### 11.4.Steps for the main menu test

1. Create a main menu
2. Verify that the player can access the game when the player clicks on the play button
3. Verify that the player can access the settings menu when the player clicks on the settings button

## 12.Tutorial Test

### 12.1.Objective for the tutorial test

To ensure that the player can access the tutorial of the game.

### 12.2.Pre-Conditions for the tutorial test

Create the tutorial.

### 12.3.Conditions for the tutorial test

|Action|Expected result|Pass/Fail|
|---|---|---|---|
|46|When the player click on the start is first game|The player directly show the tutorial|Pass|
|47|When the player haver already a game save|The player can't access to the tutorial|Fail|

### 12.4.Steps for the tutorial test

1. Create a tutorial
2. Verify that the player directly access to the tutorial when the player clicks on the start is first game
3. Verify that the player can't access to the tutorial when the player haver already a game save

## 13.Audio test

### 13.1.Objective for the audio test

To ensure that the player can hear the different sounds of the game.

### 13.2.Pre-Conditions for the audio test

Create the different sounds of the game.
Create tower and enemies.

### 13.3.Conditions for the audio test

|ID|Action|Expected result|Pass/Fail|
|---|---|---|---|
|48|When the player click on the play button|The player can hear the sound of the game|Fail|
|49|When a wave arrived|The player can hear the sound of a bank alarm|Fail|
|50|When the player click on the pause button|The sound of the game stop|Fail|
|51|When the player click on the resume button|The sound of the game resume|Fail|

### 13.4.Steps for the audio test

1. Create the different sounds of the game
2. Create tower and enemies
3. Verify that the player can hear the sound of the game when the player clicks on the play button
4. Verify that the player can hear the sound of a bank alarm when a wave arrives
5. Verify that the sound of the game stop when the player clicks on the pause button
6. Verify that the sound of the game resume when the player clicks on the resume button

## 14.Performance Test

### 14.1.Objective for the performance test

To ensure that the game is playable on a computer with low specifications.

### 14.2.Pre-Conditions for the performance test

Create the different enemies in the scene
Create the different towers in the scene
Create a different path in the scene

### 14.3.Conditions for the performance test

|ID|Action|Expected result|Pass/Fail|
|---|---|---|---|
|52|When the player launch the game|The game is playable on a computer with low specifications|Fail|
|53|Memory usage of the game|The game doesn't crash because of the memory usage|Fail|

### 14.4.Steps for the performance test

1. Create the different enemies in the scene
2. Create the different towers in the scene
3. Create a path in the scene
4. Verify that the game is playable on a computer with low specifications when the player launch the game

## 15 Third character test

### 15.1 Objective for the third character test

To ensure that the player can access to the third character.

### 15.2 Pre-Conditions for the third character test

Create the third character.

### 15.3 Conditions for the third character test

|ID|Action|Expected result|Pass/Fail|
|---|---|---|---|
|54|When the player reach a certain wave|The player can access to the third character|Fail|
|55|Click on the third character|The player can control the third character|Fail|
|56|When the player take the control of the third character|The player can't create towers|Fail|
|57|When the player take the control of the third character|The player can't upgrade towers|Fail|
|58|When the player take the control of the third character|The player can't sell towers|Fail|
|59|When the player take the control of the third character|The player can access to the settings menu|Fail|
|60|When the player take the control of the third character|The player can click on a touch to return on a Playable phase|Fail|

## 16.End Game Test

### 16.1.Objective for the end-game test

Ensure that the player cannot access the end-game menu because it's an infinite game.

### 16.2.Pre-Conditions for the end-game test

One enemie arrived at the end of the path.

### 16.3.Conditions for the end-game test

|ID|Action|Expected result|Pass/Fail|
|---|---|---|---|
|61|When the enemies reach the end point of the path|The player access to the end game menu|Fail|

### 16.4.Steps for the end-game test

1. Lose all your health points
2. Verify that the player cannot access to the end game menu when the player reach lose game
3. Verify that the game re-launch at the previous wave when the player lose the game
