# fun expressions

- mole goals ("moals"? quest system?)
- holy moley
- break the mole-d


# start of game

- ask for name but discard it because moles don't have names


# middle-to-late-game above-ground power fantasies

- peace treaty with humans (mole is best diplomat)
- war with humans (mole is best warrior)
- mars colony (mole is best astronaut)


# easily solvable dilemma

mole must choose between save pups (near kidnapper) or save mole love
(near trap)

no

mole can both save pups and save mole love

## problem

start of game only has something like a `Mole can Action` rule.

But the actions need to be done at the same time.

## solution

Add a `Mole can {Action1 and Action2} if Action1, Action2` rule to
indicate that both actions are done in a single turn.


# need to change the past

same plot as superman (1979)

change the past by changing the written history


# fast travel by induction

mole can dig through earth

mole move forward when mole dig

## problem

can mole reach 100 spaces forward?


## solution 1

mole dig

mole dig

mole dig

...


## solution 2

```
n zero action if
  do action.

n s(X) action if
  do action
  n X action.
```

n 100 (mole dig)


# order of actions

action has order

mole can only do action if first action or if another previous action

```
Entity can X if
  actions none.

Entity can X if
  actions Y,
  any from Y Z,
  Z order before X
```

## gameplay uses if changed

- Entity can do action also before some other action (time travel)
- Entity cannot do any action (avoid responsibility)


# when asking for help

mole does not need help.

mole can:

  - eat
  - sleep
  - ...


# refine what mole can do

mole can do everything

but it can be useful to sometimes only do some things

## problem

It has been established earlier that the mole can dig through anything.

It has also been established that the mole will do what is needed from
it independently of whether it wants to do it.

In this case it needs to say hello to an aquaintance on the other side
of a wall, but it doesn't like the aquaintance very much.

It is however forced to say hello, since it can just dig through the
wall.

A solution to this problem is to remove the ability to dig through
walls.

In other words, it is a moal (don't have the ability to say hello) to
remove another moal (always say hello when possible).

## solution

Refine the `mole can dig through X` rule to only work in non-wall cases
of `X`?

Maybe a `mole can lie to itself`?
