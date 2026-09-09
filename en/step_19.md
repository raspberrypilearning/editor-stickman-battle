## Make a hurt animation

Give the fighter health and an animation for taking damage.

<h2 class="c-project-heading--explainer">What you need to do</h2>

![player sprite](images/player.png)

Make a variable called `health`{:class="block3variables"}, **For all sprites**. Tick its checkbox so the player can see it.

![The health variable ticked in the Variables palette](images/variable-health.png)

On the `player` sprite, make a `hurt`{:class="block3custom"} block.

Play the hurt costumes and move backwards a little, then return to the ready stance.

```blocks3
define hurt
start sound (Crunch v)
move (-2) steps
switch costume to (hurt_01 v)
wait (0.01) seconds
switch costume to (hurt_02 v)
wait (0.01) seconds
switch costume to (hurt_03 v)
wait (0.02) seconds
broadcast (ready v)
```

## Now run your code

The enemy will run this block when it reaches the fighter.
