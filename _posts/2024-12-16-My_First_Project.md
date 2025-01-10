---
title: Game Project
date: 2024-12-16 00:00:00 +0800
categories: [Simulation,Game]
tags: [Random,Python]
---

# My First Game Project
The first project that i created is a game about clicking dots that has a difficulty settings, the harder the difficulty the speed of the dot dissapearing and changing location is increased. The game consist of 3 levels of difficulties which is easy, medium, and hard.

Inside the code i use the library Pygames so it can provide more modules that are specifics for making games in Python. It has about 134 lines, it can interact with the cursor clicks for the player
[Click Here to see the code](https://github.com/Nandes012/First-Game-Project/blob/main/Click-The-Circle.py)

```python
while True:
    events = pygame.event.get()
    for event in events:
        if event.type == pygame.QUIT:
            pygame.quit()
            sys.exit()
        if event.type == pygame.MOUSEBUTTONDOWN and not game_won:
            if event.button == 1:
                circle_radius = max(20, 50 - (score * 1.5))
                if check_circle_collision(circle_radius):
                    score += 1
                    if score >= win_goal:
                        game_won = True
                    else:
                        circle_pos = (random.randint(50, 1230), random.randint(50, 670))
                        circle_timer = pygame.time.get_ticks()
                    if difficulty != "easy":  # Adjust speed for normal and hard
                        circle_interval = max(circle_interval_min, circle_interval_base - score * 50)
                elif exit_button_rect.collidepoint(event.pos):
                    pygame.quit()
                    sys.exit()
``` 