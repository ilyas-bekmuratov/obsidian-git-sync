# main idea
interesting ways to close ads - a puzzle with a timer and score to save time and progress through a mini-story
## game loop
you smash through fake ads until you hit a real one, and you have time until it closes automatically to close it via a mini-puzzle products in the fake ads can be bought with in-game money at any time while the ad is open and if you have enough money, which also closes the ad. if you don't have enough money, you can pay with time in seconds because time=money and so on in a loop, closing, closing, closing, and then AHA GOT YOU SUCKER - real ad-mini boss

for closed ads, you get points and money, and there's a timer! constantly ticking.

each level gives you a certain amount of time - the remaining time after completing the level is saved as a record in story mode, it adds to the total for the level with the main boss every time you lose, you get an option to buy the "product" from the ad that defeated you, allowing you to start your next attempt

many unique levels with a storyline like swallowed food and choking? looking online for how not to die, but there's a lot of ads and you break through these ads hoping to survive and see the video instruction and you need to close all the ads in a minute there are different situations: need to perform CPR on a person, parachute not working, and stuff like that at the end of each level, a real reward - a promo from the real ad! a discount coupon at a local barbecue place, or bonuses in the Kaspi store for a purchase over 10k cool and feels a bit like a real reward

I would first make a few levels then mix them up and create an arcade mode in arcade mode - for closed ads, you get some extra time to keep going going further can get you cooler products (the quality affects the bonuses) from ads to start the next run on levels or in the arcade
## Ad Constructor
**item**
random unpurchased ad item
**type difficulty modifier**
add type and subtype have their own specifics to the mechanics of the ad, also determining their discount/markup
**quality**
1, 2, 3, 4, 5 ... higher quality means better bonus. Calculated as base quality for the level + ad type quality modifier
**price** = base item cost x ad type difficulty modifier x ad quality x discount/markup
**size, frame, shape** small/big, rectangle
buttons, sliders, input fields buy close
**Animations**

**closing effect** via x

**purchase effects**

**sound**

**background**

**Trigger appearance**

**Appearance location** 

**mechanics** (Discount/Markup, Closing/ Purchase, Closing queue, timing and limits, etc additional)
## Ad items
### temporary bonuses
- *0.1* hammer (building materials)
    - breaks ad screen if tapped in the rhythm of music with a fast tempo, ends as soon as you tap off-beat or when nails run out
    - higher quality - more nails
- gym membership
    - you need to tear (move fingers) the ad in different directions at a slow tempo - slower and slower - ends if tearing is not finished
    - higher quality - delay onset
- sword (knife, chainsaw, something sharp)
    - momentarily shows how to slice the ad in half at a certain angle, and you need to swipe along this line, ends if you slice wrong or the buff timer runs out
    - higher quality - more time to slice
- *0.1* meal plans/proteins/vitamins
    - make all the x buttons bigger for a period of time
    - higher quality - more time
- VPN
    - switches to an alternative ad version - changes visual content and some ad effects while active, blocks part of the ad passively like "not available in your country"
    - higher quality - more time
### One-time Purchases
- Pre-order
    - Offers to buy something from another random ad several levels higher with a markup.
    - Higher ad level means lower markup and higher purchased ad level.
- *0.1* Transport/Bus/Car/Ship/Plane, etc.
    - Can be bought at the start to begin further in the level.
    - Picking it up in the level just moves you further.
    - Higher quality moves you further, up to the boss.
- *0.1* Casino/Bets/Slots/Roulette/Wheel of Fortune
    - Start mini-games with a reward - money + return of the bet.
    - Initial bet to start the game is visible in the ad window, capped by the money on hand.
    - Higher ad level means higher bets.
    - *0.1* Roulette/Wheel of Fortune
        - Gives a random guaranteed reward from 0 to triple the bet.
    - Slots
        - Two buttons - white, black.
        - After a short animation, the bet either burns out or gives money equal to the bet depending on whether you guessed correctly.
    - Bets
        - Bet on the remaining time after completing the level with different coefficients.
        - Win to take the prize.
    - Casino
        - Blackjack with open cards, durak, poker, etc.
        - Only two buttons - raise, call.
        - Raise doubles the bet and potential winnings, capped by the money on hand.
        - Call continues.
        - The final card game is played out, and the player gets a prize for winning.
