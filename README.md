# DevMethod
YAME (yet another method explorer) for 4D databases.
DevMethod is very light weight, simple to use and provides one feature I haven't seen in any of the others: you can toggle method attributes from the method list!

Written in 4D v15.2. Not compatible with previous versions but probably could be tweaked to work with them.

## Installation
Download the repo to your computer.
  1. Compile it for use as a Component
  2. Copy the methods to a database

## How to use it
Call DEV_SHOW_methodExplorer.

![DevMethod screenshot](https://github.com/KirkBrooks/DevMethod/blob/master/images/ss1.png)

The dialog opens showing a listbox of the methods in the host database. The initial view is hierarchical. If you have named your methods so that the beginning of the method name is a module followed by an underscore (eg. DEV_SHOW_methodExplorer) the characters in front of the first underscore are used to group methods.

The listbox columns are the group, method name, modification date and check boxes for the various method attributes.

**Clicking the checkboxes changes the method attribute immediately!**

You can toggle the listbox hierarchy with the Toggle Hier button. Turning off the hierarchy is useful if you wanted to sort your methods by modification date.

![DevMethod screenshot](https://github.com/KirkBrooks/DevMethod/blob/master/images/ss2.png)

Double click a method to open it for editing.

###Drag and drop###
When you drag a method the entire text of the method is copied.

You can drag between 2 copies of 4D. With the DevMethod dialog displayed in both databases you can copy methods from one to the DevMethod dialog in the other. If a method already exists in the target you are prompted to accept the change.

## Why another method explorer?
I like being able to see my methods grouped by 'module'. I also really wanted to be able to see and edit the method attributes *en masse* rather than having to open each one. This is especially useful when working with component databases - how many times have you had to recompile something because you neglected to set the 'share' attribute?

Finally I wanted an easy way to see methods sorted by date and simplify the process of updating one database to another. For instance when adding changes from a development copy to a production copy.
