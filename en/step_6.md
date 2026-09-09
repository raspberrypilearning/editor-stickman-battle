## Animate a jump

Make a `jump`{:class="block3custom"} block and duplicate the animation blocks again.

<h2 class="c-project-heading--explainer">What you need to do</h2>

![player sprite](images/player.png)

Use the seven `jump` costumes.

```blocks3
define jump
start sound (Rip v)
switch costume to (jump_01 v)
wait (0.01) seconds
switch costume to (jump_02 v)
wait (0.01) seconds
switch costume to (jump_03 v)
wait (0.01) seconds
switch costume to (jump_04 v)
wait (0.01) seconds
switch costume to (jump_05 v)
wait (0.01) seconds
switch costume to (jump_06 v)
wait (0.01) seconds
switch costume to (jump_07 v)
wait (0.02) seconds
```

Add a `when up arrow key pressed`{:class="block3events"} script to run it.

```blocks3
when [up arrow v] key pressed
jump :: custom
```

## Now run your code

Press the up arrow. Your fighter jumps.
