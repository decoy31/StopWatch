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
var watch = new StopWatch();
watch.start();
setTimeout(function () {
  watch.stop();
}, 3000);
console.log('Elasped time: ' + watch.getMilliseconds() + 'ms'); // Console should: Elapsed time 3000ms
watch.clear(); // optional
```
