# Login_SignUp_JavaScript
Login and sign up page using listener transition swapping login and sign up 


Project description-
Before we move to the actual code, I'd like to break down the things we're going to have in the component. This will help as it will make the code we write much clearer.

We have 4 smaller screens/boxes inside the main component (the .container):

1.The Sign In form
2.The Sign Up form
3.The Sign In overlay
4.The Sign Up overlay
Also, at one moment in time you can see either:

The Sign In form alongside the Sign Up overlay
The Sign Up form alongside the Sign In overlay
In the overlay panels we have some text and a button - by clicking it you will bring up the other combination of screens and vice-versa. Check the GIF above one more time to see what I mean.

The overlay animation - explained
This is where it might be a little trickier, but I'll do my best to explain so you can understand the logic behind it.

We have the following layers for the overlay component:

The overlay-container - this will display the visible area (more on this below) at a certain moment in time. It has a width of 50% of the total container's width.

The overlay - this div has a double width size (200%) so it's taking the full width of the main container. (200% * 50%= 100%. The 50% is from the .overlay-container above).

The overlay-panels - are the divs which are holding the actual content (the text and the button) we are seeing on the screen. They both have a position of absolute -> meaning that we can position them wherever we want in the .overlay component. One of the panels is positioned to the left and the other one is positioned to the right, both having a width of 50% of the .overlay component.

## Snap_shot below
<img src="/Screenshort/capture1.png" ><img src="/snapshot/Capture1.PNG" width="363" height="564">
<img src="/Screenshort/capture1.png"><img src="/snapshot/Capture2.PNG" width="363" height="564">
