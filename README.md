# SpoonDetector

I am so tired of getting reports on GitHub about third party server builds. This is a simple class which will detect if your plugin is running on a spoon, print a message to the console, disable your plugin, and force the user to agree to read and agree to a predefined message.


To install this into your plugin you can copy the SpoonDetector class and change the namespace to your own, or if you are fancy, this is available as a virion. To use it you must add the following to your `onEnable` method

```php
SpoonDetector::printSpoon($this, 'spoon.txt');
```

