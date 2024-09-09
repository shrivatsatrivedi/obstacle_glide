Simple Canvas Game - README
Overview
This is a simple browser-based game built using JavaScript and HTML5's canvas element. The objective is to control a game piece, keeping it in the air using gravity and acceleration, while avoiding randomly generated obstacles. The game also tracks your score based on how long you survive.

Features
Game Piece Control: The game piece is represented by an image (Sman.png) and is affected by gravity. The player can control the piece's movement by using the UP button to apply negative gravity and make it move upwards.
Obstacles: Obstacles appear randomly from the right side of the canvas and move to the left. They vary in height and gaps, making it progressively harder to avoid collisions.
Scoring: The score increases based on the number of frames survived.
Gravity: The game piece is affected by gravity, which gradually pulls it down. The UP button temporarily reduces gravity to keep the piece in the air.
How to Play
Press and hold the UP button to make the game piece move upward and avoid obstacles.
The game piece will be pulled down by gravity when the button is not pressed.
Obstacles will appear from the right side of the screen, and you must avoid crashing into them.
Your score increases the longer you stay alive.
Controls:

UP Button: Hold to accelerate upwards.
Rotate Button: (Not fully implemented) Attempts to rotate the canvas or the game piece.
Game Elements
Game Piece: An image (Sman.png) that the player controls. It moves according to gravity and player input.
Obstacles: These are colored blocks that randomly appear on the canvas and move towards the game piece from the right. They differ in height and gaps.
Score: Displayed in the top right corner, showing how long you've survived.
Code Structure
HTML
The HTML file contains a <canvas> element where the game is rendered, and two buttons to control the game piece's movement.
The background image for the canvas is a parallax mountain animation.
JavaScript
Game Area: The game area is initialized by creating a canvas element where the game is drawn. It updates every 20 milliseconds, creating the illusion of movement.
Component Class: A component class is used to represent various objects in the game (the player-controlled piece, obstacles, and text elements).
Attributes: width, height, color (or image), position (x, y), and speed (speedX, speedY).
Gravity: The game piece has a gravity attribute that pulls it down unless overridden by player input.
Collision Detection: The game detects when the player crashes into an obstacle.
Obstacles: Randomly generated obstacles appear at regular intervals and move towards the left side of the canvas.
Game Loop: The updateGameArea() function continuously updates the game state, moving obstacles, checking for collisions, and adjusting the position of the game piece based on player input.
Controls
Gravity Control: The accelerate() function is triggered when the UP button is pressed or released. It changes the gravity applied to the game piece.
Rotate Function: A partial implementation exists to rotate the canvas or game piece, though it's not fully functional.
Score
The score is displayed in the top right corner and increases based on the number of frames passed.
How to Run
Clone/Download: Clone or download the HTML file.
Open in Browser: Open the HTML file in a modern web browser that supports HTML5 and JavaScript.
Start Playing: The game will start automatically when the page loads. Press and hold the UP button to control the game piece.
Potential Improvements
Rotate Functionality: Fully implement rotation of the game piece or canvas.
Sound Effects: Add sound effects for actions like collisions or scoring.
High Scores: Implement a high-score tracking system.
Mobile Support: Add touch controls for better gameplay on mobile devices.
License
This project is open-source and can be used or modified freely. No specific license applies.
