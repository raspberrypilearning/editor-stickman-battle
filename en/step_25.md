## End the game

Watch the fighter's health and end the battle when it runs out.

<h2 class="c-project-heading--explainer">What you need to do</h2>

![player sprite](images/player.png)

On the `player` sprite, add another green flag script.

Set `health`{:class="block3variables"} to `20`, then wait until it drops below `1`.

Stop the other scripts on the sprite so they cannot interrupt the defeat. Set `playing`{:class="block3variables"} to `0` so the enemies stop, then run `game over`{:class="block3custom"}.

```blocks3
when green flag clicked
set [health v] to (20)
wait until <(health) < (1)>
stop [other scripts in sprite v]
set [playing v] to (0)
game over :: custom
```

## Now run your code

Play until the fighter's health runs out.

The defeat animation plays, **GAME OVER** appears, and the game stops.
