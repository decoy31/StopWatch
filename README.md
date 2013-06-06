#StopWatch

A simple JavaScript stopwatch class.

```javascript
var stopWatch = new StopWatch();
```

##Properties

###startTime

_Type: Date_

Start date and time for the stopwatch timer.


###endTime

_Type: Date_

End date and time for the stopwatch timer.


###difference

_Type: Number_

Calculated difference between the __[startTime](#starttime)__ and __[endTime](#endtime)__.


##Methods

###start()

_Return Type: StopWatch_

"Starts" the stopwatch timer.


###stop()

_Return Type: StopWatch_

"Stops" the stopwatch timer and calculates the __[difference](#difference)__.


###clear()

_Return Type: StopWatch_

Resets the stopwatch timer.



###getMilliseconds()

_Return Type: Number_

Returns the elapsed time in milliseconds.


###getSeconds()

_Return Type: Number_

Returns the elapsed time in seconds.


###getMinutes()

_Return Type: Number_

Returns the elapsed time in minutes.


###getHours()

_Return Type: Number_

Returns the elapsed time in hours.


###getDays()

_Return Type: Number_

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

##Chaining

Chaining can be used for any of the StopWatch method calls which return the current StopWatch instance. For instance, 
in the [Example section](#example) you could combine the "watch.stop" function call with the "console.log" 
statement by chaining the "getMilliseconds" function call after the "watch.stop" function call and still get the same 
result like so:

```javascript
// Example of chaining with StopWatch.
console.log('Elasped time: ' + watch.stop().getMilliseconds() + 'ms');
```
