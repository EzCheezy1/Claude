# Spot Me

A shared workout log for two training partners. Live version: https://claude.ai/artifact/QQFpdW6DCtxeUvWf13zmoG

- Log sessions as exercises with weight × reps sets (lb)
- Head-to-head board of each lifter's best estimated 1RM (Epley) per lift
- Progress chart of estimated 1RM over time, per lifter
- PR badges on sets that beat a lifter's previous best

`index.html` is the page source. It syncs through the Claude artifact database (`db` + `user` capabilities); opened outside claude.ai it falls back to saving in the browser only.
