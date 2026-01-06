---
Status: In progress
tags:
  - projects
---
Using a SQLite database with tables for each region, holding 15 columns picking the winning team for each game.

  

Main table will hold, username, bracket ID, score, (possibly number of that brackets submitted, allowing a person to play that same bracket twice)

  

BracketID could get be the SHA1 (preferably SHA1 over MD5) of bracket data

  

  

Remember to close db connection

  

Account for SQL injection attacks

  

Add a search page to search the amount of points associated with a username or bracket ID (pick one)

probably username

  

Can split the page into subpages where you can work on one region at a time, reducing the amount of overhead needed, and allowing the landing page to be the first thing people see

Possibly use PayPal data-client-tokens to use that as an identifying factor for the transaction

Look at the on Approve thing for the PayPal API

  

  

Use division:seed notation for string building

  

Keep in mind mobile devices

  

for table management, associate a username with their Bracket ID(s) and have tables that are used to associate that bracket ID with its respective picks (this will eliminate duplicate brackets that are shared between users)

  

Have near checkout a visual to see what your payout would be if you put in your current amount of money assuming your bracket alongside people with the same bracket

ex. Pot = $200

If you put in $3 and there are $17 worth of people with the same bracket.

You would get 3/20 * 200

  

## Google Integration Notes

You have to update the info.plist in the ios folder for it to work on the ios device, along with updating the GoogleServices-Info.plist and googleSignIn.configure() function. So 3 locations