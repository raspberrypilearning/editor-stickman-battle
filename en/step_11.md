## Start the battle

Give the fighter a short introduction, then start the game.

![player sprite](images/player.png)

At the bottom of the setup script, add a pause and two lines for your fighter to shout.

Then set `playing`{:class="block3variables"} to `1` and broadcast `ready`{:class="block3events"} to start the idle animation.

```blocks3
when green flag clicked
set [playing v] to (0)
switch costume to (walk_02 v)
go to [front v] layer
go to x: (0) y: (0)
set rotation style [left-right v]
point in direction (-90)
set size to (250) %
+wait (1) seconds
+say [GOJIRA!!!!] for (2) seconds
+say [I will punch you into the shadow realm!] for (1.5) seconds
+set [playing v] to (1)
+broadcast (ready v)
```

Personalise the two `say ()`{:class="block3looks"} lines.

## Now run your code

Click the green flag. The fighter delivers its lines, then settles into the idle animation.
