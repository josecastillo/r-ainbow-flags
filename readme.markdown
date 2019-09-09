LGBT-Themed Flair for Reddit communities
========================================

This project contains 15 flags and the CSS necessary to implement them 
as flair for a subreddit, as we have done over at [/r/ainbow](http://www.reddit.com/r/ainbow/).
Thanks to the current reddit split, part of this has to be done in old reddit, and part in new. 
To assist in this links used will start with old. and new. respectively to link to the appropriate versions of reddit.

Instructions for old reddit
------------

Steps 1-2 will happen on this page: 
http://old.reddit.com/r/yoursubreddit/about/stylesheet


1. Under the "images" section, upload each of the PNG's in this folder. 
   Reddit will suggest a name in the "new image name" box. Keep that 
   name, or you'll have to change the CSS a bit. 
2. Paste the CSS from "flags.css" into the bottom of your stylesheet. 


Instructions for new reddit
------------
Step 1 will happen on this page:
https://new.reddit.com/r/yoursubreddit/about/emojis

Steps 2-5 will happen on this page:
https://new.reddit.com/r/yoursubreddit/about/userflair

1. Add an emojii for each of the PNGs in emote-images. Name them whatever feels sensible, the defaults are a good option. You are free to decide on the other options whichever suits your subreddit best.
2.  Go to the flair page mentioned above, and for each flair, select Add Flair.
3. Under flair text, give the flair some descriptive text, and either start or end with the emoji flag
4. under CSS class select the class from the below list appropriate for the flag.
5. select User can edit, then save flair

CSS Class Names
---------------

These are the CSS classes you will add to the flair template page. For 
reference, this is /r/ainbow's order as of September 2019: 

 * ainbow
 * trans
 * bi
 * ace
 * lesbian
 * genderqueer
 * pan
 * ally
 * noflag
 * trans-ainbow
 * trans-pan
 * trans-bi
 * trans-ace
 * trans-lesbian
 * genderqueer-ainbow
 * genderqueer-pan
 * genderqueer-bi
 * genderqueer-ace

Notes
-----

The CSS class names are invisible to the end user. 

Position 8 in the template list used to be the 'none' class, which removed 
the flag. Now that reddit has a 'Remove Flair' option, we've repurposed 
this positon for the 'noflag' class, which allows for freeform text in the 
standard style of reddit flair. Position 8 is ideal for this, as column 1 
contains seven flags and column two contains eight; the noflag template 
nicely fills out column one. 

The original implementation supported custom text as hover text rather 
than static text. We later decided that showing text alongside the flag at 
all times was preferable, and as of the latest update, hover text is 
incompatible with the new noflag template. Nonetheless: if you want the old 
hover text style, replace the span.flair rule with the following: 

	span.flair
	{
	   text-indent: -30000px;
	}
	
	span.flair:hover
	{ 
	   text-indent: 22px;
	   width: auto;
	   min-width: 15px;
	   padding-right: 3px;
	}

Acknowledgments
---------------

Custom text was initially implemented by reddit user kkress, and the 
blended flags were conceived and designed by WTFcannuck. RES NightMode
optimizations, lesbian flag, and alterations for new reddit were added by nekosune. Thanks so much to you all! 

If you have any questions or issues, message joeycastillo on reddit. 