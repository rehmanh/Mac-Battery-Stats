## MacBook-Battery-Stats
---

#### About

This script provides output for the time a user spends at their Mac with the screen actively turned on. The inspiration for this came from the Android (AOSP) OS with its built-in functionality to rovide the user with the time they spend looking at the screen at a given charge cycle.

The script utilizes the Darwin logfiles for battery and display usage information to calculate screen usage, for those interested in such statistics.

---

#### Usage

I do not know how to package this script such that you can download it (yet)... more to come.

---

#### Progress 

###### 06/26/2018
- Completed the today option for retreiving screen time for today's date. 
- Need to test for when screen if used through the night into the next day, and then turned off.
- Need to refactor code, __real bad__.
- 

---

#### Issues / Notes

- [Apple defines "Charged" status as being anything over 95%](https://developer.apple.com/documentation/iokit/kiopsischargedkey?language=objc) 
- Figure out how date correlates to the specfic statistic that is required by user. 
