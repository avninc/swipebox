# Swipebox
Modified for AVN based on Swipebox v1.4.4

## Description

This file has been modified to support the abiltiy to use the share slider provided by addthis
 on mobile devices, previsouly this plugin will bind the touch* events on the body element this
 causes the add this share buttons to return the following warning:
 "Ignored attempt to cancel a touchstart event with cancelable=false, for example because scrolling is in progress and cannot be interrupted."
 since the buttons relay on click event and on mobile devices the entire body element has the touch* events binded to it
 it prevents the addthis widget (or any other event for that matter when the swipebox is open) to work properly
 this was changed to bind the touch* events for mobile devices on the #swipebox-slider element rather than the body.
 
