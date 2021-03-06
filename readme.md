# Scripts for Things by Cultured Code 

## Clean Things Today list

Just a simple script to move all tasks from the Todays list to Anytime so each day I start with a fresh list. This forces me to do the daily reviews instead.

### Updated for Things 3!

The Clean Things Today script now works with Things 3. 

## Scheduling the script

I'm using [Lingon App](https://www.peterborgapps.com/lingon/) to schedule the running of my scripts.

The great thing is that they even run when my Mac sleeps ([ power nap? ](https://support.apple.com/en-us/HT204032)), and I have a clean Today's list in the morning on iPhone! 

---

### Warning!

The scripts below have not yet been tested with Things 3!

## Queue Tasks

This script will move all todos except the first open one to the Someday list. This will in turn make your tasks sequential.
 
### Motivation

 I've been using Things for at least 5 years, when I came across this article from 2009:
 
[Why Cultured Code’s “Things” app can’t do GTD](https://txfx.net/2009/02/05/why-cultured-codes-things-app-cant-do-gtd/)

Then it hit me. It's not my laziness stopping me advancing through my Next list.
If you're really committed to using a tool to capture all your open loops, then your Next list in Things will normally contain between 30 and 150 items. That's just too much to scroll through. Yes, you can filter this list, but still you get a lot of "junk", i.e. tasks that you cannot act upon, since they depend on a previous task to be finished.
 
### How I use it

You can launch the .scpt files from anywhere, but usually one places these files into ~/Library/Scripts, so you can access them from the scripts menu on your OS X menubar. It's also possible to launch script via system wide keyboard shortcuts.
 
For maximum geek pleasure, I've set up a recurring task with [Lingon](https://www.peterborgapps.com/lingon/) to launch this script every 20 minutes. I have an old Mac Mini that's running all day and periodically cleans up my Next list.
 In the end, I have much cleaner list of my task:

![Screenshot of cleaned up Next list on iPhone](http://815b1b87b51011a7a029-623c55fb68acb92f1f433c6448bed244.r60.cf3.rackcdn.com/github/things-scripts/queued-tasks.jpg)

### Check if todo is active script

The _check if todo is active.scpt_ file is the subroutine used in the main queue task.scpt file. I just put it there so that you can test the script before unleashing it on your entire Things library. Create a project in Things called _MyTestProject_, launch this script and see what happens. If you're satisfied you can launch the main _queue tasks.scpt_ file.

### Parallel tasks

I will probably add a _"skip projects tagged with"_ feature, where you can add a special tag, e.g. _"parallel"_ and the script will skip that project.

## Note on JXA vs. AppleScript

I'm a JavaScript guy. Still, I wouldn't recommend trying to script apps with JXA. Just too buggy and there's zero speed benefit (might even be slower if you're not using the built in filtering methods.).
