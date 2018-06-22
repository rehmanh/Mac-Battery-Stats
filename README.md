## MacBook-Battery-Stats
---

#### About

This script is intended to provide information about screen usage of your Mac throughout the day. The idea is to have a functional log of the time spent while the Mac is awake. This would be similar to the way that Android OS provides screen usage stats throughout the day.

So far, I am using Darwin logfiles of the battery, so this script isn't compatible with Macs that don't have a battery and rely on AC in.

---

#### Progress 

###### 06/21/2018
- Created options to be passed to the script via arguments. 
- So far, only one argument <-s> – to have the number of secomnds passed since last wake.

---

#### Issues / Notes

- [Apple defines "Charged" status as being anything over 95%](https://developer.apple.com/documentation/iokit/kiopsischargedkey?language=objc) 
- logfiles also include "Display is turned on/off" option
- need to account for date change over midnight of same wake cycle
- need to provide options for:
  1. usage since last wake
  2. usage all day
  3. usage since 100% charge
