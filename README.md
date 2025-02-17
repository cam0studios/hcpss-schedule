# hcpss-schedule
A library for getting class times and time left for HCPSS classes
## Usage
```js
import { TimeSheet, middleTimesheet, highTimesheet } from "/path/to/hcpss-schedule/main";

...

// HCPSS schedules
middleTimesheet.getCurrentPeriod(); // { period: { name: string, start: number, end: number }, timeLeft: number }
highTimesheet.getCurrentPeriod();   // { period: { name: string, start: number, end: number }, timeLeft: number }

// Other utils
let time = "12:00";
let timeNum = TimeSheet.getTimeFromString(time);  // 720
TimeSheet.formatTime(timeNum, { hour: true, minute: true, second: false })  // "12:00"
```
