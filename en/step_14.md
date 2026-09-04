## Lock the controls

Stop the fighting moves from running before the game starts.

![player sprite](images/player.png)

In the `when space key pressed`{:class="block3events"} script, place `punch`{:class="block3custom"} inside an `if then`{:class="block3control"} block that checks whether `playing`{:class="block3variables"} is `1`.

```blocks3
when [space v] key pressed
+if <(playing) = (1)> then
punch :: custom
end
```

Add the same `if playing = 1`{:class="block3control"} check to the `m`, `n`, `up arrow`, and `v` key scripts.

## Now run your code

Click the green flag and tap the move keys during the introduction — nothing happens.

Wait for the introduction to finish. Every move and both walks now work.
