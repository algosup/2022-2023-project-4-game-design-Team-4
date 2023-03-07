# Test Cases for the game design project with Unreal Engine

With this document, we will describe the test cases that we will use to test our game. We will describe the test cases and the expected result.

## Test the Documentation

### Objective for the documentation test

Ensure that the documentation is well-written and understandable.

### Pre-Conditions for the documentation test

Read the documentation

### Condition for the test

|Action|Expected result|
|---|---|
|Correct the grammar or vocabulary mistakes|The documentation is well written and understandable|

## Test the idle part of the game

### Objective for the idle part of the game

To ensure that is possible for the game to be in an idle state.
So continue if the player is not doing anything.

### Pre-Conditions for the idle part of the game

Create a little cookie clicker game

### Conditions for the idle part of the game

|Action|Expected result|
|---|---|---|
|Do nothing|The game continue to run and gain money|
|Quit the game|The game continue to run and gain money|

### Steps for the idle part of the game

1. Create a little cookie clicker game
2. Try to do nothing
3. Verify that the game continues to run and gain money
4. Quit the game
5. Verify that the game continues to run and gain money

## Test camera

### Objective for the camera test

To ensure that the tower is working as intended.

### Pre-Conditions for the camera test

Create a camera object.
Put the camera into the scene.

### Conditions for the camera test

|Action|Expected result|
|---|---|
|Move the mouse wheel upwards|Zoom in|
|Move the mouse wheel downwards|Zoom out|

### Steps for the camera test

1. Put the camera into the scene
2. Code in C++ to zoom in on the camera
3. Code in C++ to zoom out the camera
4. Verify that the output for the zoom-in is as expected
5. Verify that the output for the zoom-out is as expected

## Enemies Test

### Objective for the enemies test

To ensure that the enemy they are different depending on their class(different life, different movement speed, and different aspect). Also, enemies can move, receive damage and die.
Also, ensure that the enemy can collect gold from the base of the player.

### Pre-Conditions for the enemies test

Create the different enemies.
Create the path.

### Conditions for the enemies test

|Action|Expected result|
|---|---|
|Launch the wave|the enemies arrived|
|When the enemies arrived they follow the path created|The enemies follow the path|
|the enemies arrived with life|The enemies arrived with the correct life|
|the enemies arrived with move speed|The enemies arrived with the correct move speed|
|The turret attack the enemies|The enemies lose life|
|When the enemies lose all their life|The enemies die|
|When the enemies die|The enemies are not in the scene|
|The enemies arrive at the base of the player|The enemies collect gold|

### Steps for the enemies test

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

## Tower Test

### Objective for the tower test

To ensure that the different towers can shoot except for the income tower and the tower can be upgraded.

### Pre-Conditions for the tower test

Create the different towers

### Conditions for the tower test

|Action|Expected result|
|---|---|
|Drag and drop on the correct zone to place the tower|Create the tower|
|When the players have enough money|The tower is build|
|When the players have not enough money|The tower is not build|
|When the tower is build|The tower can be upgraded|
|When the tower is upgraded|The tower can be upgraded again|
|When the players click to sell the tower|The tower is sold|
|When the tower is sold|The tower is not in the scene|
|When the tower is sold|The players collect the money divided by 2 of the tower|
|When the tower is sold|The tower can be build again|
|When an enemies is in the range of a turret|Turret target the first enemy|
|When an enemies is target|Turret turn to the enemy|
|When an enemies is target|Turret shoot at the enemy|
|When the turret shoot at the enemy|The enemy lose life|

### Steps for the tower test

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

## Money Test

### Objective for the money test

To ensure that the player can collect money from the enemies or when he sells a tower.

### Pre-Conditions for the money test

Create the enemies
Create the different towers

### Conditions for the money test

|Action|Expected result|
|---|---|
|When the enemies is kill|The player collect money|
|When the tower is sold|The player collect money|
|When the tower is upgraded|The player lose money|
|When the tower is build|The player lose money|

### Steps for the money test

1. Create the different enemies in the scene
2. Create the different towers in the scene
3. Create a different path in the scene
4. Launch the wave
5. Verify that the player collect money when the enemy is killed
6. Verify that the player collect money when the tower is sold
7. Verify that the player loses money when the tower is upgraded
8. Verify that the player loses money when the tower is built

