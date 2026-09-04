## Return to a ready stance

Start the idle animation again after each fighting move.

![player sprite](images/player.png)

Add `broadcast ready`{:class="block3events"} to the end of `punch`{:class="block3custom"}.

```blocks3
switch costume to (punch_01 v)
wait (0.02) seconds
+broadcast (ready v)
```

Add the same `broadcast ready`{:class="block3events"} block to the end of `kick`{:class="block3custom"}, `sword`{:class="block3custom"}, `jump`{:class="block3custom"}, and `roll`{:class="block3custom"}.

## Now run your code

Click the green flag and try each move key.

After every move, the fighter returns to its idle animation.
