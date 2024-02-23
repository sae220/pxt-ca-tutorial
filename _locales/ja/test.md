# テストタイトル

## ステップ 1 (テストステップ)

``||agent: エージェントを自分の位置にもどす||``を``||player: チャットコマンドを入力した時||``の中に入れる

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
