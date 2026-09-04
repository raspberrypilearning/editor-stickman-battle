## Move left

Make the fighter walk in the other direction.

![player sprite](images/player.png)

Duplicate the `when right arrow key pressed`{:class="block3events"} script.

On the copy, change the key to `left arrow`{:class="block3sensing"}, the direction to `-90`, and every `change x by 2`{:class="block3motion"} block to `change x by -2`{:class="block3motion"}.

```blocks3
when [left arrow v] key pressed
if <(playing) = (1)> then
point in direction (-90)
switch costume to (idle_01 v)
change x by (-2)
wait (0.01) seconds
switch costume to (idle_02 v)
change x by (-2)
wait (0.01) seconds
switch costume to (idle_03 v)
change x by (-2)
wait (0.01) seconds
switch costume to (idle_04 v)
change x by (-2)
broadcast (ready v)
end
```

## Now run your code

Hold the left and right arrows. The fighter walks both ways and faces the direction it is moving.
