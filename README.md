# StopGuardian
Exploit to disable GoGuardian tab limits.

Essentially, the exploit works by stopping GoGuardian in the process of closing tabs with a popup (The one that says "Leave site? Changes you made may not be saved."). If the user clicks "Cancel" on the popup, GoGuardian gives up completely on closing tabs while the tab is open. In the case that the tab is not open when the tab limit is initially enabled, there is still a way to get another tab open with a "spacer" bookmarklet (bookmarklet code: "javascript:onbeforeunload=()=>0"). The spacer is a tab that is not initially closed by GoGuardian, although if you open another tab or change the URL of the spacer tab GoGuardian will close the tab. Steps for using the spacer with the HTML file are below:

Step 1:
Open the HTML page, as well as enough other tabs to completely fill your tab limit.
Step 2:
Right click on the spacer bookmarklet and select "Open in new tab"
Step 3:
Use the dropdown to enable the HTML page, then drag it to the right of all of your tabs.
Step 4:
Try to open a new tab, and when it asks you if you want to close the HTML page, select "Cancel"
Step 5:
The exploit is now active. No matter where the HTML page is in your browser or how many tabs you have open, as long as the HTML page stays open, the tab limit will be disabled.