- *0.1* Green Products/Solar Panels, etc.
    - Gives a discount on the next few purchases in the run.
    - Higher quality means the discount applies to more purchases.
- *0.1* Ad Blocker
    - Blocks pop-up ads if you misclick and consumes itself.
    - Higher quality blocks more ads.
- *0.1* Home Appliances, Pet/Child/Elderly Care
    - Adds time by freeing up from household chores.
    - Higher quality means more time.
- Business Services and Personal Growth Consultations
    - Costs money to enable
    - at the end of the level, if enabled, gives an option to spend all the time saved to gain extra money
    - Higher quality means more money.
- *0.1* Loans and Credits
    - Instantly gives money.
    - Deducts the loan amount from the total money after completing the level + interest.
    - Higher quality means lower interest.
- Gifts
    - "Wraps" and sends money to another player from the friend list.
    - Offers to invite a friend if there are no friends.
    - Gifts are received in the main menu.
    - Higher quality means a higher gift multiplier, up to 5x.
- *0.1* Legal Agency
    - Gives a 50% chance to recover part of the money spent on the entire run.
    - Higher quality means higher compensation %.
    - Appears at the end of the game.
- Online Contest/Seasonal Quiz
    - Buys a participation ticket.
    - Requires verified email.
    - Higher level means harder questions and bigger rewards.
    - Top players by correct answers are in the season leaderboard.
    - At the end of the season - a quiz for perks.
    - Top 1 player?
    - All top 10 players finished for?
    - Average number of purchases?
- Top Player/Friend Activities
    - Opening the notification gives a one-time discount on the same ad product.
    - Completing a level gives bonus time to a friend on the same level.
- Safekeeping/containers/storages
	- saves current game progress and exits
	- can be purchased in the pause menu
	- higher quality gives an option to buy "another player's save file" instead of yours for extra money
	- the save file can be launched the next time the game turns on
- Daily Bonus
    - Gives a choice between (+10 sec for boss a day or a discount on the type of product for the whole day).
- *0.1* Dating Site/Social Network
    - Adds game complexity for this level by opening more ads but gives an additional reward.
    - Higher quality means more bonus money and time.
### Visual Improvements
- *0.1* Event Organization
    - Description text says "why do you need this?"
    - Adds fireworks and fun stuff on the boss victory screen.
    - Higher quality means more fireworks and fun stuff.
    - Buying higher quality event organization opens a boss-only mode, after which purchases of this bonus give time.
- Furniture/Cabinets/Shelves
    - In the main menu, there's a bunch of purchases - an endless mountain of bought items organized differently.
    - Higher quality means a cooler look.
    - Design can be chosen in the main menu.
    - Buying all designs makes the bonus a waste of money - gives time.
- Property Ownership
    - Design of the main menu.
    - Higher quality means a cooler look.
    - Design can be chosen in the main menu.
    - Buying all designs makes the bonus a waste of money - gives time.
- *0.1* Online Courses/Education
    - Opens a scheme for passing one of the bosses or an explanation of one of the bonuses or a mini article about games and ads - can be read in the main menu.
    - Higher quality means more chances that the info will be about bosses.
    - Buying all schemes makes the bonus a waste of money - gives time.
- *0.1* Clothing/Jewelry/Cosmetics/Medicine
    - Opens a new skin for the character.
    - Higher quality means more stylish skins.
    - Buying all skins makes the bonus a waste of money - gives time.
- *0.1* Equipment/Phones/Computers
    - Opens new ad frames.
    - Higher quality means more stylish frames.
    - Buying all frames makes the bonus a waste of money - gives time.
- *0.1* Stat Tracker bar
    - Each one is bought separately.
    - a progress bar/pie chart shown in the main menu.
    - Until the end of the season, it shows statistics:
        - How much time is spent on the boss
        - How many attempts on each level
        - How many purchases were made
