## MacBook-Battery-Stats
---

#### About

This script is intended to provide information about screen usage of your Mac throughout the day. The idea is to have a functional log of the time spent while the Mac is awake. This would be similar to the way that Android OS provides screen usage stats throughout the day.

So far, I am using Darwin logfiles of the battery, so this script isn't compatible with Macs that don't have a battery and rely on AC in.

---

#### Progress 06/20/2018

Able to execute embedded CL script in Ruby to perform a search for time since last wake.

Can get time spent since last wake.

---

#### Issues / TODO

- need to account for date change over midnight of same wake cycle
- need to provide options for usage since last 24 hours, last wake, whether Mac was plugged in or not.
- provide stats from last time machine was at 100% charge
