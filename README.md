## MacBook-Battery-Stats
---

#### About

This script is intended to provide information about screen usage of your Mac throughout the day. The idea is to have a functional log of the time spent while the Mac is awake. This would be similar to the way that Android OS provides screen usage stats throughout the day.

Utilizes the Darwin logfiles for battery and display usage statistics to calculate screen usage, for those interested in such information.

---

#### Progress 

###### 06/25/2018
- Date change overnight resets the log, need to assume that if logfile is empty then the user has used machine into new date
- Started providing options
- Maybe think about providing date options... eh

---

#### Issues / Notes

- [Apple defines "Charged" status as being anything over 95%](https://developer.apple.com/documentation/iokit/kiopsischargedkey?language=objc) 
- Figure out how date correlates to the specfic statistic that is required by user. 
