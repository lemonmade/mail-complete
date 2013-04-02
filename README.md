# Mail Complete.scpt
## by Chris Sauvé of [pxldot](http://pxldot.com)


## Description
This script is run while in Mail.app. It finds the senders of all selected messages and then searches through your OmniFocus library for "Waiting For"-style contexts that contain the name of any of the senders. It will then offer you the option to see or complete any subset of the tasks associated with those contexts automatically. The script works best if you have a single "Waiting" context with sub-contexts for each individual person. If it does not find a "Waiting" context for the selected senders, it will offer to open its best guess of you "Waiting" perspective, if one exists.


## Runtime Options
- The script will ask if you would like to choose between completing or simply viewing the tasks found each time the script is run. You can change this at compile-time by editing the `askEachTime` property in the script.

- The script can either complete or focus on the selected tasks, and will prompt you as to which you would prefer on the first run of the script. You can change this at compile-time by editing the `actionWithSelectedTasks` property.

- The script can automatically archive messages that you use the script on, and will prompt you as to whether you would like this to happen. You can change this at compile-time by editing the `actionWithSelectedMessages` property.


## Runtime
- By default, only the available tasks in the "Waiting" contexts are shown. If you would like to show unavailable tasks as well, you can edit the `onlyShowAvailableTasks` property in the script.


## Installation
Download the most recent version of the script. Once you have downloaded the script, navigate to your Application script folder located at `~/Library/Scripts/Applications/Mail`. Apple hides the Library folder in Mac OS X 10.7 or later by default, so the easiest way to get to this folder is to select the menu item `Go > Go To Folder...` in Finder.app. You may have to manually create an Mail folder in the `~/Library/Scripts/Applications` directory if you do not have any previous scripts for Mail (you may have to create more of the folders in the directory; if you don't have an Applications folder or even a Scripts folder, you will have to create those as well).


## Using The Script
There are countless ways you can run the script. If you are a pro user, you likely know even more ways than I do: options like launching the script from FastScripts, Alfred, LaunchBar, or a Keyboard Maestro macro are all available to you.

Your other option is to run the script from Apple's AppleScript menu. If you don't have a little script icon near the clock in your Mac's menubar, you need to turn this on manually. Open AppleScript Editor.app from your `Applications > Utilities` folder. Go to AppleScript's preferences by selecting `AppleScript Editor > Preferences...` from the menubar. On the "General" pane, you should check the checkbox to "Show Script menu in menu bar". Now, when in Mail.app, select the new script menubar item and you will see the script at the bottom of the list, ready to be clicked and run.


## Version History
- **0.1.2** (January 22, 2013): Fancy icon

- **0.1.1** (Janauary 15, 2013): Added the ability to see tasks in their containing projects instead of automatically completing them

- **0.1** (January 15, 2013): Initial release


## License
Use it, change it, repackage it, whatever. Try not to take credit for my work.