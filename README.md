# SpoonDetector

I am so tired of getting reports on GitHub about third party server builds. This is a simple class which will detect if your plugin is running on a spoon, print a message to the console, disable your plugin, and force the user to agree to read and agree to a predefined message.


To install this into your plugin you can copy the SpoonDetector class and change the namespace to your own, or if you are fancy, this is available as a virion. To use it you must add the following to your `onEnable` method

```php
SpoonDetector::printSpoon($this, 'spoon.txt');
```


## What I think about spoons
Spoons are great. However, Spoons do not help the PocketMine community or our open source philosophy, they fragment it. Everyone who uses this library (myself included) is happy for spoon users to use their plugin, they just want to make it clear that they don't have the time to provide support.


## A note to spoon developers

* SpoonDetector is not a "spoon blocker", it will never prevent a plugin from being used on your server.
* SpoonDetector will continue to work regardless of silly reflection hacks you put in place. If you use reflection hacks, you decrease the quality of your software (and mine, but mine is just a hack anyway) and make yourself look silly and childish. So don't do it. 
* If you are a "good spoon" (which I have yet to see), I am willing to remove the detection note. However, you must use entirely independent API versions from PocketMine so that unsupported plugins will not load. Once you do this, create an issue here and I will exempt you.