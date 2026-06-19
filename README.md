# Airstrike Game Using Rocket

A Python Pygame-based computer graphics academic project where the player controls a rocket, shoots enemy planes, avoids bombs, and tries to achieve the highest score.

## Project Overview

**Airstrike Game Using Rocket** is a 2D arcade-style game developed using Python and Pygame. The game includes rocket movement, shooting mechanics, enemy planes, a big boss plane, bomb attacks, difficulty levels, score tracking, and sound effects.

This project was developed as an academic computer graphics project.

## Features

* Main menu system
* Player ID and player name input
* Difficulty levels: Easy, Medium, Hard
* Rocket movement using keyboard controls
* Shooting system using the Spacebar
* Enemy planes with random movement
* Big plane/boss enemy
* Bomb dropping system from the big plane
* Collision detection
* Explosion sound effect
* Score tracking
* Missed plane tracking
* Rocket hit counter
* Top score display system
* Score saving in a text file

## Technologies Used

* Python
* Pygame
* File Handling
* Basic Computer Graphics Concepts
* Collision Detection
* Game Loop Logic

## Game Controls

| Key         | Action              |
| ----------- | ------------------- |
| Up Arrow    | Move rocket up      |
| Down Arrow  | Move rocket down    |
| Left Arrow  | Move rocket left    |
| Right Arrow | Move rocket right   |
| Spacebar    | Shoot               |
| Enter       | Confirm input/start |
| 1, 2, 3     | Select menu options |

## Project Structure

```text
Academic-Project-on-computer-graphics-/
│
├── rocket.py
├── boom.wav
├── README.md
├── requirements.txt
├── .gitignore
│
├── docs/
│   ├── project for game development.docx
│   ├── Rocket Launch.pptx
│   ├── UML class.jpeg
│   └── Use case diagram.jpeg
│
└── screenshots/
    └── UI interface.png
```

## How to Run the Project

### Step 1: Clone the Repository

```bash
git clone https://github.com/Elahi-01/Academic-Project-on-computer-graphics-.git
cd Academic-Project-on-computer-graphics-
```

### Step 2: Install Required Package

```bash
pip install -r requirements.txt
```

If `requirements.txt` is not available, install Pygame manually:

```bash
pip install pygame
```

### Step 3: Run the Game

```bash
python rocket.py
```

## Required Files

Make sure these files are in the same project folder:

```text
rocket.py
boom.wav
```

The `boom.wav` file is used as the collision/explosion sound effect.

## Difficulty Levels

| Difficulty | Plane Speed | Missed Plane Limit |
| ---------- | ----------: | -----------------: |
| Easy       |         Low |                 10 |
| Medium     |      Medium |                  5 |
| Hard       |        High |                  3 |

## Gameplay Summary

The player controls a rocket and shoots enemy planes. If a plane is hit, the score increases. If too many planes are missed, the game ends. After reaching a certain score, a big plane appears and drops bombs. The rocket must avoid the bombs and continue scoring.

## Score System

* Destroying a normal plane increases the score.
* Destroying the big plane gives bonus points.
* Scores are saved in `scores.txt`.
* The score display menu shows top scores.

## Screenshots

### Game Interface

![Game Interface](screenshots/UI%20interface.png)

## Documentation

This repository also includes academic project documents such as:

* Project development document
* Presentation file
* UML class diagram
* Use case diagram
* Cost estimation documents

These files are stored in the `docs/` folder.

## Build EXE Version

To create a Windows executable file:

```bash
pip install pyinstaller
pyinstaller --onefile --windowed --add-data "boom.wav;." rocket.py
```

After building, the executable file will be available inside:

```text
dist/rocket.exe
```

## Download EXE

You can download the playable Windows version from the **Releases** section of this repository.

## Author

**MD Fazley Elahi**

GitHub: [Elahi-01](https://github.com/Elahi-01)

## License

This project is created for academic and learning purposes.
