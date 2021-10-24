### Quatre-four (Q-core)

![fourman](https://user-images.githubusercontent.com/87430168/138263368-22748e2d-9faa-447b-9d5d-f589ac62d4ff.png)
-----------------------------------

This is a pool four-man peer-to-peer short-term lending and borrowing structure with 2 major categories and 4 subcategories to preselect from. They all benefits from mutual lending and borrowing in a rotational manner. That is, an user subcribing to Quatre-four will be a lender and same time a borrower. So if you're looking to lend only, please refer to the [Q-Lend section](https://link-here). Users must have at least, an amount in _[minimumstakingAmount]()_ given via approval in favor of the _[factory contract]()_. It will be deducted from the source then added to their stake balance - tie-locked to the _[factory]()_ throughout the _[quat period]()_. Subsequently, balance is automatically available to unstake.

> `NOTE:` After the *quat period* has ended, reward will stop counting. 

[fig 1.0]()

BtoS | base | exponential | denominator | value | | StoB | base | exponential | denominator | value
---- | ---- | ----------- | ------------ | ----- |-| ---- | ---- | ----------- | ------------ | ---------------------
4 | 10 | 18 | 0.000000000000000001 BNB | 4 BNB | | 3000 | 10 | 1 | base x base asset's decimals | 3000 x denomination
8 | 10 | 18 | 0.000000000000000001 BNB | 4 BNB | | 6000 | 10 | 1 | base x base asset's decimals | 6000 x denomination
12 | 10 | 18 | 0.000000000000000001 BNB | 4 BNB | | 9000 | 10 | 1 | base x base asset's decimals | 9000 x denomination
20 | 10 | 18 | 0.000000000000000001 BNB | 4 BNB | | 20000 | 10 | 1 | base x base asset's decimals | 20000 x denomination

Exmaple: Assume (in order of first-come) Alice, Bob, Peter and John joined a pool of **`4 BNB`**, each of which is not aware of another's identity. Alice being the first, selects **`4`** from the **`BtoS`** category. At this point, Alice is required to forward along with the call - an amount of **`4 BNB`** only if the current pool is unfilled hence a new instance of pool with Alice's preferences is launched and she is added. The final value of each consecutive preceeding number in the list `(fig. 1.0)` is an unsigned integer representing 10 in exponential of 18 multiplied by the denominator presented in smallest unit of BNB. Alice will retain the first position in the current **`BtoS[4]`** pool. Every subsequent user that joins the pool is treated in the order of first-in-first-out (FIFO) basis. Soon as the expected pool participants is achieved, the total pool amount is immediately available to the first participant to withdraw, in this case **Alice**.

What it simply mean is that, the [Proxfactory](https://something.here) creates a single pool in any of the selected category that can only be filled with four persons. While the pool has slots, anyone is free to join, perhaps the protocol unanimously add user to a free slot in the category they have selected. When the pool is completed, a flag is raised which sets an activation time allowing the first participant to withdraw the total pool amount. To access the fund, Alice will provide collateral base on the set collateral factor as at that time. She will have the possession of the total pool amount for period not greater than 7 days after which fund is made available to the next on the queue. `Note`: We do not track what Alice uses this fund for but in the future, we plan to integrate more investment tools in the protocol. It is a mutual financial relationship among four persons who have by implied reason agreed to collectively provide funds to finance one another at a lending rate (set by the ecosystem users) and share profits in equal ratio. Every participants in the pool is lender and same time borrower. The Quatre protocol ensures that no potential internal loss is incurred in this relationship by enforcing necessary and some strict measures but does not guarantee profit from business or fiancial engagement (s) user may diversify into with the fund. On the repayment due date (plus grace period if any), if the borrower defaults, a liquidation floor is open but restricted only to any of the three remaining members otherwise, the pool is updated and available to the next on queue i.e Bob. [Read and understand how the liquidation works](). When Alice repays, it comes with interest recorded in favor of all participants. The circle continues until John's session is completed. For more information, please see the [FAQ section](). Soon as the round is completed (i.e 28 days period), the interest(s) in the pool is aggregrated, shared and distributed equally amongt the four participants

**`NOTE :`** _Quatre-finance does not have control over your account or funds. In fact, we have no way to access it_.

#### In-line benefit
Some time, it may take a while for the pool to complete since action does not begin until the required quorum is attained, to compliment for this, paeticipants automatically qualify to participate in the Quatre farming where they earn reward at every emitted block for participating in the protocol. Reward is calculated [here](). However, this is not to be confused with reward for staking as the base rate for the former is lesser than latter. Benefits come in both ways: _interest for lending to others_, _benefits of using the pool to generate more asset_, _reward for participating in the protocol_, and _staking benefit_,

#### The goal
We aim to enable anyone from any part of the globe to access a short-term moderate amount of loan by providing a quota with promise to return (without default) the full amount together with accrued interest, and direct it to any profit-yielding endeavor (s) or use for trading on exchange (s) of their choice while at the same being a lender while being part of the decision maker. We cannot also rule out the reward aspect where participants are rewarded for staking together with participation in keeping the protocol healthy. 

-----------------------

:copyright: Quatrefinance | **[Return to home](https://github.com/Quatre-Finance/Q-paper#concept-overview)**

