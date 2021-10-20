# Introduction
![Logopit_1632895157540](https://user-images.githubusercontent.com/35783747/135256124-da1fe235-08d6-453a-9734-3148911a77d2.png)

## Welcome to Quatre-Finance.

---------------------

### What is Quatre-Finance (QFOUR)?
Quatre-finance is a platform for decentralized digital services that aims not to completely uninstall the application world but to continually re-emphasize the need for true decentralization while building decentralized products tailored to individual needs putting them in complete control of their funds and/or investments. Our core product and ideology is centred around creating a platfiorm for low-income to high income grade users to easily access funds via peer-to-peer system. Our incentivized program (s) allow investors, liquidity provider and participants in the network to make more from their committed funds, time and participation.

Our mission is to provide build decentralized products that create and manages financial relationship between parties to trade (lenders and borrowers, buyers and sellers) exempting an intermediary, without either of the parties having to know or trust who they are dealing with in a manner that regards the right of both parties while giving them equal control commensurate to their position in the trade at that point, and everyone is happy in the end. 

### Quatre-finance underlying technology.
The protocol will exist both on the Binance smart chain and Ethereum blockchain technologies. The former ranks first on our list of preferences.

### Why Binance Smart Chain?
Every EVM compatible technologies have one or more uniqueness (es). We chose Binance for a couple of reasons. Some of which are thus: 

* It is Ethereum virtual machines compatible. That is, it is capable of executing smart contracts instructions which we deem suitable for implemeting our backend.
* Binance Smart Chain (BSC) is preferred for its considerably low transaction fees.
* BSC network encourages Borderless decentralized finance (DeFi) that allows anyone around the globe with an internet service to acceess our services.
* Among others, its performance is suitable for mass adoption.

Leveraging on the use cases of blockchain technology such as the distributive, permissionless and immutability features via smart contract architecture, we established Quatre-finance protocol that inherits the modern blockchain attributes with customised rules.

###  Highly Decentralized
Even with some decentralized finance platforms, you're still at the mercy of someone. At Quatre-finance, you decide which way to go: if your decision is fairly reasonable enough regarding the rights of your counterparties.

Our products and core value will always consider a four-sided properties thus:
- Own it.
- control it.
- be fair.
- trust less.

#### Own it
Quatre products gives the fulfilment of ownership. Most of our products are (and will be) designed to brings you ownership experience. Accessility to your funds are blended with your signature and you don't have to be at the mercy of any centralized exchange platform to bring in or take take out your funds. We build it : you own it.

#### Control it
> Knowing you're in control is the first assurance of security.

Control is preceded by ownership. In fact they go hand in hand. The Quatre protocol brings you a high level of control over your assets/funds. If you engage in any of the Quatre-finance's p2p products, control is mutual while you also retain a good amount of ownership.

#### Be fair
We believe in fair dealings. While control and ownership belongs to the user, we on the fair side ensures that counterparties in any transaction are fairly treated without jeopardizing your need for control.

#### Trust less
This is an inherently-interesting blockchain feature that Quatre-finance builds upon. With this, Alice does not need to know or have Bob's trust in order to make transact with him. Quatre protocol gives you rest of mind even while the identity of the other party is preserved.

----------------------------------------------------------------

## GETTING STARTED

### Quatre-four (Q-core)

A pool four-man peer-to-peer short-term lending and borrowing structure with 2 major categories and 4 subcategories to preselect from. They all benefits from mutual lending and borrowing in a rotational manner. That is, an user subcribing to Quatre-four will be a lender and same time a borrower. So if you're looking to lend only, please refer to the [Q-Lend section](https://link-here). Users must have at least, an amount in _[minimumstakingAmount]()_ given via approval in favor of the _[factory contract]()_. It will be deducted from the source then added to their stake balance - tie-locked to the _[factory]()_ throughout the _[quat period]()_. Subsequently, balance is automatically available to unstake.
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

#### FAQ - Q-core

- **What is a session?**
This is a period of not greater than 7 days i.e period from the time fund was released to repayment period.

- **What is a period**
Aggregate time (days) it takes to complete a round i.e 28 days.

- **How is collateral factor determined?**
QuatreFinance is decentralized hence every participants in the protocol is given opportunity to parcipate in decision making. QuatreFinance operaes a governance model that allows users of the platform to participate in upgrade process by voting for what they wish to be implemented in the protocol. Such process requies that user has voting power prior to voting which is weighted in the platform native asset. After voting is completed, the factory is updated with the proposed interest rate.

- **How much do I need to join a pool?**
By specification, there are two major categories an user can choose from thus: `BtoS` and `StoB`. **BtoS** signifies that user will join a pool where they can lend and borrow **BNB** or **ETH** collaterized in stable currency or fiat such as **USDT**. The reverse is to **BtoS** category. Under each of the categories, there are four sub-categories. For `BtoS`: *4 BNB*, *8 BNB*, *12 BNB* and *16 BNB* and `StoB` : *3000*, *6000*, *9000*, *15000*. User who selects any of these categories will have to provide exact amount at the point of joining.

- **How do I join?**
    - Have the _[minimumstakingAmount]()_ (in QFT) in your wallet.
    - Proceed to the Quatre interface and give approval to the factory to spend the minimum amount from your wallet.
    - If you select any of the `BtoS` category, have the equivalent amount in your wallet else perform step 2 for currency accepted on the interface.
    - Call the required function.

- **What happens next after I joined?**
The contract is smart enough to know when the pool is completed. Your fund is safe. Soon as the pool is completed, the total funds in the pool is available for withdraw only to the next person treated in first-in-first-out (FIFO) basis.

- **What if no one join?**
We built QuatreFinance for the masses and on peer-to-peer trustless and faceless basis hence we believe the timing will become shorter in no time as more people get to know about us. In the event of a lengthy delay, after 6 hours or block based on average block emission on the target network (whichever comes first), user is automatically staged to earn reward based on amount selected for a period. 
`Note`: This may change in the future as we hope to device better incentive structure for the platform via the community governance.

- **What happens if any of the participants default?**
Firstly, the protocol ensures to fund is let out unless collateral is provided. If any of the participants defaults in repayment, the protocol will leave the floor open to any of the rest three liquidate the borrower. liquidation sets off borrower's debt with the deposited collateral with additional liquidation fee if any. If balance is left after calculation made and deducted from the collateral, it is sent to the borrower and their position is left blank.  The round continues until a period is achieved. 

-------------------

### Quatre LandB (Q-LandB)

Similar to **Q-core**, Providers in this category are lenders that singlehandedly provide loans in the amount they wish via their personal account residing in the _[proxy]()_. Here, we do not have a pool of persons but a fairly one-man who decides when to put his fund in use. The lender sets parameters such as the loan amount, collateral plus the factor, interest rate, duration their funds can be used and a few other settings. Going by the proxy pattern, the lender owns up to 50% level of control while rest is shared between the proxy and the borrower. We embedded some checks that analyzes the activities of both parties ensuring interests are protected. There can only be one borrower in a round. That is, if as an example, the lender set duration to 14 days of use, then no other borrower will be allowed during this period until the current loan is settled. If the borrower defaults payments after the repayment period lapses, the right to liquidate the borrower remains with the lender. While yet not the reapayment period, lender has no means to put the other party in the liquidation state. However, this category does not qualify them for the Quatre farming reward.
One can also consider a p2p use case scenario where Bob does not want to sell off his **BNB** but need some stable asset, requests to borrow some from Alice. Because of trust issues in human nature coupled with the fear of not paying back the loan, Alice may be reluctant to grant such request. But with vast improving technology, Alice can set up and account (_[Proxy]()_) on the QuatreFinance _[interface]()_ with the required fund and thereafter refer Bob to his account in the lenders pool.

#### FAQ - Q-LandB

- **What is a proxy account?**
An account created solely for an user blended with their signatures with owner and control of it. In the case of **Q-LandB**, A proxy administers and manages lending and borrowig relationship between the owner and the borrower.

- **What do I need to set up a proxy account?**
    - Have the _[minimumstakingAmount]()_ (in QFT) in your wallet.
    - Have the _[minimum creation fee]()_ in _**BNB**_.
    - Hit the required button and a proxy is launched for you. The minimum stake amount is deducted from your EOA and staked in favor of the proxy created amount which is locked for as long as the proxy runs. The reward for minimum stake amount accrues as well. 
    - There is a one-time creation fee which is very minimal with repect to the network it is deployed to.

- **Who updates the Proxy parameters?**
Owner of course! And that's the initiator. As the initiator, we provide you with detailed information on how to updated any of the upgradeable parameters such as the price, interest rate etc.

- **What if I need to close my account?**
You are fee to stop your proxy from running at any time. However there two options with which you can do this: 
    `pause`: You can pause your account so one can perform any buy transaction. But does not unstake the initial minimum stake amount.
    `closeOut`: Closing your account permanently deactivates your account from the database. Even though the identifier address is visible, yet it cannot perform any transaction again. Before this is done, your initial minimum stake amount is unstaked and sent to your recognized address together with accrued reward to date.

- **Any potential risk involved?**
Your account (Proxy) hold values hence should be valued and protected. An access to your account (EOA with which youu created it) should be well secured. The proxy is securely built to resist unwanted actions on sensitive settings other than you from external sources but we do not have control over external actions that may be supercharged to it either in the course of owner's negligence or superadded activities from the direct users.

**`NOTE :`** _Quatre-finance does not have control over your account or funds. In fact, we have no way to access it. You own it._

----------


### Quatre Buy and Sell (Q-BandS)

This category operates similar to the usual way of buy and selling crypto assets but with uniques differences and features thus:
- No centralized exchange or intermediary.
- No KYC is needed.
- Seller creates a one-time flexible account (added to the pool of sellers on the Quatre page) that absolutely belongs to them. Flexibility means that it can be added/listed on our partners's exchange for greater visibility(`coming soon...`). **`Note`**: this may remove the **no-kyc** feature. Anyone can be referred to directly buy from same seller repeatedly.
- Prices are solely determined and set by the seller. Our protocol handles all necessary and underlying calculations, checks and balances for achieving precision.
- Free from CEX's regulations and demands.
- Your funds stay with you.
- Sell as much as you want.
- Withdraw as much as want.

#### FAQ - Q-BandS

- **What do I need to set up a Q-BandS account?**
    - Have the _[minimumstakingAmount]()_ (in QFT) in your wallet.
    - Have the _[minimum creation fee]()_ in _**BNB**_.
    - Hit the required button and a proxy is launched for you. The minimum stake amount is deducted from your EOA and staked in favor of the proxy created amount which is locked for as long as the proxy runs. The reward for minimum stake amount accrues as well. 
    - There is a one-time creation fee which is very minimal with repect to the network it is deployed to.


---------

### Quatre P2P (Q-Native)
> Coming soon ...

----------

### Quatre wallet (Q-Wallet)
> Coming soon ...

----------

## Understand the QFOUR Token metrics
**QFOUR** Token (BEP20 : ERC20 standard : Binance smart chain : Ethereum network) is the native token of the QuatreFinance platform with enormously foreseeable use cases deployed and verifiable at [BScscan](http://bscscan.com) : [Etherscan](http://bscscan.com). 

_fig. 1.1_

**Name** | **QFOUR Token**
-------- | ---------------
**Token Type** | **BEP-20**, **ERC-20**
**Ticker(Symbol)** | **QFT**
**Decimals** | **18**
**Max Supply** | **500_000_000** x **10** ** **Decimals**
**Total Supply** | _vary_
**CurrentSupply** | **Total Supply** _(may vary)_

The **QFOUR Token** : initially emmitted from [[Source Address]](http://bscscan.com) at construction time is housed mintable and burnable only by the [[Farm Contract Address]](http://bscscan.com). Total amount of **`QFT`** the farm is able to mint in the contract lifeTime cannot exceed amount of **_Max Supply_** (See fig. 1.1). Access control is enforced on _[special functions]()_ like `burn()` available only to the Farmer is controlled by this _[multisignature account]()_. Such control however does not include the general public methods specified in _[ERC20 Token standard]()_. **QFOUR Token** is built with some internal safety and checks to reduce the risk of losing funds - please refert to our _[API section]()_.

### Token-Burn
We employed this mechanism to compiment the methods we have devised for creating scarcity to bring more value to **QFOUR Token**. As the farm owner, the farmer needs to have more control on what he produces and the quantity in circulation hence the answer to why and who burns token? **QFT** is designed to call for value via its use cases and a special staking algorithm which temporarily mops out token from circulation as need increases and similarly emits when unstaked. Such need is tied to virtually all QuatreFinance products.

The Quatre team will perform periodic burn on a quarterly basis or as the team deem fit which will be communicated in our various channels.

#### How it works: 
In the Buy and Sell category for example, to keep the system healthy, a user who needs to create a seller account is required to have hold `minimumStakeAmount` in **QFT** unstakeable only via a proxy account that will be generated in the process. When the ```stake``` is called, it switches the farmer to what we termed **_Sedentary mode_**. This is a state of unavailability that does reduces **totalSupply** by the staked amount. The balance is reflected in the **_allowances_** of farmer to the source contract - balance which is neither spendable nor withdrawable. 
Just as the mechanism renders the caller's staked balance inactive for the period as long as their proxy account is active, the only way to retrieve the staked balance is when **proxy account** is `closeOut`. To perform this action, user must first put the proxy in an inactive mode, then `unstake` and `closeOut` is performed in a single call. Thereafter, the **`stakedAmount`** is forwarded along with the accrued reward to the staker's EOA. It in-turn increases the amount of token in circulation with the **`stakedAmount`**. One can always verify total **QFOUR** Token in circulation from the source totalSupply.

`NOTE`: At some point, **`_CurrentSupply_`** may differ from **`_TotalSupply_`**. This however is not an anomally. Activation of fanTip will cause the two variables to differ.

#### Some uniques features of QFOUR Token

- **`safeSignedTransfer`** : **QFT** uses a dual internal ledger to administer users' balances. Holders can choose to transfer their funds in two ways thus: **`ERC20 transfer standard`** and alternatively **`locked Balance`** (a bit different from the traditional method specified in the _[ERC20 standard]()_). To use this feature, holder of **QFT** must set up a passcode hashed (with _keccak256 hashing algorith_) and stored on-chain. At the point of setting up a lock, the total user's balance is moved to the locked section which sets the regular balance to zero while preserving the total balance. On QuatreFinance protocol, every account on the _[Binance Smart Chain]()_ by defaults inherits two ledger balances with preference given to regular default balance. Let's take scenario where **Bob** receives 1000 `QFT` for the first time. **Bob** obviously does not have lock set. His regular balance is updated to 1000 `QFT` while locked balance is set to 0. Later if Bob decides to transfer 500 `QFT` to **Alice** using the _`safeSignedTransfer`_ function, he is required to provide the lock paramaters. A lock is set up() and balance in **Bob's** regular ledger is moved to the locked section, then 500 `QFT` is unlocked and send to **Alice**.

Subsequent action will be reflected in a new state where _Bob's_ locked balance is now 500 `QFT`, regular becomes 0. If the recipient (_Alice_) already has lock set, her new state will cause her regular balance to remain unchanged while the locked balance is increased by the transferred amount.

A potential use case (An important feature of Q-Wallet) is where an attacker successfully gained access to holder's externally owned account (EOA). If the user already set a lock on their fund and have it reside in the locked ledger balance, it becomes useless for the attacker as they cannot effect a transfer unless the passlock is provided. But in this case, the regular ledger becomes a victim. At any time, a holder can choose to lock the entire balances until they are ready to make another transaction or simply unlock an amount they wish to transfer at that point.

**Note the difference**
If a holder calls the `safeSignedTransfer` with the correct _'lock'_ and _'amount'_, the value of an _'amount'_ is deducted from the aggregate balance, send to recipient and the aggregate balance left is locked.

Alternately, a holder can use the `lockBalance` to move specific amount to the locked ledger or `unlockBalance` to move an amount to the regular ledger. The traditional _`transfer(sender, recipient, amount)`_ utility simply moves an amount from the sender's regular balance to the recipient's locked balance if they have lock in place otherwise effect change to the regular balance. For more information, please refer to the  _[API section]()_.

#### Uses of **QFOUR Token**.
**QFOUR Token** will be used for but not limited to such as:
- Paying for fee in some, not all Quatre-finance products.
- For voting and making decisions in the QuatreFinance ecosystem.
- To keep the ecosystem healthy via intermediate programs such as staking.
- For incentivizing participating in the protocol.
- Gas that keep the proxies running.


### Token distribution and Economics






### Ways to Earn With Quatre-finance
* 


### FAQ
- **What is a session?**
This is a period of not greater than 7 days i.e period from the time fund was released to repayment period.
