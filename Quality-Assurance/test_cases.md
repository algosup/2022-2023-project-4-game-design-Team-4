# Test Cases for the game design project with Unreal Engine

With this document we will describe the test cases that we will use to test our game. We will describe the test cases and the expected result.

## Test the idle part of the game

### Objective

To ensure that is possible to the game to be in idle state.
So continue if the player is not doing anything.

|Pre-conditions|Action|Expected result|
|---|---|---|
|Create a little cookie clicker game|Do nothing|The game continue to run and gain money|
|Create a little cookie clicker game|Quit the game|The game continue to run and gain money|

### Steps for the idle part of the game

1. Create a little cookie clicker game
2. Try to do nothing
3. Verify that the game continue to run and gain money
4. Quit the game
5. Verify that the game continue to run and gain money

## Test camera

### Objective for the camera test

To ensure that the tower is working as intended.

|Pre-conditions|Action|Expected result|
|---|---|---|
|Put the camera into the scene|Move the mouse wheel upwards|Zoom in|
|Put the camera into the scene|Move the mouse wheel downwards|Zoom out|

### Steps for the camera test

1. Put the camera into the scene
2. Code in C++ to zoom in the camera
3. Code in C++ to zoom out the camera
4. Verify that the output for the zoom in is as expected
5. Verify that the output for the zoom out is as expected

## Enemies Test

### Objective for the enemies test

To ensure that the enemy they are different depending on their class(different life,different move speed and different aspect).Also enemies can move, receive damage and die.
Also to ensure that the enemy can recolt gold from the base of the player.

|Pre-conditions|Action|Expected result|
|---|---|---|
|Create the different enemies|Launch the wave|the enemies arrived|
|Create the path|When the enemies arrived they follow the path created|The enemies follow the path|
|Create the different enemies|the enemies arrived with life|The enemies arrived with the correct life|
|Create the different enemies|the enemies arrived with move speed|The enemies arrived with the correct move speed|
|Create the different enemies|The turret attack the enemies|The enemies lose life|
|Create the different enemies|When the enemies lose all their life|The enemies die|
|Create the different enemies|When the enemies die|The enemies are not in the scene|
|Create the different enemies|The enemies arrive at the base of the player|The enemies recolt gold|

### Steps for the enemies test

1. Create the enemies in the scene
2. Create a map with a path in the scene
3. Launch the wave
4. Verify that the enemies arrived
5. Verify that the enemies follow the path
6. Verify that the enemies arrived with the correct life
7. Verify that the enemies arrived with the correct move speed
8. Verify that the enemies lose life when the turret attack them
9. Verify that the enemies recolt gold when they arrive at the base of the player
10. Verify that the enemies die when they lose all their life
11. Verify that the enemies are not in the scene when they die

## Tower Test

### Objective for the tower test

To ensure that the different tower can shoot except for the income tower and the tower can be upgraded.

|Pre-conditions|Action|Expected result|
|---|---|---|
|Create the different towers|drag and drop on the correct zone to place the tower|Create the tower|
|Create the different towers|When the players have enough money|The tower is build|
|Create the different towers|When the players have not enough money|The tower is not build|
|Create the different towers|When the tower is build|The tower can be upgraded|
|Create the different towers|When the tower is upgraded|The tower can be upgraded again|
|Create the different towers|When the players click to sell the tower|The tower is sold|
|Create the different towers|When the tower is sold|The tower is not in the scene|
|Create the different towers|When the tower is sold|The players recolt the money divided by 2 of the tower|
|Create the different towers|When the tower is sold|The tower can be build again|
|Create the different towers|When an enemies is in the range of a turret|Turret target the first enemy|
|Create the different towers|When an enemies is target|Turret turn to the enemy|
|Create the different towers|When an enemies is target|Turret shoot at the enemy|
|Create the different towers|When the turret shoot at the enemy|The enemy lose life|

### Steps for the tower test

1. Create the different towers in the scene

2. Create the different enemies in the scene

3. Create the different path in the scene

4. Launch the wave

5. Verify that the tower is build when the players have enough money

6. Verify that the tower is not build when the players have not enough money

7. Verify that the tower is not build when it is not in the correct zone

8. Verify that the tower is not build when it is already build in the same zone

9. Verify that the tower can be upgraded when the tower is build

10. Verify that the tower can be upgraded again when the tower is upgraded

11. Verify that the tower is sold when the players click to sell the tower

12. Verify that the tower is not in the scene when the tower is sold

13. Verify that the players recolt the money divided by 2 of the tower when the tower is sold

14. Verify that the tower can be build again when the tower is sold

15. Verify that the turret target the first enemy when an enemies is in the range of a turret

16. Verify that the turret turn to the enemy when an enemies is target

17. Verify that the turret shoot at the enemy when an enemies is target

18. Verify that the turret have a cooldown between each shot depending on the type of the turret

19. Verify that the enemy lose life when the turret shoot at the enemy depending on the type of the turret

20. Verify that the turret can shoot multiple enemies at the same time depending on the type of the turret

21. Verify that the turret can slow the enemies depending on the type of the turret

22. Verify that the turret can burst the enemies depending on the type of the turret

