# Debug log



### CC-01 — "The search suggestions are behind everything"

**Reproduced:** When I opened the website i clicked on the search ha not all result were shown and using developer tools i confirmed that there is something behind the filters

**Cause:** There wasn't any margin or padding on the top because of it the items weren't completely shown

**Fix:** I just added margin on the top 45px;

**Checked:** Checked now it shows the above item as well

**Time:** about 30 mins I first didn't get what the query meant like i thought it is saying the search is above the menu then i get it when i checked through the ddeveloper tools that one is behind the nav bar


## CC-02 — "<The dish name and price color problem on the dark them visiblity was not good>"

**Reproduced:** In the website when i clicked on the dark the color was darkish(not remember)

**Cause:** Wasn't setuped with data theme

**Fix:**I setuped with data-theme present in the html 

**Checked:**Checked the text color is now changing

**Time:**Around 2 hour i didn't get what is causing the problem changed the approach 3 times


## CC-06 — "<I ordered more than they had>"

**Reproduced:** In the website i first checked the counter where there is a small quantity the i placed an order of more than the stock and the order got placed

**Cause:** In the validateline item.qty is compared to 10 and not compared with the stock, no. if it is integer, less than 1 and same in reservestock there is nothing done with item.qty and only the stock decrease

**Fix:** "I just pushed an error if stock is less than item then the sentence you want to gave to the customer is pushed to error and in order.routes.js I just changed the sentence which was displayed to another so customer get what canteen is short on"

**Checked:**Checked now it is displaing the error and the error is correct and is displayed in the last part

**Time:** About 45 mins


## CC-08 — "<An old coupon still works>"

**Reproduced:** "FRESHERS24 was 2024 offer and it expired ages ago but when i write FRESHERS24 in the coupon box it got applied and the order was made

**Cause:** It was with display but no such thing with the data

**Fix:** " I just copied from the coupons.routes.js and change the < to > and put it in the if"

**Checked:**Checked by applying FRESHERS 24

**Time:** About 20 mins


## CC-10 — "<Sorting by price is backwards>"

**Reproduced:** > When i opened the website i used the filter section then used sort price low to high and it gave me high to low instead

**Cause:** The desc was asc and asc was desc

**Fix:** " I changed the desc with asc and asc with desc"

**Checked:**Checked by using the price low to high ang high to low confirming both

**Time:** About 5 mins


## CC-07 — "<Cancelling makes it worse>"

**Reproduced:** I placed an order but i canceled it then i checked the counter the counter had less value then the original

**Cause:** While when we ordered something it deducts that much amount from the stock but when we canceled it then also deducts that much from the stock that makes it negative and stock cannot get negative so I can eat it not a problem how much deduct but atleast it should left something for me to eat so due to that

**Fix:** " I just change the minus sign to + sign in the release stock function"

**Checked:**Checked by using veg momos

**Time:** About 5 mins


## CC-03 — "<The menu is wider than my phone>"

**Reproduced:** When i opened the website in the developer tools and set to the px greater than 480px and less than 717px the dish was outside the space i checked it by checking the outline of the body(Don't remenber correctly) 

**Cause:** 1fr was applied in the menu-grid in the css causing cut of the screen

**Fix:** " I changed the 1 fr to minmax(0,1fr)"

**Checked:** I checked in the developer tools it is showing correect

**Time:** More than 1 hour I didn't get it so i understand with a 2nd year senior


## CC-04 — "<The buttons don't work on my tablet>"

**Reproduced:** When i tried clicking add to cart button in 800px there was nothing added to the cart while the buttons in filters were working

**Cause:** There was media thing placed on the page for 761 - 900 that was not any useful also creating the problem
.dish-card::after was an empty box covering the bottom 58px of the card. That is exactly where the Add to Cart button sits, and it is same with .img-wrap do sit at the save button with z=1

**Fix:** " I just deleted that thing"

**Checked:** I checked it by adding the dishes in the cart and the button is working

**Time:** Around 3 mins


## CC-05 — "<The category bar scrolls away on my phone>"

**Reproduced:** In the 400px the filter bar did't stick when i checked it in the developer tools

**Cause:** First there was a problem that was due to z-idex it was over shadowed by header which cause the problem in all the resolution and also there was overflow there in filter so when the overflow is there and there is something another than visible then it causes the same work in y direction 

**Fix:** " I added the top 92.1668px as it is the height of the header and removed the overflow-x : hidden"

**Checked:** Checked on different ratio 400px 480px 717px 1000px

**Time:** Around 20 mins


## CC-09 — "<The menu shows more dishes than it should>"

**Reproduced:** > "On smaller screens, the category and filter bar scrolls away instead of
> staying visible at the top while I scroll down through the menu dishes."

**Cause:** In the function paginate() slices the list into items but the return object has items: list that make the part of paginate(to slice the list) the hardwork the function did
list. menu.routes.js sends paged.items as dishes, so the whole menu went
out on every page.

**Fix:** " I just removed the list tag in the return

**Checked:** I checked the website the error which was shown AC-02 check down isn't coming

**Time:** Around 20 mins


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

## AC-03 — "<To get the new stock left reload have to be done>"

**Reproduced:** > When we place an order the amount left in the stock doest show up in menu we have to reload

**Cause:** 

**Fix:** " 

**Checked:**

**Time:**