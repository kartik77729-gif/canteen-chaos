# Debug log

Your notes. One entry per bug you fixed, using the template below.

This file is read as carefully as your code. A correct fix you cannot
explain counts for little; a bug you could not fix but investigated
honestly still counts for something.

Delete the example before you submit.



## Example — delete this

### CC-01 — "The search suggestions are behind everything"

**Reproduced:** > "I start typing a dish name and the list of suggestions comes up, but
> it's stuck behind the rest of the page. I can only click the very top
> bit of it. The rest I can see, sort of, but clicking does nothing."

**Cause:** There wasn't any margin or padding on the top because of it the items weren't completely shown

**Fix:** I just added margin on the top 45px;

**Checked:** Checked now it shows the above item as well

**Time:** about 30 mins I first didn't get what the query meant like i thought it is saying the search is above the menu then i get it when i checked through the ddeveloper tools that one is behind the nav bar



## CC-02 — "<The dish name and price color problem on the dark them visiblity was not good>"

**Reproduced:** > "I switched the site to dark mode and now the dish names and the prices
> are almost invisible. The grey line under the name is fine, it's just
> the name and the price."

**Cause:** Wasn't setuped with data theme

**Fix:**I setuped with data-theme present in the html 

**Checked:**Checked the text color is now changing

**Time:**Around 2 hour i didn't get what is causing the problem changed the approach 5 times



## Could not fix

For anything you investigated but did not solve. Say what you tried and
where you got to. This is worth marks — leaving it blank when you got
stuck is not.

### CC-0X — "<the complaint>"

**What I tried:**

**Where I got to:**

**What I would try next:**



## Extra credit

Anything not on the bug log: a problem you found yourself, a test you
wrote, or a fix you are unsure about. Same format, plus one line on how
you noticed it.

MC-01 : The problem is with veg and non veg it automatically doesn't change
    You have to do something then it changes in the first screen which you see
    in the all section else in every other it works