## Animate the punch

Showing still pictures quickly, one after another, makes the sprite look as though it is moving.

![player sprite](images/player.png)

Under `define punch`{:class="block3custom"}, start the **Tennis Hit** sound.

Switch through the punch costumes with a short wait after each one. Run forwards to `punch_06`, then return through `punch_02` to `punch_01` so the fighter's arm comes back to rest.

```blocks3
define punch
start sound (Tennis Hit v)
switch costume to (punch_01 v)
wait (0.01) seconds
switch costume to (punch_02 v)
wait (0.01) seconds
switch costume to (punch_03 v)
wait (0.01) seconds
switch costume to (punch_04 v)
wait (0.01) seconds
switch costume to (punch_05 v)
wait (0.01) seconds
switch costume to (punch_06 v)
wait (0.01) seconds
switch costume to (punch_02 v)
wait (0.01) seconds
switch costume to (punch_01 v)
wait (0.02) seconds
```

The whole animation can now run from one `punch`{:class="block3custom"} block.
