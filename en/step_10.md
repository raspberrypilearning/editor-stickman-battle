## Set up the fighter

Set the fighter's costume, position, direction, and size at the start of every game.

![player sprite](images/player.png)

Make a variable called `playing`{:class="block3variables"}, **For all sprites**. Untick its checkbox so it does not appear on the Stage.

![The playing variable unticked in the Variables palette](images/variable-playing.png)

Add a `when green flag clicked`{:class="block3events"} script to the `player` sprite.

Set `playing`{:class="block3variables"} to `0` first, so none of the controls work during the introduction.

```blocks3
when green flag clicked
set [playing v] to (0)
switch costume to (walk_02 v)
go to [front v] layer
go to x: (0) y: (0)
set rotation style [left-right v]
point in direction (-90)
set size to (250) %
```

The `set rotation style left-right`{:class="block3motion"} block lets the fighter face left or right without turning upside down.

Change the size if your fighter looks too big or too small on the Stage.
