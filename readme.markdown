LGBT-Themed Flair for Reddit communities
========================================

This project contains 15 flags and the CSS necessary to implement them 
as flair for a subreddit, as we have done over at [/r/ainbow](http://www.reddit.com/r/ainbow/).

Instructions
------------

Steps 1-2 will happen on this page: 
http://www.reddit.com/r/yoursubreddit/about/stylesheet

Steps 3-4 will happen on this page: 
http://www.reddit.com/r/yoursubreddit/about/flair/

1. Under the "images" section, upload each of the PNG's in this folder. 
   Reddit will suggest a name in the "new image name" box. Keep that 
   name, or you'll have to change the CSS a bit. 
2. Paste the CSS from "flags.css" into the bottom of your stylesheet.
3. Go to the flair page mentioned above, and click on the "Edit Flair
   Templates" tab. There are 16 CSS classes to enter by default; all 
   will have an empty "flair text" box, and "user can edit?" unchecked. 
   You can use any order, and that will be the order they appear in the 
   sidebar flair picker. The class names are listed below. 
4. (optional) Check off the "allow users to assign their own flair" box
   atop the page if you want people to be able to select their own flags. 
   
Congratulations, you're done!
   
CSS Class Names
---------------

These are the CSS classes you will add to the flair template page. For 
reference, this is /r/ainbow's order as of March 2012: 

 * ainbow
 * trans
 * bi
 * ace
 * genderqueer
 * pan
 * ally
 * none
 * trans-ainbow
 * trans-pan
 * trans-bi
 * trans-ace
 * genderqueer-ainbow
 * genderqueer-pan
 * genderqueer-bi
 * genderqueer-ace

Notes
-----

"None" at position 8 looks good, as it puts all the blended flags
into a second column. The CSS class names are invisible to the end user. 

Thanks to kkress, the flair now supports hover text! If you want to add 
an explanation of the flag or custom text alongside the flag, put it
in the "Flair Text" box. This is entirely optional. 

Blended flags were designed by reddit user WTFcannuck; thanks so much! 

If you have any questions or issues, message joeycastillo on reddit. 