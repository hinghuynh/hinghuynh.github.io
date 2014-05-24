What are the differences between relative, absolute, and fixed positioning?

First Let's Start with Relative Position

You want to use relative position when you want to adjust a specific object's position without affecting the positon of any of the other objects. For instance, say I use "top:100px;". This would move the object down 100 pixels from the top of it's current position, but doesn't move any other objects down 100 pixels. For the purposes of illustrating this point, I will be moving around a happy face icon.

![alt tag](/unit1_projects/images/relative1.png?raw=true) 
![alt tag](/unit1_projects/images/relative2.png?raw=true)
 
Okay, so What's Absolute Position used for?

With position absolute, your object overrides starting position which starts within the position of your element. For instance if I used "top:0px;", "left:0px;", this would put the object at the most top left of the page overriding the default position of the most top left position of an element, like the header. Absolute overrides to position relative to the parent element. This is shown in the example to the left below. To change parent element to another element instead of the entire page, add "position: relative;" to another nearby element. This is shown in the example to the right below. I set the content element position to relative to get my icon move with respect to the confines of the content borders.

![alt tag](/unit1_projects/images/absolute1.png?raw=true) 
![alt tag](/unit1_projects/images/absolute2.png?raw=true)
   

Why do we need Fixed Position then?

Absolute and Fixed are similar in that is overrides to be relative to parent position, but the key difference is that fixed will stay in the same position on the screen, even after scrolling/resizing. Whereas absolute will stay in the same place on the page, and move up as you scroll down. For this example I placed the the icon using "bottom:0px;", "right:0px;" with a fixed position. Notice what happens when I scrolled.

![alt tag](/unit1_projects/images/fixed1.png?raw=true) 
![alt tag](/unit1_projects/images/fixed2.png?raw=true)