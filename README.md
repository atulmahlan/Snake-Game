# Snake Game Project
## Description:
The "Snake Game" is a classic arcade game implemented in JavaScript, where the player controls a growing snake to navigate a grid, eat food, and avoid collisions with the walls or itself. The objective is to achieve the highest possible score by consuming food, which causes the snake to grow in length and increases the game's speed.

### Functionalities:
#### Game Board and Elements:
1. The game is played on a grid defined by gridSize.
2. The snake, food, score, and high score elements are displayed on the game board.

#### Game Initialization:
1. The game initializes with a snake of length 1 at a fixed position.
2. Food is generated randomly on the grid.
3. Score and high score are tracked and displayed.

#### Game Mechanics:
1. The snake moves in the direction specified by arrow keys.
2. When the snake eats food, it grows in length, and new food is generated.
3. The game speed increases progressively as the snake eats more food.
4. The game ends if the snake collides with the walls or itself, resetting the snake and updating the high score if applicable.

#### Controls:
1. The game starts when the spacebar is pressed.
2. Arrow keys control the snake's direction.
3. Code Explanation

#### HTML Elements:
1. const board = document.getElementById("game-board");
2. const instructionText = document.getElementById("instruction-text");
3. const logo = document.getElementById("logo");
4. const score = document.getElementById("score");
5. const highScoreText = document.getElementById("highScore");

#### Game Variables:
1. const gridSize = 20;
2. let snake = [{x:10, y:10}];
3. let food = generateFood();
4. let highScore = 0;
5. let direction = "right";
6. let gameInterval;
7. let gameSpeedDelay = 200;
8. let gameStarted = false;

#### Drawing Functions:
1. draw(): Clears and redraws the game board, snake, and food.
2. drawSnake(): Draws the snake on the board.
3. drawFood(): Draws the food on the board.
4. createGameEl(tag, className): Creates a new game element (snake or food).
5. setPosition(element, position): Sets the position of an element on the grid.

#### Food Generation:
> function generateFood() { \
>    const x = Math.floor(Math.random() * gridSize) + 1; \
>    const y = Math.floor(Math.random() * gridSize) + 1; \
>    return {x, y}; \

#### Movement and Game Logic:
1. move(): Moves the snake in the current direction, checks for food collision, and increases speed if food is eaten.
2. startGame(): Starts the game, hiding instructions and logo, and setting the game interval.
3. handleKeyPress(event): Handles key presses to start the game or change the snake's direction.

#### Speed and Collision Handling:
1. increaseSpeed(): Increases the game speed based on predefined conditions.
2. checkCollision(): Checks for collisions with walls or the snake itself, resetting the game if a collision occurs.

#### Game Reset and Score Update:
1. resetGame(): Resets the game variables, snake position, and speed.
2. updateScore(): Updates the current score display.
3. stopGame(): Stops the game and shows the instructions and logo.
4. updateHighScore(): Updates and displays the high score if the current score is higher.

This project provides a fun and engaging way to learn and practice JavaScript, utilizing DOM manipulation, event handling, and basic game logic.

### Images of project:

![Screenshot 2024-08-03 045256](https://github.com/user-attachments/assets/52d5f238-9597-4ce1-afd8-6d75e6b98bfd)
![Screenshot (106)](https://github.com/user-attachments/assets/61a9843f-1676-4b2d-b9df-b2cce1024753)

