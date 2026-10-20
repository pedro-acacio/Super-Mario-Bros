# Super Mario Bros

A work-in-progress recreation of the classic Super Mario Bros mechanics, made in the [Godot 4.4](https://godotengine.org/) engine. The project is still in its early stages: there is a playable character with movement and jumping, and two enemy types (Goomba and Koopa) with basic patrol logic and dying when stomped on, plus the original game's sprites and assets imported into the project.

## Technologies

- Godot Engine 4.4 (GDScript)
- Animated 2D sprites (`AnimatedSprite2D`) and `CharacterBody2D`/`Area2D` physics

## Structure

- `project.godot` — project configuration (input map, collision layers, main scene)
- `player.gd` / `player.tscn` — Mario's movement, jumping and animations (small/big/fire modes)
- `Cenas/enemy.gd`, `Cenas/goomba.gd`, `Cenas/goomba.tscn` — enemy base and the Goomba
- `koopa.gd` / `koopa.tscn` — Koopa Troopa, which hides in its shell when stomped on
- `Assets Super Mario Bros/` — sprites and font used in the game
- `Resources/CollisionShapes/` — collision shapes reused by the enemies
- `main.tscn` — the project's main scene

## How to run

Open the repository folder in Godot Engine 4.4 (importing `project.godot`) and run the main scene from the editor.
