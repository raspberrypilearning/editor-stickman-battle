## Make an idle animation

Give the fighter an animation to use while it waits for the player's next move.

![player sprite](images/player.png)

Add a `when I receive ()`{:class="block3events"} block. Make a new message called `ready`.

Add a `repeat until ()`{:class="block3control"} loop with `key any pressed?`{:class="block3sensing"} as its condition.

Inside the loop, cycle through the four `idle` costumes with a short wait after each one.

```blocks3
when I receive (ready v)
repeat until <key (any v) pressed?>
switch costume to (idle_01 v)
wait (0.01) seconds
switch costume to (idle_02 v)
wait (0.01) seconds
switch costume to (idle_03 v)
wait (0.01) seconds
switch costume to (idle_04 v)
wait (0.02) seconds
end
```

The idle animation will start when another script broadcasts `ready`{:class="block3events"}.
