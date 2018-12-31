# User Input > Mobile-Only

***

> **Note:** These blocks only work on iOS and Android. They have no effect on other platforms (or return 0/-1/useless values).

***

## Accelerometer

### <a name="accelerometer"></a> Accelerometer Value

![accel-block](http://static.stencyl.com/pedia2/blocks/user_input/mobile/Accel.png)

Returns the current values for the [accelerometer](http://www.stencyl.com/help/view/mobile-accelerometer/).

**Portrait Orientation**

Name | Description
--- | ---
X (Positive) | Right
X (Negative) | Left
Y (Positive) | Up
Y (Negative) | Down

**Landscape Orientation**

Name | Description
--- | ---
X (Positive) | Up
X (Negative) | Down
Y (Positive) | Left
Y (Negative) | Right

```
Input.accelX
Input.accelY
```

***

## Gestures

### <a name="swipe-detect"></a> Swiped

![swipe-block](http://static.stencyl.com/pedia2/blocks/user_input/mobile/Swipe.png)

Returns `true` if the user has swiped [up/down/left/right]. A swipe is defined as touching the screen, sliding the finger and then releasing.

```
Input.swipedUp
Input.swipedDown
Input.swipedLeft
Input.swipedRight
```

#### Alernate Approach: Events

![swipe-event](http://static.stencyl.com/help/images/mobile-input-5.png)

We recommend using a swipe event instead of a swipe block. It's easier to work with.


***

## Other

### <a name="show-hide-keyboard"></a> Show / Hide Keyboard

![keyboard-block](http://static.stencyl.com/pedia2/blocks/user_input/mobile/Keyboard.png)

Immediately shows or hides the [virtual keyboard](http://www.stencyl.com/help/view/mobile-features/). Use mobile keyboard events to track what's been typed.

![example](http://static.stencyl.com/help/images/mobile-features-3.png)

```
showKeyboard();
hideKeyboard();
```

***

### <a name="set-keyboard-text"></a> Set Keyboard Text

![text-block](http://static.stencyl.com/pedia2/blocks/user_input/mobile/KeyboardText.png)

Imagine that the keyboard is inputting into an invisible text field. This sets the text that's in that text field.

```
setKeyboardText([TEXT]);
```

***

### <a name="clear-keyboard-text"></a> Clear Keyboard Text

![clear-block](http://static.stencyl.com/pedia2/blocks/user_input/mobile/ClearKeyboard.png)

Imagine that the keyboard is inputting into an invisible text field. This clears out the text that's in that text field.

```
setKeyboardText("");
```

***

### <a name="vibrate"></a> Vibrate

![vibrate-block](http://static.stencyl.com/pedia2/blocks/user_input/mobile/Vibrate.png)

[Vibrates](http://www.stencyl.com/help/view/mobile-features/) the device for the given number of seconds. On some devices, vibration duration cannot be controlled.

```
vibrate([NUMBER]);
```

***
