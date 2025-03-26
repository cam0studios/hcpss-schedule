# hcpss-schedule
A library for getting class times and time left for HCPSS classes
## Usage
```js
import { middleTimeSheet, highTimeSheet } from "/path/to/hcpss-schedule/main";

...

// get the current period and time left
middleTimeSheet.current     //  { period: { name: string, start: number, end: number }, timeLeft: number }
// set the current schedule
middleTimeSheet.schedule =  //  0: normal, 1: eagle time, 2: half day, 3: 2 hour delay
// set the user's grade
middleTimeSheet.grade =     //  0: 6th lunch, 1: 7th lunch, 2: 8th lunch

// get the current period and time left
highTimeSheet.current        //  { period: { name: string, start: number, end: number }, timeLeft: number }
// set the current schedule
highTimeSheet.schedule =     //  0: normal, 1: lions' time, 2: half day, 3: 2 hour delay
// set the current day
highTimeSheet.day =          //  0: A day, 2: B day
// set the user's lunches
highTimeSheet.lunchDays =    //  [ A day, B day ], 0: A lunch, 1: B lunch, 2: C lunch, 3: D lunch
// update the current day
highTimeSheet.updateDay()    //  0: set to A, 1: set to B, undefined: not set
```
