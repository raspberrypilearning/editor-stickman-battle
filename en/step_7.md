## Add a dash roll

Add a roll that moves the fighter quickly out of danger.

<h2 class="c-project-heading--explainer">What you need to do</h2>

![player sprite](images/player.png)

Make a `roll`{:class="block3custom"} block. Add a sound, then switch through the five `dash_roll` costumes.

Add `move () steps`{:class="block3motion"} before each costume switch so the fighter slides forwards during the roll.

```blocks3
define roll
start sound (Rip v)
move (5) steps
switch costume to (dash_roll_01 v)
wait (0.01) seconds
move (5) steps
switch costume to (dash_roll_02 v)
wait (0.01) seconds
move (5) steps
switch costume to (dash_roll_03 v)
wait (0.01) seconds
move (5) steps
switch costume to (dash_roll_04 v)
wait (0.01) seconds
move (5) steps
switch costume to (dash_roll_05 v)
wait (0.02) seconds
```

Change all five `move 5 steps`{:class="block3motion"} blocks to the same larger number for a longer dash, or the same smaller number for a shorter dash.

Add a `when v key pressed`{:class="block3events"} script to run `roll`{:class="block3custom"}.

```blocks3
when [v v] key pressed
roll :: custom
```

## Now run your code

Press `v`{:class="block3sensing"}. The fighter rolls smoothly across the stage.
