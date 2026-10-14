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

**Time:**Around 2 hour i didn't get what is causing the problem changed the approach 3 times

## CC-06 — "<I ordered more than they had>"

**Reproduced:** > "The counter says only 2 samosas were left but it let me order 5, and
> the order went through fine. When I got there they only had 2?"

**Cause:** Error wasn't there of this thing

**Fix:** "in the validateline item.qty is compared to 10 and not compared with the stock, no., less than 1 and same in reservestock there is nothing done with item.qty and only the stock decrease so i just pushed an error if stock is less than item then the sentence you want to gave to the customer is pushed to error and in order.routes.js I just changed the sentence which was displayed to another so customer get what canteen is short on"

**Checked:**Checked now it is displaing the error and the error is correct and is displayed in the last part

**Time:** About 45 mins

## CC-08 — "<An old coupon still works>"

**Reproduced:** > "FRESHERS24 was last year's offer and it expired ages ago. Someone used
> it yesterday and got the discount?!!"

**Cause:** It was with display but no such thing with the data

**Fix:** " I just copied from the coupons.routes.js and change the < to > and put it in the if"

**Checked:**Checked by applying FRESHERS 24

**Time:** About 20 mins

## CC-10 — "<Sorting by price is backwards>"

**Reproduced:** > "I picked 'price: low to high' and the most expensive things came first.
> I tried the other option and that gave me the cheap ones. Both are the
> wrong way round."

**Cause:** The desc was asc and asc was desc

**Fix:** " I changed the desc with asc and asc with desc"

**Checked:**Checked by using the price low to high ang high to low confirming both

**Time:** About 5 mins

## Could not fix

For anything you investigated but did not solve. Say what you tried and
where you got to. This is worth marks — leaving it blank when you got
stuck is not.

### CC-0X — "<the>"

**What I tried:**

**Where I got to:**

**What I would try next:**



## Extra credit

Anything not on the bug log: a problem you found yourself, a test you
wrote, or a fix you are unsure about. Same format, plus one line on how
you noticed it.

## AC-03 — "<The time coupon can be used doesn't decrease>"

**Reproduced:** > time coupon can be used doesn't decrease

**Cause:** It was use.left = use.left

**Fix:** " I just put use.left = use.left -1

**Checked:**Checked by applying BYTE10

**Time:** About 10 mins

**Notice** I was just interacting with the website

AC-01 : The problem is with veg and non veg it automatically doesn't change
    You have to do something then it changes in the first screen which you see
    in the all section else in every other it works

AC-02 : The problem is the same dishes keep repeating 9 times

## AC-04 — There is a thing like when i have to do sorting i have to go to another page then go to another to get the page sorted but when i open the developer tools then do sorting nothing like that happen it instantly sort the page no need to go like all to lunch then to all like that. 