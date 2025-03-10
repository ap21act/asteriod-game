# Asteroids Game Clone

A Python implementation of the classic [Asteroids](w) arcade game using [Pygame](w).

## Overview
This project recreates the iconic Asteroids arcade game where players navigate a triangular spaceship through an asteroid field. Shoot asteroids to split them into smaller pieces and avoid collisions to survive as long as possible.

## Features
- Ship rotation and movement physics
- Asteroid splitting mechanics
- Projectile shooting system
- Collision detection
- Procedural asteroid field generation
- Screen wrapping for all game objects

## Prerequisites
- [Python 3.x](w)
- [Pygame](w)

## Installation
```sh
git clone https://github.com/your-username/asteroids-clone.git
cd asteroids-clone
pip install pygame
```

## How to Play
```sh
python main.py
```

## Controls
```
W - Thrust forward
S - Thrust backward
A - Rotate counterclockwise
D - Rotate clockwise
SPACE - Fire projectiles
```

## Game Mechanics
- **Ship Movement**: The player's ship rotates and accelerates in the direction it's facing.
- **Asteroids**: Large asteroids split into smaller ones when shot.
- **Collision**: The game ends if the player collides with any asteroid.
- **Asteroid Field**: New asteroids continuously spawn from the edges of the screen.

## Project Structure
```
asteroids-clone/
├── main.py          # Game initialization, main loop, and collision handling
├── player.py        # Player ship controls, movement, and shooting mechanics
├── asteroid.py      # Asteroid behavior and splitting logic
├── shot.py          # Projectile physics and rendering
├── asteroidfield.py # Manages procedural asteroid spawning
├── constants.py     # Game configuration (speeds, sizes, timers)
├── circleshape.py   # Base class for circular collision detection
└── assets/          # Sprites, sounds, and other resources
```

## Code Architecture
- **CircleShape**: Base class for all game objects with collision detection.
- **Inheritance hierarchy** for specialized game objects (*Player, Asteroid, Shot*).
- **Pygame sprite groups** for efficient updates and rendering.
- **Delta-time based movement** for consistent physics regardless of frame rate.

## Key Constants
```
Screen dimensions: 1280×720
Player movement speed: 200 units/second
Player rotation speed: 300 degrees/second
Shot speed: 500 units/second
Multiple asteroid sizes with different behaviors
```

## Future Enhancements
- Scoring system
- Lives system
- Sound effects and background music
- Visual effects (explosions, thruster particles)
- Level progression
- Power-ups

## Contributing
```sh
git fork
cd asteroids-clone
git checkout -b new-feature
git commit -am "Add new feature"
git push origin new-feature
```
Submit a pull request.

## License
This project is licensed under the [MIT License](w).

## Acknowledgments
- Original [Asteroids](w) game by Atari
- [Pygame](w) community and documentation