## Achievement Test

### Objective for the achievement test

To ensure that the player can unlock the achievement when he reaches a certain amount of money or a certain wave.

### Pre-Conditions for the achievement test

Create the different enemies

### Conditions for the achievement test

|Action|Expected result|
|---|---|
|When the player reach a certain wave|The player unlock an achievement|
|When the player reach a certain amount of money|The player unlock an achievement|
|When the player unlock an achievement|The player can see the achievement in the achievement menu|
|Create the different enemies|When the player reach kill a certain enemy|The player unlock an achievement|

### Steps for the achievement test

1. Create the different enemies in the scene
2. Create the different towers in the scene
3. Create a different path in the scene
4. Launch the wave
5. Verify that the player unlocks an achievement when the player reaches a certain wave
6. Verify that the player unlocks an achievement when the player reaches a certain amount of money
7. Verify that the player can see the achievement in the achievement menu when the player unlocks an achievement
8. Verify that the player unlocks an achievement when the player reaches kill a certain enemy

## Player stat Test

### Objective for the player stat test

To ensure that the player can see his stat in the menu.

### Pre-Conditions for the player stat test

Create the stat menu

### Conditions for the player stat test

|Action|Expected result|
|---|---|
|When the player click on the stat menu|The player can see his stat|
|When the player click on his stat|The player see the total of enemies kill|
|When the player click on his stat|The player see the total of boss kill|
|When the player click on his stat|The player see the total of money collect|
|When the player click on his stat|The player see the total of special enemies kill|
|When the player click on his stat|The player see the total of wave reach|
|When the player click on his stat|The player see the maximum of wave reach|

### Steps for the player stat test

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

## Bestiary Test

### Objective for the bestiary test

To ensure that the player can see the different enemies in the bestiary.

### Pre-Conditions for the bestiary test

Create the bestiary menu

### Conditions for the bestiary test

|Pre-conditions|Action|Expected result|
|---|---|---|
|------------|When the player click on the bestiary menu|The player can see the different enemies encounter|
|------------|When the player click on the bestiary menu|The player can see the different boss encounter|
|------------|When the player click on the bestiary menu|The player can see the different special enemies encounter|

### Steps for the bestiary test

1. Create the different enemies in the scene
2. Create the different towers in the scene
3. Create a different path in the scene
4. Launch the wave
5. Verify that the player can see the different enemies encounter when the player clicks on the bestiary menu.
6. Verify that the player can see the different boss encounters when the player clicks on the bestiary menu.
7. Verify that the player can see the different special enemies encounter when the player clicks on the bestiary menu.

## Settings Test

### Objective for the settings test

To ensure that the player can change the settings of the game.

### Pre-Conditions for the settings test

Create the settings

### Conditions for the settings test

|Action|Expected result|
|---|---|
|When the player click on the settings menu|The player can change the volume of the game|
|When the player click on the settings menu|The player can change the resolution of the game|

### Steps for the settings test

1. Create a Settings menu
2. Verify that the player can change the volume of the game when the player clicks on the settings menu
3. Verify that the player can change the resolution of the game when the player clicks on the settings menu

## Pause Test

### Objective for the pause test

To ensure that the player can pause the game.

### Pre-Conditions for the pause test

Create the pause part.

### Conditions for the pause test

|Action|Expected result|
|---|---|
|When the player click on the pause button|The game is paused|

### Steps for the pause test

1. Create a pause button
2. Verify that the game is paused when the player clicks on the pause button

## Main Menu Test

### Objective for the main menu test

To ensure that the player can access the different menus of the game.

### Pre-Conditions for the main menu test

Create the main menu.

### Conditions for the main menu test

|Action|Expected result|
|---|---|
|When the player click on the play button|The player can access to the game|
|When the player click on the settings button|The player can access to the settings menu|

### Steps for the main menu test

1. Create a main menu
2. Verify that the player can access the game when the player clicks on the play button
3. Verify that the player can access the settings menu when the player clicks on the settings button

## End Game Test

### Objective for the end-game test

Ensure that the player cannot access the end-game menu because it's an infinite game.

### Pre-Conditions

Lose all your health points

|Action|Expected result|
|---|---|
|When the player reach lose game|The player cannot access to the end game menu|
|When the lose the game|The game re-launch at the previous wave|
