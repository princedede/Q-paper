### Quatre-four (Q-core)

This is a pool of four-participants cooperative peer-to-peer short-term lending and borrowing structure with 2 major categories and 4 subcategories to preselect from. They all benefits from mutual lending and borrowing in a rotational manner. That is, an user subcribing to for this category is deemed a lender and borrower at the same time. If you're looking to lend only, please refer to the [Q-Lend section](https://link-here). Users must have at least, an amount in _[minimumstakingAmount]()_ given via approval in favor of the _[factory contract]()_. It will be deducted from the regular ledger balance and is added to their stake balance; tie-locked to the factory throughout the _[quat period]()_. After the whole rounds is completed, balance is automatically available to unstake.

> `NOTE:` After the *quat period* has ended, reward will stop counting. Quat is achieved when the four rounds is completed.

[fig 1.0]()

BtoS | base | exponential | denominator | value | | StoB | base | exponential | denominator | value
---- | ---- | ----------- | ------------ | ----- |-| ---- | ---- | ----------- | ------------ | ---------------------
4 | 10 | 18 | 0.000000000000000001 ETH | 4 ETH | | 3000 | 10 | 1 | base x base asset's decimals | 3000 x denomination
8 | 10 | 18 | 0.000000000000000001 ETH | 4 ETH | | 6000 | 10 | 1 | base x base asset's decimals | 6000 x denomination
12 | 10 | 18 | 0.000000000000000001 ETH | 4 ETH | | 9000 | 10 | 1 | base x base asset's decimals | 9000 x denomination
20 | 10 | 18 | 0.000000000000000001 ETH | 4 ETH | | 20000 | 10 | 1 | base x base asset's decimals | 20000 x denomination

`NOTE`: For demonstration purpose, we use ETH as a denomination. The real denomination will reflect when product is live.

Exmaple: Assume (in order of first-come) Alice, Bob, Peter and John joined a pool of **`4 ETH`**, each of which does not have to be aware of other's identity. Alice being the first, selects **`4`** from the **`BtoS`** category. At this point, Alice is required to forward along with the call - an amount of **`4 ETH`** only if the current pool is unfilled hence a new instance of pool with Alice's preferences is launched and she is added. The final value of each consecutive preceeding number in the list `(fig. 1.0)` is an unsigned integer representing 10 in exponential of 18 multiplied by the denominator presented in smallest unit of ETH. Alice will retain the first position in the current **`BtoS[4]`** pool. Every subsequent user that joins the pool is treated in the order of first-in-first-out (FIFO) basis. Soon as the expected pool participants is achieved, the total pool amount is immediately available to the first participant to withdraw, in this case **Alice**.


What this simply mean is: the [Proxfactory](https://something.here) creates a single pool in any of the selected category that can only be filled with four persons. While the pool has slots, anyone is free to join, perhaps the protocol unanimously add user to a free slot in the category they have selected. When the pool is completed, a flag is raised which sets an activation time allowing the first participant to withdraw the total pool amount. To access the fund, Alice will provide collateral base on the set collateral factor as at that time. She will have the possession of the total pool amount for period not greater than 7 days after which fund is made available to the next in queue. `Note`: We do not track what Alice uses this fund for but in the future, we plan to integrate more investment tools in the protocol. It is a mutual financial relationship among four persons who have by implied reason agreed to collectively provide funds to finance one another at a lending rate (set by the ecosystem users) and share profits in equal ratio. Every participants in the pool is lender and same time borrower. The Quatre protocol ensures that no potential internal loss is incurred in this relationship by enforcing necessary and measures but does not guarantee profit from business or financial engagement (s) user may diversify into with the fund. On the repayment due date (plus grace period if any), if the borrower defaults, a liquidation floor is open but restricted only to any of the three remaining members otherwise, the pool is updated and available to the next on queue i.e Bob. [Read and understand how the liquidation works](). When Alice repays, it comes with interest recorded in favor of all participants. The circle continues until John's session is completed. For more information, please see the [FAQ section](). Soon as the round is completed (i.e 28 days period), the interest(s) in the pool is aggregrated, shared and distributed equally among the participants

**`NOTE :`** _Quatre-finance does not have control over this pool of funds. In fact, we have no way to access it_.

---------------------------

#### In-line benefit
Some time, it may take a while for the pool to complete since action does not begin until the required quorum is attained, to compliment it, participants are automatically qualified to participate in farming **QFT** where they earn reward at every emitted block for participating in the protocol. Reward is calculated [here](). However, this is not to be confused with reward for staking as the base rate for the former is lesser than latter.

Benefits come in the following ways: 

- _Interest on lending and borrowing_
- _Benefits of utilizing the pool to generate more profits_
- _Reward for participating in the protocol_
- _Staking benefit_

--------------------------

#### The goal
The target is to enable anyone across the globe to access a moderate short-term loan by providing a quota with promise to return (without default) the full amount together with accrued interest, and direct it to any profit-yielding endeavor (s) of their choice or access credits using existing portfolio as collateral. We cannot also rule out the reward aspect where participants are rewarded for staking as well as participating in the protocol. 

-----------------------

**[Previous]()** | **[Next]()**

:copyright: Quatrefinance | **[Home](https://github.com/Quatre-Finance/Q-paper#concept-overview)**

