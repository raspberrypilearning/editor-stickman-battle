## Make a game over animation

Animate the fighter's defeat when all its health is gone.

<h2 class="c-project-heading--explainer">What you need to do</h2>

![player sprite](images/player.png)

On the `player` sprite, make a `game over`{:class="block3custom"} block.

Play the death costumes, show a message, then stop the game.

```blocks3
define game over
start sound (Dun Dun Dunnn v)
switch costume to (death_01 v)
wait (0.01) seconds
switch costume to (death_02 v)
wait (0.01) seconds
switch costume to (death_03 v)
wait (0.01) seconds
switch costume to (death_04 v)
wait (0.5) seconds
say [GAME OVER] for (2) seconds
stop [all v]
```

## Now run your code

You'll run this animation when health reaches zero.
