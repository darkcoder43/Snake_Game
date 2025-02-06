# Flask Snake Game

A simple, interactive Snake game built using the Flask framework for the backend and HTML5, CSS, and JavaScript for the frontend. The game allows users to control a snake that grows as it eats food, and the player must avoid hitting walls or the snake's own body. The game keeps track of the player's score and displays it in real-time.

## Features

- **Snake Movement**: Use the arrow keys to move the snake in four directions (Up, Down, Left, Right).
- **Food**: Each time the snake eats food, it grows in length, and the score increases.
- **Collision Detection**: The game ends if the snake hits the wall or collides with itself.
- **Real-Time Score Display**: The score updates instantly as you eat food.
- **Responsive Design**: The game runs on any modern browser.

## Installation

To run the Snake game on your local machine, follow the instructions below.

### 1. Clone the Repository

Clone this repository to your local machine using `git`:

```bash
git clone https://github.com/yourusername/my_flask_snake_game.git
cd my_flask_snake_game
2. Set Up a Virtual Environment (Recommended)
It is recommended to set up a Python virtual environment to isolate the dependencies for this project:

bash
Copy
Edit
python -m venv venv
source venv/bin/activate   # On Windows use `venv\Scripts\activate`
3. Install the Required Dependencies
Install the project dependencies listed in requirements.txt:

bash
Copy
Edit
pip install -r requirements.txt
4. Run the Flask Application
Start the Flask development server by running:

bash
Copy
Edit
python app.py
Once the server starts, you should see output similar to the following:

bash
Copy
Edit
 * Running on http://127.0.0.1:5000/ (Press CTRL+C to quit)
5. Play the Game
Open a web browser and go to http://127.0.0.1:5000/. The Snake game should appear, and you can start playing.

How to Play
Arrow Keys: Use the arrow keys (Up, Down, Left, Right) to control the direction of the snake.
Eat Food: Each time the snake eats food, it grows in length and the score increases by 1 point.
Avoid Collisions: The game will end if the snake collides with the walls or its own body.
Restart: After the game ends, simply refresh the page to start a new game.
Scoring
Every time the snake eats food, it gains one point.
The score is displayed at the top of the screen in real-time.
The game ends when the snake collides with the walls or itself.
Project Files
app.py
This is the main Python file that initializes the Flask application and serves the game. It contains the route to render the HTML template where the game is displayed.

templates/index.html
This file contains the HTML structure of the game. It uses the canvas element to render the snake and food, and it links to the CSS and JavaScript files.

static/css/style.css
This file contains the styling for the game. It is used to make the canvas responsive and to style the score display and background.

static/js/game.js
This file contains the JavaScript logic for the Snake game. It handles:

Snake movement.
Food generation.
Collision detection.
Score updating.
Key events to control the snake.
