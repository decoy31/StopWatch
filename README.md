#StopWatch

A simple JavaScript stopwatch class.

##Methods

###start()
"Starts" the stopwatch timer.

###stop()
"Stops" the stopwatch timer and calculates the difference.

###clear()
Resets the stopwatch timer.

###getMilliseconds()
Returns the elapsed time in milliseconds.

###getSeconds()
Returns the elapsed time in seconds.

###getMinutes()
Returns the elapsed time in minutes.

###getHours()
Returns the elapsed time in hours.

###getDays()
Returns the elapsed time in days.

##Example

The following is an example of using StopWatch:

```javascript
var watch = new StopWatch(); // Initialize a new instance of the StopWatch class.
watch.start(); // "Start" the stopwatch timer.

setTimeout(function () {
    watch.stop(); // "Stop" the stopwatch timer and calculate the difference.
    console.log('Elasped time: ' + watch.getMilliseconds() + 'ms'); // Console should approx. read: Elapsed time: 3000ms
    watch.clear(); // optional
}, 3000); // 3000ms (or 3 seconds)
```

Demo of the above code can be found here: [jsFiddle](http://jsfiddle.net/decoy31/qNaV3/).
