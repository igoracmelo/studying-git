# Git tricks for your daily life
## Change last commit
Let's say you add a new cool feature to your `pizza_killer.py` and now you want to commit.

You just have to do:
```sh
git add pizza_killer.py
git commit -m "feat: chedar splash hit"
```

But wait, you made a mistake!
Instead of typing "cheddar", you typed "chedar".

The only solution to this is to ignore it and push, right?

Right...?

**WRONG!**

If its just to change the last commit, you only have to use `--amend`:
```sh
git commit --amend -m "feat: cheddar splash hit"
```

But wait a second, you also forgot that you are using `cheddar_splash_hit()` in your `game.py`, so now you're gonna have to create a new commit, right?

Right...?

Ok, I got it... Wrong!

To do that is pretty simple too:
```sh
git add game.py
git commit --amend -m "feat: cheddar splash hit"
```

Problem solved 😎!

**Fun fact:** I used amend like 5 times in a row in this topic, because I made a lot of mistakes.


