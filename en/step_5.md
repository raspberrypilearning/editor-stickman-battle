## Animate a sword slash

Make a `sword`{:class="block3custom"} block and duplicate the animation blocks again.

![player sprite](images/player.png)

Change them to the eight `sword_slash` costumes. End on `sword_slash_07` to bring the blade back.

```blocks3
define sword
start sound (Rip v)
switch costume to (sword_slash_01 v)
wait (0.01) seconds
switch costume to (sword_slash_02 v)
wait (0.01) seconds
switch costume to (sword_slash_03 v)
wait (0.01) seconds
switch costume to (sword_slash_04 v)
wait (0.01) seconds
switch costume to (sword_slash_05 v)
wait (0.01) seconds
switch costume to (sword_slash_06 v)
wait (0.01) seconds
switch costume to (sword_slash_07 v)
wait (0.01) seconds
switch costume to (sword_slash_08 v)
wait (0.01) seconds
switch costume to (sword_slash_07 v)
wait (0.02) seconds
```

Add a `when n key pressed`{:class="block3events"} script to run it.

```blocks3
when [n v] key pressed
sword :: custom
```

## Now run your code

Press `n`{:class="block3sensing"}. Your fighter swings the sword.