23. Verify that the turret can stun the enemies depending on the type of the turret

24. Verify that the turret can earn money depending on the type of the turret

## Money Test

### Objective for the money test

To ensure that the player can recolt money from the enemies or when he sell a tower.

|Pre-conditions|Action|Expected result|
|---|---|---|
|Create the different enemies|When the enemies is kill|The player recolt money|
|Create the different towers|When the tower is sold|The player recolt money|
|Create the different towers|When the tower is upgraded|The player lose money|
|Create the different towers|When the tower is build|The player lose money|

### Steps for the money test

1. Create the different enemies in the scene
2. Create the different towers in the scene
3. Create the different path in the scene
4. Launch the wave
5. Verify that the player recolt money when the enemies is kill
6. Verify that the player recolt money when the tower is sold
7. Verify that the player lose money when the tower is upgraded
8. Verify that the player lose money when the tower is build

## Achievement Test

### Objective for the achievement test

To ensure that the player can unlock achievement when he reach a certain amount of money or a certain wave.

|Pre-conditions|Action|Expected result|
|---|---|---|
|Create the different enemies|When the player reach a certain wave|The player unlock an achievement|
|------------|When the player reach a certain amount of money|The player unlock an achievement|
|------------|When the player unlock an achievement|The player can see the achievement in the achievement menu|
|Create the different enemies|When the player reach kill a certain enemy|The player unlock an achievement|

### Steps for the achievement test

1. Create the different enemies in the scene
2. Create the different towers in the scene
3. Create the different path in the scene
4. Launch the wave
5. Verify that the player unlock an achievement when the player reach a certain wave
6. Verify that the player unlock an achievement when the player reach a certain amount of money
7. Verify that the player can see the achievement in the achievement menu when the player unlock an achievement
8. Verify that the player unlock an achievement when the player reach kill a certain enemy

## Player stat Test

### Objective for the player stat test

To ensure that the player can see his stat in the menu.

|Pre-conditions|Action|Expected result|
|---|---|---|
|------------|When the player click on the stat menu|The player can see his stat|
|------------|When the player click on his stat|The player see the total of enemies kill|
|------------|When the player click on his stat|The player see the total of boss kill|
|------------|When the player click on his stat|The player see the total of money recolt|
|------------|When the player click on his stat|The player see the total of special enemies kill|
|------------|When the player click on his stat|The player see the total of wave reach|
|------------|When the player click on his stat|The player see the maximum of wave reach|

### Steps for the player stat test

1. Create the different enemies in the scene
2. Create the different towers in the scene
3. Create the different path in the scene
4. Launch the wave
5. Verify that the player can see his stat when the player click on the stat menu
6. Verify that the player see the total of enemies kill when the player click on his stat
7. Verify that the player see the total of boss kill when the player click on his stat
8. Verify that the player see the total of money recolt when the player click on his stat
9. Verify that the player see the total of special enemies kill when the player click on his stat
10. Verify that the player see the total of wave reach when the player click on his stat.

## Bestiary Test

### Objective for the bestiary test

To ensure that the player can see the different enemies in the bestiary.

|Pre-conditions|Action|Expected result|
|---|---|---|
|------------|When the player click on the bestiary menu|The player can see the different enemies encounter|
|------------|When the player click on the bestiary menu|The player can see the different boss encounter|
|------------|When the player click on the bestiary menu|The player can see the different special enemies encounter|

### Steps for the bestiary test

1. Create the different enemies in the scene
2. Create the different towers in the scene
3. Create the different path in the scene
4. Launch the wave
5. Verify that the player can see the different enemies encounter when the player click on the bestiary menu.
6. Verify that the player can see the different boss encounter when the player click on the bestiary menu.
7. Verify that the player can see the different special enemies encounter when the player click on the bestiary menu.

## Settings Test

### Objective for the settings test

To ensure that the player can change the settings of the game.

|Pre-conditions|Action|Expected result|
|---|---|---|
|------------|When the player click on the settings menu|The player can change the volume of the game|
|------------|When the player click on the settings menu|The player can change the resolution of the game|

### Steps for the settings test

1. Create a Settings menu
2. Verify that the player can change the volume of the game when the player click on the settings menu
3. Verify that the player can change the resolution of the game when the player click on the settings menu

## Pause Test

### Objective for the pause test

To ensure that the player can pause the game.

|Pre-conditions|Action|Expected result|
|---|---|---|
|------------|When the player click on the pause button|The game is paused|

### Steps for the pause test

1. Create a pause button
2. Verify that the game is paused when the player click on the pause button

## Main Menu Test

### Objective for the main menu test

To ensure that the player can access to the different menu of the game.

|Pre-conditions|Action|Expected result|
|---|---|---|
|------------|When the player click on the play button|The player can access to the game|
|------------|When the player click on the settings button|The player can access to the settings menu|

## End Game Test

### Objective for the end game test

To ensure that the player cannot access to the end game menu because it's an infinite game.

|Pre-conditions|Action|Expected result|
|---|---|---|
|------------|When the player reach lose game|The player cannot access to the end game menu|
|------------|When the lose the game|The game re-launch in the previous wave|
