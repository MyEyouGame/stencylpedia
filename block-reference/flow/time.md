# Flow > Time

***

## Delayed

### <a name="dolater"></a> Do after N seconds

![do-after-block](http://static.stencyl.com/pedia2/block-images/1%20-%20Flow/2%20-%20Time/dolater.png)

Runs the code after the given delay (in seconds, can be partial seconds).

```
runLater(1000 * [NUMBER], function(task:TimedTask):Void {
  [ACTIONS]
});
```

> **Warning:** Do not use this block in a `when updating` event, unless constrained by an `if` block or other conditional.

***

## Periodic

### <a name="periodic"></a> Do every N seconds

![do-every-block](http://static.stencyl.com/pedia2/block-images/1%20-%20Flow/2%20-%20Time/periodic.png)

Runs the code every [N] seconds (can be partial seconds).

```
runPeriodically(1000 * [NUMBER], function(task:TimedTask):Void {
  [ACTIONS]
});
```

> **Warning:** Do not use this block in a `when updating` event, unless constrained by an `if` block or other conditional.

#### Example

![time-example](http://static.stencyl.com/pedia2/blocks/flow/flow_time/PeriodicExample2.png)

`do after n seconds` and `do every n seconds` can be combined together. In this example, we implement a "blinking" effect by alternating the actor between hidden and not-hidden, without relying on a variable to store state.


### <a name="cancel"></a> Cancel

![cancel-block](http://static.stencyl.com/pedia2/block-images/1%20-%20Flow/2%20-%20Time/cancel.png)

Cancels the execution of a periodic (`do every n seconds`) task.

```
timeTask.repeats = false;
return;
```

***
