# Introduction
![Logopit_1632895157540](https://user-images.githubusercontent.com/35783747/135256124-da1fe235-08d6-453a-9734-3148911a77d2.png)

## Welcome to Quatre-Finance.

---------------------

### What is Quatre-Finance (QFOUR)?
Quatre-finance is a platform for decentralized digital services that aims not to completely uninstall the application world but to continually re-emphasize the need for true decentralization by building decentralized products tailored to individual needs putting them in complete control of their funds and/or investments. Our core product and ideology is centred around creating a platfiorm for low-income to high income grade users to easily access funds via peer-to-peer system.

Our mission is to provide tools for that create and manages financial relationship between lenders and borrowers without either parties having to know or trust who they are dealing with in a manner that regards the right of both parties, give them equal control and everyone is happy in the end. 

### Quatre-finance underlying technology.
The protocol will exist both on the Binance smart chain and Ethereum blockchain technologies.

### Why Binance Smart Chain?
Every EVM compatible technologies have one thing that differentiates them from one another. We chose Binance for a couple of reasons. Some of which states: 

* It is Ethereum virtual machines compatible i.e it capable of executing smart contracts instructions which we deem suitable for implemeting our backend.
* Binance Smart Chain (BSC) is preferred for its considerably low transaction fees.
* BSC network encourages Borderless decentralized finance (DeFi) that allows anyone around the globe with an internet service to acceess our services.
* Its performance is suitable for mass adoption.

Leveraging on the use cases of blockchain technology such as the distributive, permissionless and immutability features via smart contract architecture, we established Quatre-finance protocol that inherits the modern blockchain attributes with customised rules.

###  Highly Decentralized
Even with some decentralized finance platforms, you're still at the mercy of someone. At Quatre-finance, you decide which way to go if your decision is fairly reasonable enough. 
Our products and core value will always consider a four-sided properties thus:
- Own it.
- control it.
- be fair.
- trust less.

#### Own it
Quatre products gives the fulfilment of owning it. Accessility to your funds are blended with your signature and you don't have to be at the mercy any centralized exchange platform to bring in or take take out your funds. We build it : you own it.

#### Control it
> Knowing you're in control is the first assurance of security.

Control is preceded by ownership. In fact they go hand in hand. The Quatre protocol brings you a high level of control over your assets/funds. If you engage in any of the Quatre-finance's p2p products, control is mutual while you also retain a good amount of ownership.

#### Be fair
We believe in fair dealings. While control and ownership belongs to a user, our protocol ensures that other parties involved with you in any transaction are fairly treated without jeopardizing your need for control.

#### Trust less
This is an inherently-interesting blockchain feature that Quatre-finance builds upon. With this, Alice does not need to know or have Bob's trust in order to transact without fear. Quatre protocol gives you rest of mind without knowing the identity of the other party.

----------------------------------------------------------------
## Quatre Products

### Quatre-four (Q-core)
- How it works

A pool four-man peer-to-peer short-term lending and borrowing structure with 2 major categories and 4 subcategories to preselect from. They all benefits from mutual lending and borrowing in a rotational manner. That is, an user subcribing to Quatre-four will be a lender and same time a borrower. So if you're looking to lend, please refer to the [Q-Lend section](https://link-here). Users must have at least, an amount in _[minimumstakingAmount]()_ given via approval in favor of the _[factory contract]()_. It will be deducted from the source then added to their stake balance, tie-locked to the _[proxy]()_ throughout the _[quat period]()_. Subsequently, balance is automatically available to unstake.
> `NOTE:` After the *quat period* has ended, reward will stop counting. 

[fig 1.0]()

BtoS | base | exponential | denominator | value | | StoB | base | exponential | denominator | value
---- | ---- | ----------- | ------------ | ----- |-| ---- | ---- | ----------- | ------------ | ---------------------
4 | 10 | 18 | 0.000000000000000001 BNB | 4 BNB | | 3000 | 10 | 1 | base x base asset's decimals | 3000 x denomination
8 | 10 | 18 | 0.000000000000000001 BNB | 4 BNB | | 6000 | 10 | 1 | base x base asset's decimals | 6000 x denomination
12 | 10 | 18 | 0.000000000000000001 BNB | 4 BNB | | 9000 | 10 | 1 | base x base asset's decimals | 9000 x denomination
20 | 10 | 18 | 0.000000000000000001 BNB | 4 BNB | | 20000 | 10 | 1 | base x base asset's decimals | 20000 x denomination

Exmaple: Assume (in order of first-come) Alice, Bob, Peter and John joined a pool of **`4 BNB`**, each of which is not aware of another's identity. Alice being the first, selects **`4`** from the **`BtoS`** category. At this point, Alice is required to forward along with the call - an amount of **`4 BNB`** only if the current pool is unfilled hence a new instance of pool with Alice's preferences is launched and she is added. The final value of each consecutive preceeding number in the list is an unsigned integer representing 10 in exponential of 18 multiplied by the denominator presented in smallest unit of BNB. Alice will retain the first position in the current **`BtoS[4]`** pool. Every subsequent user that joins the pool is treated in the order of first-in-first-out (FIFO) basis. Soon as the expected pool participants is achieved, the total pool amount is immediately available to the first participant to withdraw, in this case **Alice**.

What it simply mean is that, the [Proxfactory](https://something.here) creates a single pool in any of the selected category that can only be filled with four persons. While the pool has slots, anyone is free to join, perhaps the protocol unanimously add user to a free slot in the category they have selected. When the pool is completed, a flag is raised which sets an activation time allowing the first participant to withdraw the total pool amount. To access the fund, Alice will provide collateral base on the set collateral factor as at that time. She will have the possession of the total pool amount for period not greater than 7 days after which fund is made available to the next on the queue. It is a mutual financial relationship among four persons who have by implied reason agreed to collectively provide funds to finance one another at a prevailing market lending rate and share profits in equal ratio. Every participants in the pool is lender and same time borrower. The Quatre protocol ensures that no potential loss is incurred in this relationship by enforcing necessary and some strict measures but does not guarantee profit from business or fiancial engagement (s) user may diversify into with the fund. On the repayment due date (plus grace period if any), if the borrower defaults, a liquidation floor is open but restricted only to any of the three remaining members otherwise, the pool is updated and available to the next on queue i.e Bob. [Read and understand how the liquidation works](). When Alice repays, it comes with interest recorded in favor of all participants. The circle continues until John's is completed. For more information, please see the [FAQ section]().

**`NOTE :`** _Quatre-finance does not have control over your account or funds. In fact, we have no way to access it._

#### In-line benefit
Some time, it may take a while for the pool to complete since action does not begin until the required quorum is attained, to compliment for the lag, we automatically qualify user to participate in the Quatre farming where they earn reward at every emitted block for participating in the protocol. Reward is calculated [here](). However, this is not to be confused with reward for staking as the base rate for the former is lesser than latter.

#### The goal
We aim to enable anyone from any part of the globe to access a short-term moderate amount of loan by providing a quota with promise to return (without default) the full amount together with accrued interest, and direct it to any profit-yielding endeavor (s) or use for trading on exchange (s) of their choice. We cannot also rule out the reward aspect where participants are rewarded for staking together with participation in keeping the protocol healthy.  

----------

### Quatre LandB (Q-LandB)

Similar to **Q-core**, LP providers in this category are lenders but singlehandedly provide loans in the amount they wish. We do not have a pool of persons but a fairly one-man show. The lender sets parameters such as the loan amount, collateral plus the factor, duration their funds can be used and a few others. By  the proxy pattern, the lender owns up to 50% level of control while rest is shared between the proxy and the borrower. There can only be one borrower in a round. That is, if as an instance, the lender set duration to 14 days of use, then no other borrower will be allowed during this period until the current loan is settled. However, this category does not qualify for the Quatre farming reward.

**`NOTE :`** _Quatre-finance does not have control over your account or funds. In fact, we have no way to access it. You own it._

----------

### Quatre P2P (Q-Native)



## Understanding the FOUR Token
**FOUR** : (BEP20 standard : Binance smart chain) is the native token of the Quatre-finance platform with enormously foreseeable use cases deployed and verifiable at [BScscan](http://bscscan.com).

**Name** | **QFOUR Token**
-------- | ---------------
**Ticker(Symbol)** | **FOUR**
**Decimals** | **18**
**Max Supply** | **500_000_000** x **10** ** **Decimals**
**Total Supply** | _vary_
**CurrentSupply** | **Total Supply**

The **FOUR** Token is controlled by smart contract at [[Contract Address]](http://bscscan.com) which is owned by the [[Farmer Contract Address]](http://bscscan.com). The instruction is set at construction time for the farmer can only mint a total lifeTime amount of **_Max Supply_**. The farmer is a bit stricter, never allows token be burnt by anyone but by self with mechanisms a mechanism for creating scarcity to bring greater value to the **FOUR Token**. 

### Farmer does not allow to burn token. Why?
As the farm owner, the farmer needs to have more control on his produce hence the restriction but without sacrificing decentralization, that is, anyone who buys from the farmer is an acceptable valid channel (s) retains the ownership for as long as they wish. In the event of otherwise,   **QFOUR Token** is designed to call for value via its use cases and a special staking algorithm which temporarily mops out token from circulation by usage (i.e NeedDotStaking NDS) as staking increases and similarly emits when unstaked.
  * #### How it works: 
  For instance, in the Buy and Sell category, to keep the system healthy, a user who wants to create a seller account is required to have an amount in **FOUR** Token staked with the farmer via a proxy account. When the ```stake()``` is called, it switches the farmer to what we termed **_Sedentary mode_**. This is a state of unavailability that does reduces **totalSupply** by the staked amount. The balance is reflected in the **_allowances_** of farmer to the source contract - balance which is neither spendable nor withdrawable by anyone. 
 Just as the mechanism renders the caller's staked balance inactive for the period as long as the account is active. The only way to retrieve the staked balance is when **proxy account** is ```closeOut()```. In this process, an action is created notifying the farmer. Thereafter, a **_stakedAmt** is forwarded along with the accrued reward to the staker's account. It in-turn increases the amount of token in circulation. One can always verify total **QFOUR** Token in circulation either from the farm or the farmer.
  This applies only to the **"Pro"** category.
  Also, it uses a method of recycling

`NOTE`: At any given time, **_CurrentSupply_** will always equal **_TotalSupply_**.

#### Uses of **QFOUR Token**.
**QFOUR Token** will be used for but not limited to such as:
- For fee in some, not all Quatre-finance products.
- To keep the ecosystem healthy via intermediate programs such as staking.
- Gas to keep the proxies running.
    ...
    
    




### Ways to Earn With Quatre-finance
* 

