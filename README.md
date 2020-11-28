# CtC-Extensions
Javascript Extensions for Cracking the Cryptic's Web App (Both the Legacy and their New App)

Currently only one extension. I hope to add more in the future as needed.

# Four Corner Color Extension

## Adds the ability to mark cells with a different (or same) color in each of the four corners.

### Instructions: (Must be done each time a puzzle page is loaded.)

1. Right click on a blank spot on the browser page and select "Inspect" or "Open Inspector".
2. Navigate to the console panel in the inspector window.
3. Make sure the correct frame is selected. For the new app, this will be the one labeled "top". The frame drop down is usually located at the top or bottom of the console tab. For the legacy app, the correct frame will be a set of characters with "cracking-the-cryptic.web.app" next to them.
4. Next copy the entire file and paste it into the console tab.
5. Hit the enter key on your keyboard.

If everything is successful, you will be greeted with a message saying the script has run. Hit okay and At this point you can close the inspector window. You should now see a button in a box below the standard controls. Click this button to active the extension.

This extension operates completely separate from the normal toolbar. It only interacts with the grid using its own methods. This means all the buttons on the regular toolbar including undo and redo have no effect regarding corner colors. This extension also does not have its own undo/redo feature at this time, so all actions are final with regard to corner colors.

This extension has been tested in Chrome and Edge. It may work in other browsers. Use at your own risk. I will try and keep it working, but I make no guarantees that it will work in the future, or with all past puzzles. I've tested it on a few. If there are any issues, feel free to submit them.

###    How to Use the Extension:
**Applying colors to corners of selected cells:**
1. Select any cells you want to affect in the grid.
2. Click on one or more of the four white squares in the new tool area. These are the corners of the selected cells that will be affected by your next action.
3. Click on one of the colors (in the new tool area) to apply that color to the selected corners.

**Removing colors from the corners of selected cells:**
1. Select any cells you want to affect in the grid.
2. Click on one or more of the four white squares in the new tool area. These are the corners of the selected cells that will be affected by your next action.
3. Click on delete (in the new tool area) to remove any color from the selected corners of the selected cells.

**Removing all corner colors from the entire grid at once:**
1. Click on Clear All Corner Colors button to clear all corner colors from the grid.
2. Click yes/continue/confirm to the prompt to remove them or cancel to leave them.

**Temporarily disabling the extension:**
1. Click on the Disable button to remove the extension. A button will remain to re-enable it.
2. Click yes/continue/confirm to remove the extension or cancel to leave it active.

**Completely remove the extension:**
1. Simply reload the webpage. Note that in the legacy app this will reset the puzzle.
    
**Notes:**
In some of the older puzzles, and especially in the legacy app, the sorting order can cause the corner squares to hide some puzzle elements. I have tried to ensure the best consistency between the new app and the legacy app, meaning that when possible, the corner colors will sit in front of the standard colors, behind (most) puzzle elements, behind the numbers, and behind the selected cells. You can mix corner square markings and the regular color markings in both the legacy app and the new app. Some blending of colors may occur, but for the most part I think I've stopped this from happening, or at least happening with most color combinations.

For these reasons, I recommend that if a cell needs multiple color options, use the extension only for that cell.

There are currently no keyboard shortcuts and you must click on each of the corner selection cells in the control area separately. To keep this extension simple, I did not have it make modifications to the underlying game code (although it does use a few functions from the original code). This extension does rely on certain assumptions about how the app creates and updates the puzzle grid, so any updates to the apps could break this extension, even without changes, future (or some past) puzzles may also break this extension. You can always try it, and if it fails, submit a bug report. 

There is no harm in trying the extension (beyond possible loss of progress during play, but unlikely as failure would more likely happen during installation) and if something does go wrong, simply reload the puzzle and the extension will be gone. During testing I noted that the new app will still save any puzzle marks between reloading the page (although all corner marks are not saved, again, separate code), but the legacy app does lose all progress when reloading.

The code to handle all this is pretty basic and the way I've implemented it lends well to being added to the new app permenantly should CtC ask their developer to add it to the app. The ony work left besides some formatting would be the keyboard inputs and the undo/redo integration. Maybe they will give them the go ahead.

**Enjoy!**
