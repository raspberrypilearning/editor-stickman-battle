## React to being hurt

Let the enemy tell the fighter when to play its hurt animation.

![player sprite](images/player.png)

On the `player` sprite, add a `when I receive ()`{:class="block3events"} block.

Make a new message called `hurt` and run the `hurt`{:class="block3custom"} block when the message arrives.

```blocks3
when I receive (hurt v)
hurt :: custom
```

Nothing looks different yet. In the next step, the enemy will broadcast this message when it bites.
