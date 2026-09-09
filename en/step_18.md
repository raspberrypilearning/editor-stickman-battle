## Make enemies chase

Start the enemy wave and make each clone move towards the fighter.

<h2 class="c-project-heading--explainer">What you need to do</h2>

## Step 1

Click on the `player` sprite.

At the end of its green flag script, broadcast the `dino`{:class="block3events"} message after `ready`{:class="block3events"}.

```blocks3
set [playing v] to (1)
broadcast (ready v)
+broadcast (dino v)
```

## Step 2

Click on the `enemy` sprite.

Make each clone appear and move towards the `player` while changing costume. When the game ends, delete the clone.

```blocks3
when I start as a clone
show
repeat until <(playing) = (0)>
point towards (player v)
move (2) steps
next costume
end
delete this clone
```

## Now run your code

Click the green flag. After the introduction, enemies appear from both sides and close in on the fighter.
