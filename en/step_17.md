## Create enemy clones

A clone is a working copy of a sprite that runs its own scripts.

<h2 class="c-project-heading--explainer">What you need to do</h2>

![enemy sprite](images/enemy-labelled.png)

Inside the spawning loop, add an `if then else`{:class="block3control"} block.

For side `1`, move the original enemy to the left edge before making a clone. Otherwise, move it to the right edge before making a clone.

```blocks3
when I receive (dino v)
repeat until <(playing) = (0)>
set [side v] to (pick random (1) to (2))
+if <(side) = (1)> then
go to x: (-280) y: (0)
create clone of (myself v)
else
go to x: (280) y: (0)
create clone of (myself v)
end
wait (1) seconds
end
```

## Now run your code

The clones are still hidden and stationary. You'll make them chase the fighter next.
