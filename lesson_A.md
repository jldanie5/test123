### @explicitHints 1
# Activity: Chicken Storm 

## Step 1
Joshua Drag an ``||Player:on chat||`` command into the coding Workspace and change the command to **"chickens"**.

## Step 2
Add a ``||Loops:repeat||`` loop inside ``||Player:on chat command||`` "chickens".

## Step 3
Add a ``||Mobs:spawn animal||`` block inside the ``||Loops:repeat||`` loop.

## Step 4
Change the **Y** coordinate to **10** inside ``||Mobs:spawn animal||``. Chickens will spawn 10 blocks above your head.

### ~ tutorialhint
``` blocks
player.onChat("chickens", function () {
    for (let index = 0; index < 4; index++) {
        mobs.spawn(CHICKEN, pos(0, 10, 0))
    }
})
```

## Step 5
Go into Minecraft, press **T** to open the chat window, and enter **chickens** in the chat window. It’s raining hens! 

## Step 6
Click the (+) next to chickens.  This allows you to specify the number of chickens you want to spawn.  This is a variable. 
By default, it is a number named num1.


## Step 7
More chickens! From ``||Variables:VARIABLES||``, replace the number **4** in ``||Loops:repeat||`` with ``||Variables:num1||``.

### ~ tutorialhint
``` blocks
player.onChat("chickens", function (num1) {
    for (let i = 0; i < num1; i++) {
        mobs.spawn(CHICKEN, pos(0, 10, 0))
    }
})
```
