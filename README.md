#StopWatch

A simple JavaScript stopwatch class.

##Properties

###startTime
__Type:__ Date

Start date and time for the stopwatch timer.

###endTime
__Type:__ Date

End date and time for the stopwatch timer.

###difference
__Type:__ Number

Calculated difference between the __[startTime](startTime)__ and __[endTime](endTime)__.

##Methods

###start()
"Starts" the stopwatch timer.

###stop()
"Stops" the stopwatch timer and calculates the __[difference](difference)__.

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
// Initialize a new instance of the StopWatch class.
var watch = new StopWatch();

// "Start" the stopwatch timer.
watch.start();

// Set the timeout function to run in 3000 milliseconds (3 seconds).
setTimeout(function () {
    
    // "Stop" the stopwatch timer and calculate the difference.
    watch.stop();
    
    // Console should approx. read: Elapsed time: 3000ms
    console.log('Elasped time: ' + watch.getMilliseconds() + 'ms');
    
    // Optional cleanup.
    watch.clear();
    
}, 3000);
```

Demo of the above code can be found here: [jsFiddle](http://jsfiddle.net/decoy31/qNaV3/).
