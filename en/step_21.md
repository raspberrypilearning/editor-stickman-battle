## Make enemies bite

Make an enemy damage the fighter when it reaches them.

<h2 class="c-project-heading--explainer">What you need to do</h2>

![enemy sprite](images/enemy-labelled.png)

Click the `Sounds`{:class="block3sound"} tab and add a bite sound and a knock-back sound. The example uses **Bite** and **Boing**.

![The Sounds tab at the top-left of the editor](images/sounds_tab.png)

Go back to the `Code`{:class="block3control"} tab.

In the clone script, add an `if then`{:class="block3control"} block after `next costume`{:class="block3looks"}.

If the clone touches the `player`, play the bite sound, broadcast `hurt`{:class="block3events"}, take away one health point, and delete the clone.

```blocks3
when I start as a clone
show
repeat until <(playing) = (0)>
point towards (player v)
move (2) steps
next costume
+if <touching (player v)?> then
start sound (Bite v)
broadcast (hurt v)
change [health v] by (-1)
delete this clone
end
end
delete this clone
```

## Now run your code

Click the green flag and let an enemy reach the fighter.

The enemy bites, the fighter flinches, and `health`{:class="block3variables"} drops by one.
