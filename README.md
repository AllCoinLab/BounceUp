# BounceUp

# Feature
Price bounces up after the sell

# Motivation
Buyback system is incomplete
-> want to make a new system
-> BounceUp is made

# Detailed Description
Buyback system is incomplete system for below reasons  
1. Buy happens **BEFORE** the sell  
before or after, buy can make the price go up.  
But as it happens before the sell,  
it helps sellers to get more money.  
If it was for the mitigating impact of the sell,  
it should have been done after the sell.

2. Buy amount is constant
So if someone makes small amount of sell than the buy amount,  
person can benefit with higher price because of this buy.  
Also it could make overall price to go up.  
It seems good for the holders,  
but the sellers usually can take advantage of this by selling small amounts in multiple sequence.  
For example,  
people can make very small buy to trigger constant buy multiple times to make price high,  
and then sell all to make a bigger profit.  

3. To block 1,2, liquidity should be high
If liquidity high, price will not change by relatively small amount of buy.  
So 1. sellers wont get more money, 2. price will not go up and so won't get a bigger profit.  
But it means buyback system itself is not effective.  
it just makes a auto relatively small buy before the sell to make green buy log in the poocoin.  
but it is not effective enough in the high liquidity situation.  
also does not mitigate the sell impact regarding high liquidity.  

4. because of 3. it is hard to be applied in low liquidity token.
only presales with high liquidity can apply this method.  
that means it cannot be widely used like redistribution, autoliquidity system.  
as more widely used system helps more advertisement of the token invented that,  
buyback system has limitations.

5. It needs bag with BNB
and also with 3, it needs big BNB.  
which also enhances the problem of 4.

# Detailed motivation
I have made a new system which removes all those limitations,  
most of all, **BUY HAPPENS AFTER THE SELL**  
and can be applied with any liquidity size.  
with proportial buy size based on sell size.  
so it actually mitigates the impact of the sell.  
Also it doesnt need BNB bag.  

So I named it as 'BounceUp'  
(can be changed by the community. as always)
as price actually bounce up after the sell 

and like I said, it is proportional with sell size,  
so it relatively bounces (mitigates) the impact of the sell.  
It will not make effective price movement if the buy is small and the liquidity is high,  
but it means sell is also small.  
So it will be meaningless for the comparing effectiveness with the liquidity.  
It should be compared with the sell impact.  

# Implementation
## Buy happens after the sell  
This is tricky part because in the sell process of the usual pancake router,  
token transfer -> BNB swap happens in sequence.  
if buy to be happened after the sell,  
It should be done after the BNB swap. which is impossible in this process.  

It was hard for me but I have made a tweak workaround.  
Now verifying that it could be possible.  
And implementation could be hard.  
So it may take lot of time. or maybe not.  

And test will be quite easy.  
Just spending some money matters.  

# Implementation Difficuly
High

Thank you
