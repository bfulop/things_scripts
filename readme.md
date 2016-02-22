# Scripts of Cultured Code Things

While Cultured Code is busy making the new version of Things, here are some scripts that will make it more aligned with a GTD workflow.

## Queue Tasks

This script will move all todos except the first open one to the Someday list. This will in turn make your tasks sequential.
 
### Motivation

 I've been using Things for at least 5 years, when I came across this article from 2009:
 
[Why Cultured Code’s “Things” app can’t do GTD](https://txfx.net/2009/02/05/why-cultured-codes-things-app-cant-do-gtd/)

Then it hit me. It's not my laziness stopping me advancing through my Next list. If you're really committed to using a tool to capture all your open loops, then your Next list in Things will normally contain between 30 and 150 items. That's just too much to scroll through. Yes, you can filter this list, but still you get a lot of "junk", tasks that you cannot act upon, since they depend on a previous task to be finished.
 
 ### How I use it
 
 I've set up a recurring task with [Lingon](https://www.peterborgapps.com/lingon/) to launch this script every 20 minutes. I have an old Mac Mini that's running all day and periodically cleans up my Next list.
 In the end, I have much cleaner list of my task:

![Screenshot of cleaned up Next list on iPhone](http://815b1b87b51011a7a029-623c55fb68acb92f1f433c6448bed244.r60.cf3.rackcdn.com/github/things-scripts/queued-tasks.jpg)

## Clean Things Today

Just a simple script to move all tasks from the Todays list to Next so each day I start with a fresh list. It works for me.

## Note on JXA vs. AppleScript

I'm a JavaScript guy. Still, I wouldn't recommend trying to script apps with JXA. Just too buggy and there's zero speed benefit (might even be slower if you're not using the built in filtering methods.).