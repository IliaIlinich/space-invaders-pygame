# Space Invaders PyGame

A classic Space Invaders-style arcade game built with Python and PyGame. The player controls a spaceship, shoots waves of descending aliens, protects bases, and competes for the highest score.

## Features

- Classic Space Invaders gameplay
- Multiple alien types with animated sprites
- Destructible shields
- Score tracking and persistent high-score history
- Main menu with scoreboard access
- Pause / return to menu with `Escape`

## Tech Stack

- **Python 3**
- **PyGame** — game graphics, input, and audio handling

## Project Structure

```text
space-invaders-pygame/
├── main.py                 # Game entry point
├── alienController.py      # Alien behavior and movement logic
├── alienLevels.py          # Level configuration and progression
├── bulletController.py     # Player and alien bullet logic
├── playerControler.py      # Player ship movement and shooting
├── scoreController.py      # Score tracking and high-score management
├── shieldController.py     # Shield/base destruction mechanics
├── highestScores.json      # Persistent high-score data
├── doc link.txt            # External documentation link
├── .gitignore
├── README.md
└── Sprites/                # Game assets
    ├── Space_Invaders_Logo.jpg
    ├── player_sprite.png
    ├── Aliens/
    │   ├── alien_1_sprite_1.png
    │   ├── alien_1_sprite_2.png
    │   ├── alien_2_sprite_1.png
    │   ├── alien_2_sprite_2.png
    │   ├── alien_3_sprite_1.png
    │   └── alien_3_sprite_2.png
    └── base/
        ├── normal/
        ├── top_left/
        ├── top_right/
        ├── bottom_left/
        └── bottom_right/
```

## Installation

### 1. Clone the repository

```bash
git clone https://github.com/IliaIlinich/space-invaders-pygame.git
cd space-invaders-pygame
```

### 2. Create a virtual environment (recommended)

```bash
python3 -m venv venv
source venv/bin/activate        # On Linux / macOS
# venv\Scripts\activate.bat     # On Windows
```

### 3. Install dependencies

```bash
pip install pygame
```

> If the project includes a `requirements.txt`, use:
>
> ```bash
> pip install -r requirements.txt
> ```

## How to Run

Start the game from the project root:

```bash
python3 main.py
```

## Controls

| Key | Action |
|---|---|
| `←` / `→` | Move the spaceship left / right |
| `Space` | Shoot |
| `Escape` | Return to the main menu |
| `Score` button | View high-score history from the menu |

## Gameplay

- Destroy all aliens before they reach the bottom of the screen.
- Use shields for cover — they take damage from both enemy and friendly fire.
- Your score is saved automatically when you die.
- Check the highest scores from the main menu.

## Notes

- High scores are stored in `highestScores.json`.
- Press `Escape` at any time to return to the main menu.
- This project was created for educational purposes.
