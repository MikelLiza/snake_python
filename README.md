🐍 Classic Snake Game (Python + Pygame)

A faithful recreation of the iconic Snake game with smooth controls, score tracking, and retro aesthetics. Built using Python and Pygame.

Snake Game Demo (Replace with your gameplay GIF)
Features ✨

    Keyboard Controls – Arrow keys (↑ ↓ ← →) for intuitive movement.

    Score System – Earn points for each apple eaten (score = snake length - 3).

    Collision Detection – Game resets if you hit walls or yourself.

    Visual Polish – Checkerboard grass, custom apple sprite, and score display.

    60 FPS Gameplay – Smooth animations with clock.tick(60).

Installation 🛠️

    Clone the repository:
    sh
    Copy

    git clone https://github.com/your-username/mikelliza-snake_python.git
    cd mikelliza-snake_python

    Install Pygame (requires Python 3.6+):
    sh
    Copy

    pip install pygame

    Run the game:
    sh
    Copy

    python snake.py

How to Play 🎮

    Objective: Grow your snake by eating apples (red squares).

    Controls:

        ↑ / ↓ / ← / → – Change direction.

        ESC or close window – Quit the game.

    Rules:

        Crashing into walls or your tail resets the game.

        Each apple increases your length and score.

Code Highlights 🔍
python
Copy

# Key mechanics from your code:
- Snake movement: Vector2-based grid system (cell_size = 40px).
- Fruit spawn: Randomly generated via FRUIT.randomize().
- Collision checks: compare Vector2 positions of head/fruit/walls.
- Score: Rendered dynamically with pygame.font.

Project Structure 📂
Copy

mikelliza-snake_python/
├── snake.py               # Main game logic (SNAKE, FRUIT, MAIN classes)
└── Graphics/
    └── apple.png          # Custom apple sprite (loaded via pygame.image.load)

Customization 🎨

    Change sprites: Replace Graphics/apple.png with your own image (keep the same name).

    Adjust difficulty: Modify pygame.time.set_timer(SCREEN_UPDATE, 150) (lower = faster).

    Theme: Edit colors in draw_grass() (RGB values) or snake body (currently (183,111,122)).

Future Ideas 💡

    Add a start screen and high-score tracker.

    Implement sound effects (eating, crash).

    Support WASD keys alongside arrows.

License 📜

MIT License – Free for personal and educational use
