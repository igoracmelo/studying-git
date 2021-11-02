# Git tricks for your daily life
## Change last commit
Let's say you add a new cool feature to your `pizza_killer.py` and now you want to commit.

You just have to do:
```sh
git add pizza_killer.py
git commit -m "feat: cheddar splashea"
```

But wait, I you made a mistake!
Instead of typing "splashes", you typed "splashea".

The only solution to this is to ignore it and push, right?

Right...?

**WRONG!**

If its just to change the last commit, you only have to use `--amend`:
```sh
git commit --amend -m "feat: cheddar splashes"
```

But wait a second, you also forgot that you are using `cheddar_splash()` in your `main.py`, so now you're gonna have to create a new commit, right?

Right...?

Ok, I got it... Wrong!

To do that is pretty simple too:
```sh
git add main.py
git commit --amend -m "feat: cheddar splashes"
```

Problem solved 😎!

**Fun fact:** I used amend like 5 times in a row in this topic, because I made a lot of mistakes.


