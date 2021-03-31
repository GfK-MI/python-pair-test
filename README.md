Hello there!  

Imagine you just joined a team as the only Senior Developer. 

The codebase already supports several use cases, but the business wants you to add another feature.  
They want the code to be able to handle a new type of items, called "Conjured" (they have the word "conjured" in the name).  

Your task is to:
- **add this new feature to our system**  
- **maintain the current functionality - all the existing use cases should be supported**  
- **add any improvements to the existing code you deem necessary**  


Here are some tips about our system:  

- All items have a `sell_in` value which denotes the number of days we have to sell the item (similar to a "best before" date).  
- All items have a `quality` value which denotes how valuable the item is.
- **At the end of each day our system lowers both `sell_in` and `quality` for every item**.

Pretty simple, right? Well this is where it gets interesting. Here are some additional facts from your helpful Product Manager:

- Once the sell by date has passed, `quality` degrades twice as fast.
- The `quality` of an item is never negative.
- **"Aged Brie"** actually increases in `quality` the older it gets.
- The `quality` of an item is never more than `50`.
- **"Sulfuras"**, being a legendary item, never has to be sold, nor does it decrease in `Quality`.

We have recently signed a supplier of conjured items. This requires an update to our system:

- **"Conjured"** items degrade in `2uality` twice as fast as normal items.

Feel free to make any changes to the `update_quality` method and add any new code as long as everything
still works correctly. 

However, **do not alter the `Item` class or `Items` property**.  
Also, you can make the `UpdateQuality` method and `Items` property static if you like, we'll cover
for you.  