- Charity
	- donations in coins
	- all the donations in coins are converted and actually donated to charity by the dev
	- higher quality means more bonus time for the current level
	- total amount of donated money is proudly displayed in the main menu as a stat tracker
	- also changes the color of their name tag
- *0.1* Membership in the Winners Club
    - Available only on the boss victory screen.
    - Records this result - time - points - money - purchases in the player table in the main menu in the boss section.
    - The top players spent the least time and purchases, earning the most points and money for the run and defeating the boss.
    - Only verified accounts.
- Streaming Services
    - Opens new soundtracks - you can choose what to listen to during the game.
    - Higher quality means cooler soundtracks.
    - Buying all soundtracks makes the bonus a waste of money - gives time.
### Permanent Bonuses
- Trip to Warm Countries, Concerts/Stand-Up/Shows/Movies
    - Saves progress, permanently opening this level in the starting point selection.
    - Further levels mean higher quality and cost.
    - Appears only on the boss victory screen.
- Insurance/Warranty
    - Gives a chance that temporary bonuses return money if completed within the warranty timer.
    - Higher quality means a longer warranty timer.
- Organizer/Shopping List/Duty Tracker
    - Daily tasks.
    - +money for completion.
- Bank Cards
    - Different color wallets for money for different banks.
    - Different banks have different discounts on various products and give different daily bonuses.
    - First registration with the bank.
- Crypto Investments
    - Buy crypto shares for your "electronic wallet" - the price varies daily, and you can convert them back to money to spend if you wait for the price to rise.
    - Higher quality means cheaper purchase price.
    - The amount of crypto investments is visible in the main menu along with their total value at the moment.
- Magazine Subscription
    - Appears as a pop-up message every day.
    - The code is valid only for that day.
    - Gives discount codes on some bonuses during the run.
    - Higher level means longer code and bigger discount.
    - The code must be entered each time a new ad opens.
- *0.1* Sponsorship Contract
    - Opens after defeating the boss.
    - Signed in the main menu.
    - After signing, a sponsorship banner appears in the game, blocking part of the screen.
    - Multiplies the amount of money and points for each closed ad while the banner is active.
    - Can be turned off in the main menu.
- Loyalty Card
    - Seasonal subscription.
    - +1 second for the boss permanently.
    - +money.
    - higher tier for higher price
    - Expires each season with a new boss.
- Religious Organization/Ritual Services
    - Bought only for time and who knows what it gives.
    - Actually saves time in a "bank," which will give bonus time on failure equal to half the spent time.
    - Higher quality means more return time on failure.
    - Half of the spent time goes to the karma bank - the karma bank gives extra time (max 10 sec) at the start of the next run.

## [37 типов всплывающих окон](https://www.internet-technologies.ru/articles/37-tipov-vsplyvayuschih-okon.html)
##### Basic Advertisement
- Lightbox pop-up window
    - Yes/No - close
    - Yes/Yes - close
    - Yes - close
- Fullscreen
- Floating panel
- On click
##### Informational Notification
- Page redirection
- Adblock bypass
- Login - registration
- Survey form
- Lead magnet - free item for input
- Webinar registration
- Pre-order
- Coupon code for info - discount for email input
- Email request
- Phone request
##### Product Recommendation
- Based on purchased ads
- Upsell - additional offer post-purchase
- Downsell - offer after purchase screen close
- Tripwire - downsell after upsell rejection
- Wait, don't go - offers abandoned items at a discount
- Countdown timer
##### Triggers - Any Action
- Close
- Purchase
- Input field
- Scroll
- Viewing time
- Location-based
- Cookie-based
- Re-engagement - after breaks
- Seasonal
- Time of year
## ideas for puzzles:
press x 
in the correct order 
hold x 
press a small x 
find the real x among fakes 
trace the outline of x 
unroll a banner ad to close with x button 
fold (to the edge of the screen) or swipe (to the side) a banner ad to close it 
mute and wait for the ad to close 
scroll to the end and close 
trick - x moves 
enlarge x to press 
watch or fast forward video to the end to press x

