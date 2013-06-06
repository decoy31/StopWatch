#StopWatch

A simple JavaScript stopwatch class.

```javascript
var stopWatch = new StopWatch();
```

##Properties

###startTime

__Type:__ Date

Start date and time for the stopwatch timer.


###endTime

__Type:__ Date

End date and time for the stopwatch timer.


###difference

__Type:__ Number

Calculated difference between the __[startTime](#startTime)__ and __[endTime](#endTime)__.


##Methods

###start()

__Return Type:__ StopWatch

"Starts" the stopwatch timer.


###stop()

__Return Type:__ StopWatch

"Stops" the stopwatch timer and calculates the __[difference](#difference)__.


###clear()

__Return Type:__ StopWatch

Resets the stopwatch timer.



###getMilliseconds()

__Return Type:__ Number

Returns the elapsed time in milliseconds.


###getSeconds()

__Return Type:__ Number

Returns the elapsed time in seconds.


###getMinutes()

__Return Type:__ Number

Returns the elapsed time in minutes.


###getHours()

__Return Type:__ Number

Returns the elapsed time in hours.


###getDays()

__Return Type:__ Number

Returns the elapsed time in days.


##Example

The following is an example of using StopWatch. A demo of the code below can be found on
[jsFiddle](http://jsfiddle.net/decoy31/qNaV3/).

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
