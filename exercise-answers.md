# Exercise Answers

## E 2.0 - Sidequest

Why is first-bid pricing not DSIC? I just wanted to think about this more even though there is not an exercise about it.

### Answer

Case 1: I bid b=v. 

In this case, if I win, utility is zero, but thats fine. I didnt lose. I got something I deemed at a fair price.

Case 2: I bid b<v.

If I lose, fine. If I win, utility > 0. great. This the case that makes it non-DSIC. the auction still functions, but I'm incentivized to consider bids lower than my valuation. Whereas in 2nd-bid pricing, my bid does not directly correlate to my utility other than a win/lose function.

Case 3: I bid b>v.

I means this is dumb. if I win its negative utility.

## E 2.1

Exercise 2.1 Consider a single-item auction with at least three bidders. Prove
that awarding the item to the highest bidder, at a price equal to the third-highest
bid, yields an auction that is not DSIC.

### Answer

Part 1: Being honest

B1: {v: 100, b: 100} // honest
B2: {v: 150, b: 150} // honest
B3: {v: 200, b: 200} // honest

In this case, B3 wins, and B2's utility is 0

Part 2: Lying

B1: {v: 100, b: 100} // honest
B2: {v: 150, b: 250} // lie
B3: {v: 200, b: 200} // honest

B2 wins the bid, even though their valuation was < B3's valuation.

B2's utility is v-p (150-100): $50.

Thus a winning strategy is to lie, so 3rd-highest bid is NOT DSIC.


## E 2.2

Exercise 2.2 Prove that for every false bid b_i ≠ v_i by a bidder in a second-price
auction, there exist bids b_~i (bids by not i) by the other bidders such that i’s utility when bidding
b_i is strictly less than when bidding v_i.

### Answer

So lets look at bidder i=2. B2, where b_2 ≠ v_2.

There are two cases. When b_2 < v_2, and when b_2 > v_2.

Case 1: b_2 < v_2

In this case, B2 made a bid lower than their valuation.

We can construct B3's bid where v_2 > b_3 > b_2.

In english: B3 made a bid that was lower than B2's valuation, yet B2 still lost. Utility = 0. Poor B2.

B2's utility here is 0. if B2 had been honest, they would have beaten B3, giving a utility > 0.

Case 2: b_2 > v_2

In this case, B2 made a bid higher than their valuation.

B1: {v: 100, b: 100} // honest
B2: {v: 150, b: 250} // lie
B3: {v: 200, b: 200} // honest

Here, when B2 wins, their utility is v - p (150-200 = -50). p is greater than v, so their utility is negative.
If they had been honest, they would have lost the bid with utility 0, and 0 > -50.

## E 2.3

Exercise 2.3 Suppose there are k identical copies of an item and n > k bidders.
Suppose also that each bidder can receive at most one item. What is the analog of
the second-price auction? Prove that your auction is DSIC.

### Answer

We have N bidders, and K items, and N > K.

We have W winners, where W = K.
That means we also have L losers, where L = N-K.

Since the items are identical, the price W pays can be identical.

The closest bid that the W did not need to beat was the greatest L's bid.

As long as L's bid < any of the W's price, utility for W will be positive.

Proof:

What happens when a bidder...

A. does b > v, so if they win => yields -utility when truth would have yielded 0
B. does b < v, so if they lose => yields a 0 utility when truth would have yielded > 0

So this is DSIC because both forms of dishonest yields a lower utility

## E 2.4

Exercise 2.4 Consider a seller that incurs a cost of c > 0 for selling her item—
either because she has a value of c for retaining the item or because she would
need to produce the item at a cost of c. The social welfare is now defined as the
valuation of the winning buyer (if any) minus the cost incurred by the seller (if
any). How would you modify the second-price auction so that it remains DSIC
and welfare maximizing? Argue that your auction is budget-balanced, meaning
that whenever the seller sells the item, her revenue is at least her cost c.

### Answer

In this case, we take into account c.

welfare (w) = v - c.

To be budget balancing, the auctioner needs to set a minimum bid price that is >= c.
For this to be DSIC, everything stays the same, its just that for each bidder, b >= c.

This means that if there are any bids below c, well, the auctioner won't accept. 
If there is only 1 bid above c, then c is the price.
If there are > 1 bids above c, we fall back to the standard 2nd-price model described above.

As far as lying:
If a bidder's valuation < c, they necessarily have negative utility if they win because they lied to place a bid and p > v.
If a bidder's valuation > c, then we fall back to standard auction of 2nd-price, which we've already established as DSIC.

