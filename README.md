# Super Mario Bros

Recriação em progresso das mecânicas clássicas de Super Mario Bros, feita na engine [Godot 4.4](https://godotengine.org/). O projeto ainda está no início: há um personagem jogável com movimentação e pulo, e dois tipos de inimigo (Goomba e Koopa) com lógica básica de patrulha e morte ao serem pisados, além dos sprites e assets do jogo original importados no projeto.

## Tecnologias

- Godot Engine 4.4 (GDScript)
- Sprites 2D animados (`AnimatedSprite2D`) e física de `CharacterBody2D`/`Area2D`

## Estrutura

- `project.godot` — configuração do projeto (input map, layers de colisão, cena principal)
- `player.gd` / `player.tscn` — movimentação, pulo e animações do Mario (modos pequeno/grande/atirando)
- `Cenas/enemy.gd`, `Cenas/goomba.gd`, `Cenas/goomba.tscn` — base de inimigos e o Goomba
- `koopa.gd` / `koopa.tscn` — Koopa Troopa, com comportamento de esconder-se na casca ao ser pisado
- `Assets Super Mario Bros/` — sprites e fonte usados no jogo
- `Resources/CollisionShapes/` — formas de colisão reutilizadas pelos inimigos
- `main.tscn` — cena principal do projeto

## Como rodar

Abra a pasta do repositório no Godot Engine 4.4 (importando `project.godot`) e rode a cena principal pelo editor.
