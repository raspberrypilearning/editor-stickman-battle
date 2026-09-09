## Move right

Make the fighter walk right while cycling through its idle costumes.

<h2 class="c-project-heading--explainer">What you need to do</h2>

![player sprite](images/player.png)

Add a `when right arrow key pressed`{:class="block3events"} script.

Only move when `playing`{:class="block3variables"} is `1`, after the introduction has finished.

```blocks3
when [right arrow v] key pressed
if <(playing) = (1)> then
point in direction (90)
switch costume to (idle_01 v)
change x by (2)
wait (0.01) seconds
switch costume to (idle_02 v)
change x by (2)
wait (0.01) seconds
switch costume to (idle_03 v)
change x by (2)
wait (0.01) seconds
switch costume to (idle_04 v)
change x by (2)
broadcast (ready v)
end
```

## Now run your code

Click the green flag, wait for the introduction, then press the right arrow.

The fighter walks right and faces that way.
