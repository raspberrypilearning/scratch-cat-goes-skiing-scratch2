## Crashing

If the skier crashes into an obstacle, it should fall over and the game should end.

![skier crashed](images/skier_crash.png)

--- task ---

Change the code for the skier sprite to `wait until`{:class="blockcontrol"} it is `touching`{:class="blocksensing"} the obstacle, and to then `stop all`{:class="blockcontrol"}.

![skier sprite](images/skier_sprite_small.png)

```blocks
when green flag clicked
wait until <touching [Tree2 v] ?>
stop [all v]
```

--- /task ---

--- task ---

When the skier crashes, you should also `switch costume to fallenover`{:class="blocklooks"}.

The updated code should look like this:

![skier sprite](images/skier_sprite_small.png)

```blocks
when green flag clicked
wait until <touching [Tree2 v] ?>
+ switch costume to [fallenover v]
stop [all v]
```
--- /task ---

--- task ---

Save and test your code. When the skier hits the obstacle, the costume should change and the game should stop. 

--- /task ---

However, there is a now problem with your game: the next time you run it, the skier will still be wearing the `fallenover`{:class="blocklooks"} costume.

--- task ---

Edit the skier's so that their costume changes back to `skiing`{:class="blocklooks"} when the game starts by `switching the costume to skiing`{:class="blocklooks"}.

![skier sprite](images/skier_sprite_small.png)

```blocks
when green flag clicked
+ switch costume to [skiing v]
wait until <touching [Tree2 v] ?>
switch costume to [fallenover v]
stop [all v]
```
--- /task ---