reopen the game 
close the screen 
"turn off internet" in places 
rotate the phone 
shake the phone 
mute the ad 
take a screenshot 
auto-fill passwords - find the correct password among autofill options - at first 3, but with each registration more, each organization has its password requirements 
same with logins and with phone number if registered email registration - any email can be registered, but verified emails get more bonuses

enter login and password wheel of fortune
find differences between pictures mark pictures for the presence of objects rotate picture to the correct position
simple arithmetic move numbers together move a stick to form the correct equation
save the princess from lava and get money by moving a stick distribute resources correctly so characters in the ad don't freeze

5-10 seconds minimum viewing and closes itself more complex mini-bosses need to be closed after viewing, otherwise, it reopens can't be closed until time runs out but you can close other ads in parallel

### references
- [iq dungeon](https://play.google.com/store/apps/details?id=com.Hirameku.IQDungeon)
- сапёр
	- 6 by 6 with 6 mines
	- higher tier = bigger +1
- судоку
	- 4 missing
	- higher tier = +2 missing
- angry birds
	- destroy a building
	- higher tier = taller building
- shower crocodile
	- draw a line with a finger for the water to flow
	- higher tier = harder level
- flappy bird
	- tap in timing to avoid obstacles
	- higher tier = +1 obstacle to go
- pinball
	- get the ball where it needs to be
	- higher tier = +1 obstacle
- fighter plane
	- defeat all enemies
	- higher tier = more enemies
- Tetris
- [2048](https://www.2048.org)
- [pop ads closing sim](https://donian.itch.io/1b-ads)
- [osu](https://osu.ppy.sh)
- [хелтакер](https://store.steampowered.com/app/1289310/Helltaker/)
- [yeah you want those games](https://store.steampowered.com/app/2348100/EY_QUIERES_JUGAR_A_ESOS_JUEGOS_VERDAD_PUES_AQU_LOS_TIENES_VEAMOS_CMO_LOS_COMPLETAS/?l=spanish)
- [tiny room stories town mystery](https://play.google.com/store/apps/details?id=com.kiarygames.tinyroom)
- [как достать соседа](https://store.steampowered.com/app/1283190/Neighbours_back_From_Hell/?curator_clanid=32976304)
- [outer wilds](https://store.steampowered.com/app/753640/Outer_Wilds/)

- [brain code: hard puzzle game](https://play.google.com/store/apps/details?id=com.kk.braincode)
- [not not a brain buster](https://www.xbox.com/en-gb/games/store/not-not---a-brain-buster/9P5V8KS3B9SW)
- [baba is you](https://store.steampowered.com/app/736260/Baba_Is_You/)
- [gorogoa](https://play.google.com/store/apps/details?id=unity.Annapurna.Gorogoa)
- [there is no game: wrong dimension](https://store.steampowered.com/app/1240210/There_Is_No_Game_Wrong_Dimension/)
- [human resource machine](https://store.steampowered.com/app/375820/Human_Resource_Machine/)
- [bad banker](https://play.google.com/store/apps/details?id=com.sirnic.badbanker)
- [puzzle quest](https://store.steampowered.com/app/12500/PuzzleQuest_Challenge_of_the_Warlords/)
- [world of goo](https://store.steampowered.com/app/22000/World_of_Goo/)
## bosses
30 seconds minimum to close when reaching bosses, the timer automatically sets to 30 seconds if it is less if more than 30 seconds, no extra time is added
#### LATER
miss "all our lines are busy right now, call us later"
#### PROVIDER
local internet provider
#### Gates, Zuker-musky-jobgates
ultra-high net worth individual, possibly lizard-man
#### Вова
12yo Russian genius kid
#### xxxLANAxxx
internet "model"
#### AdVersary
the CEO of Most Evil Corporation (MEC), first of the Bright Day Robbery Group (BDRG), that has drowned the internet landscape in advertisement and is profiteering from immense ad-revenue. - first big boss
