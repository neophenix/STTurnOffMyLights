# Turn Off My Lights
SmartApp that checks once a minute if lights should be off based on motion

The built in smart lights app is pretty horrible at turning off lights based on lack of motion.
If there is any hiccup when it tries, it never tries again.  This is especially apparent when using
options that cause the app to run in the cloud instead of locally (or against cloud based light APIs,
 like LIFX).

This app runs once a minute, checks for the last motion from 1 - N sensors, and if the last time motion
was recorded was >= the minutes you specify, turns off the selected lights.
