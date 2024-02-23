# test title

## step 1 (test step)

add ``||agent: Agent teleport to player||`` in ``||player: on chat||``

```template
player.onChat("come", function() {
})
player.onChat("go", function() {
})
```

```block
player.onChat("come", function() {
    agent.teleportToPlayer()
})
```

```ghost
player.onChat("ghost", function() {
    agent.turn(TurnDirection.Left)
    agent.place(FORWARD)
})
```
