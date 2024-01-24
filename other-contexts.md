# Other contexts where a similar technology could be used

For inspiration.

General: Get auto completion of commands for free as an integrated part
of the narrative.

Potentially simpler parser but still with very custom use.  Somewhat of
an illusion.

## Examples

```
can bike to work if
  has_bike(Bike),
  is_oiled(Bike),
  knows_how_to_bike,
  (if (work_end(WorkEndTime), dark_start(DarkTime), before(DarkTime, WorkEndTime)): has_lights(Bike))

knows_how_to_bike if
  ...
```

```
can whip cream if
  open fridge,
  take cream,
  open cream,
  pour cream in bowl,
  open drawer,
  take electric mixer,
  plug in electric mixer to power.

Alternative: can whip cream if
  has(bowl),
  has(cream),
  has(electric mixer),
  plug in electric mixer to power.

can take Item if
  very_close(Item).

can open Item if
  very_close(Item).

very_close(Item) if
  open ParentItem,
  child(ParentItem, Item).

can pour Item1 in Item2 if
  size(Item1, Size1),
  size(Item2, Size2),
  less(Size1, Size2).

can plug in ...

has(Item, !true) if
  take Item.
  
has(Item) if
  has(Item, !true).

has(Item, !false) if
  pour Item in _.
```
