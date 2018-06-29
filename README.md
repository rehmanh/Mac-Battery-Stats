## Mac-Screen-Time

#### About

This script provides information for the time spent at your Mac with the screen actively turned on. The inspiration for this came from the Android (AOSP) OS with its built-in functionality to provide users with the time they spend looking at the screen in a given charge cycle.

---

#### Installation

###### Option 1: Git

1. Use the [Clone](https://github.com/rehmanh/Mac-Battery-Stats.git) option above to copy the Git URL.
2. Open up a terminal on your Mac and navigate to whatever directory you want to place the script in, eg `$ cd ~/path/to/directory`
3. Use `git clone https://github.com/rehmanh/Mac-Battery-Stats.git` 
4. Add the screen_time script to your $PATH to be able to access it anywhere system-wide. In your `.*shrc` file add the following line before existing exports: `export PATH="$PATH:$HOME/path/to/cloned/repository"`

###### Option 2: Download the Source

1. Use the download link above to download a zipped version of the repository.
2. Copy and paste the zip file into any directory you wish, then unzip the file to reveal its contents.
3. Use the script from the directory by referring the usage options below, or
4. Add the `screen_time` script to your $PATH to be able to access it anywhere system-wide. In your `.*shrc` file add the following line before existing exports: `export PATH="$PATH:$HOME/path/to/cloned/repository"`

---

#### Usage

`./screen_time <options>` from the repo directory, or
`screen_time <options>` from any directory if the PATH is exported (see installation instructions above).

###### Options:
`-r` : to get screen-time since most recent wake / boot
`-d` : to get screen-time of current date
`-A` : to get scree-time since device was last fully charged (for Macs with batteries)

---

#### Progress 

###### 06/28/2018
- All options are working.
- Need to test all options for when user keeps machine on into the next day, more to come.
- Refactored some code, refactor more if possible.

---

#### Issues / Notes

- [Apple defines "Charged" status as being anything over 95%](https://developer.apple.com/documentation/iokit/kiopsischargedkey?language=objc). `screen_time` defines fully charged as a device reaching 100% charge.
- reported time is inaccurate by mere seconds because of the fact that conversions from `Time` class are parsed to integers first.
- Does __not__ account for time-zone changes, or Daylight savings.

