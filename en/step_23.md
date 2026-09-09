## Knock enemies away

Make a strike defeat an enemy before it can bite.

<h2 class="c-project-heading--explainer">What you need to do</h2>

![enemy sprite](images/enemy-labelled.png)

Click on the `enemy` sprite and find `if touching player`{:class="block3control"}.

Add an `if then else`{:class="block3control"} choice inside it:

- If the clone touches the strike colour, play **Boing**, turn around, move away, and delete the clone
- Otherwise, run the bite blocks

Click the colour in `touching color?`{:class="block3sensing"}, choose the eyedropper, and pick the strike colour from the fighter on the Stage.

```blocks3
if <touching (player v)?> then
+if <touching color [#ffe500]?> then
start sound (Boing v)
turn right (180) degrees
repeat (20)
move (20) steps
end
delete this clone
else
start sound (Bite v)
broadcast (hurt v)
change [health v] by (-1)
delete this clone
end
end
```

## Now run your code

Turn to face an incoming enemy and strike as it arrives. The enemy is knocked away.

Stand still and let another enemy reach the fighter. It bites instead.
