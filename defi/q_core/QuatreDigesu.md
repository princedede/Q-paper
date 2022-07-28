### Quatre Digesu (Q-Core)
![IMG_20220223_072720 (1)](https://user-images.githubusercontent.com/35783747/157897718-5105cd09-ac12-43b3-8497-4df906247957.png)

<!-- ![IMG_20220223_072700](https://user-images.githubusercontent.com/87430168/155271873-ca4643f1-c4fd-4fca-ad85-8a62607d2529.png) -->

`NB`: This document is under development and may change from time to time.

## Problem statement

Digesu models after a prominent culture on the Africans, where two or more persons usually between 2 to 10 people provides financial support to one beneficiary `p` at a time, with a view to put the position of all the contributors as P. It is also been used as a means of saving. As simple as it sounds, it is somewhat complicated as most time, if not all, many of the participants are left with regret for committing to such scheme.  

Irrespective of the odds, yet, people find themselves coming back to form a group for this purpose - a part that is worth noting. This tells us how much people crave for financial freedom but something would not just make it work, even if they try harder. Obviously, there is/are problem (s). If we diligently trace the cause of economic hiccups, it would take us to a point where we would conclude this accounts for a significant portion.

Unarguably, there are systems such as MicroFinance and institutions who claimed to provide solutions, but their activities are obviously not suitable for the common. Their conditions and policies are too rigid for the audience.

### Setbacks
  - The biggest challenge is how to establish trust among the participants since money is involved.
  - Some participants often join with the motive to abscond.
  - The rule `"Time is money"` is not respectted.
  - Sometime, dealing with cash is unsafe. Some collectors get robbed off people's hard earned money.
  - Many supposed solutions aren't the right tool for the job hence they reinvented the problems.
  - Participants are limited to a locality which inhibits ability to access large pool of fund.

  Since money and people are involved, `trust` is a major issue to deal with and questions such as:

- Will the next paticipants fulfill their obligation?
- Will they pay back in full?
- How do we get our money if they default?
- I do not know Mr. B hence I cant peer-fund with him.
- One ajo man ran away with my money, so I am afraid to save.
- It is stressfull to join queues in the bank.
- I am not tech savvy. Besides, I am saving as little as NGN100 etc

--------------------

## How we solve it

Quater **Digesu** was conceived to uphold the social spirit while providing solutions to the aforementioned problems. Think of a system that: 
 - connects people with different financial goals from different part  of the world, 
 - harmonizes them into a community, 
 - accepts and merge arbitrary deposits from each of the participants,
 - enforces a set of rules,
 - forwards the fund to one of them until all the participant is reached
 - ensures all participants fulfil their obligation
 - creates a trustless atmosphere and rewards them for doing what is right.

Unlike the tranditionary way, to raise fund via All For One (AFO) system, participants need not be aware of the existenece of other participants or trust that they will act in good faith. Digesu as a solution uses a high level of abstraction to simplify interactivity such as : participants do not worry whether current beneficiary will fulfill their obligation or not. Blockchain technology has helped us to achieve all of these with the introduction of smart contract system.

People from the same community or anyone anywhere in the world is able to participate by launching a new community for themselves or join existing ones. When an user creates a closed community, they restrict participation to the preregistered participants. Put it, a closely related group of people could raise capital among themselves by approaching Digesu ro create an agreement binding on all the participants with commitments, at the same time enforce the agreement.
This is just one the twos Digesu does.

Each of the participants is treated as the borrower and the lender which nullifies the `interest` element. **Public band** is ideal for bprrowers and lenders looking to join an existing community. `Note` : Anyone can launch a public band. The differences and similarities are itemize below

Configuration | PUBLIC | PRIVATE
-------- | ------------ | -----------
Create | Anyone | Anyone from the group
No of expected participants (i.e Quorum) | Set by the creator at construction | Supplies list of participants' addresses at construction
Interest charge | - | -
Interval | Set at construction | Same as public
Collateral Index | Sets at construction | Same as public


----------------------

## The side 2 of the coin

This is the bigger picture and long-term vision of QuatreDigesu. The goal is to make even the less tech savvy interact with the blockchain without knowing they do. There are a lot of problems that need blockchain solution but the target audience may not be technically inclined to use the solution. We have adopted a hybrid approach to solving such challenges by blending web3 and web2 solutions which will encourage the usage of the E-naira as well.

An average African income earner saves a smaller portion of their income most especially the traders such as the market men and women, artisans, abokis and so on. QuatreDigesu will drive the exitement of saving to earn among these calibres of wealth faucets.
With Digesu, an African with the least mobile device standard will be able to save without having to worry about the safety and withdrawal of their funds.

---------------

At Quatrefinance, we harness the potentials of blockchain technology to solve existing or emerging problems in the African societies and globally. Our solutions go beyond connecting the African communities but the world at large. This implies that anyone around the world can participate in the scheme in a decentralized manner. Our software (Digesu) will not only ensure cooperations but also enforces actions to protect the rights of every user in the context of our applications, encourage savings and boost the economy on a long-run.

### Benefits of using Digesu

- Quickly raise capital without going through any form of KYC.
- Pay no interest.
- Join as many community of funders as you can.
- Cashback for Earn participating in the protocol.
- Worry less about who to trust or safety of your fund.
- Get your savings on request.
- Save more to finance business endeavours.
- Pleasant and convenient saving and funding experience.
- Earn for saving.


### For more info, see the [FAQs](https://github.com/Quatre-Finance/Q-paper/blob/main/defi/q_core/faq.md) | **[Home](https://github.com/Quatre-Finance/Q-paper#concept-overview)**
<!-- 
We represent thus:
- With collaterized:
  **Minimum QFT Holding** = **unit per head** x **Quorum**

- Without collaterized
  **Minimum QFT Holding** = **unit per head** x **Quorum** x **collateral factor**

`NOTE`: The pool admin (creator) may raise the collateral index at creation point. If this happens, the effect will be a correponding raise in the amount of **QFT holding** needed to get financed.
 -->


<!-- #### How it works
--------------
- Visit the website to launch the [app page](https://quatre.finance)

**1.** **Creating a band**

  - Strict mode

Assume Bob, Alice and Gorimapa have agreed to set up a pool of three persons to raise funds among themselves with unit amount of **1 ETH** for a total cycle of 15 days. Agreeing to set collateral to 1.2 of the total pool using **QFT** as the collateral base, we then have the following settings to launch a new pool:

  - **Amount** : **1 BNB**.
  - **Quorum** : **3**.
  - **Duration** : **5 days**.
  - **Collateral Index** : **120**. 
  - ~**Collateral Address** : **QFT Token Contract address**~.
  - **Participants** : **A list of participating addresses** in the case of private band.

**NOTE**: Supplying addresses will restrict anyone other than the broadcasted participants to make deposit to the pool.

--------------------

#### onFinance

Soon as the quorum value is reached, the total pool amount becomes available to the first on the list as preserved at creation. It continues in a rotational order if there is no default from the previous taker. This sets a lock on their **QFT** holding until the loan is repaid. Participant whose turn is to get financed must possess **QFT** in their wallet of an amount not less than the unit funding multiplied by the **Quorum** (total number of particiants) multiplied by the collateral factor.

##### onDefault

Participant who got financed may decide to amortize the loan or pay all at once but must complete the total repayment amount before the duration elapsed. If the otherwise happens, anyone (who must be a member of the pool) may liquidate the defaulter. In this case, their **QFT** is confiscated and use to set off the loan. 


  - Non-Strict mode

In contrast to the strict mode, the creator may allow anyone to join their pool. This mean, as the creator, you do not have to explicitly add participants to your community. Anyone may select to join in but the initial setting will slightly change from that of strict mode. Please use the designated function for this purpose. 

-----------------

**2.** **Joining existing pool**

A pool we created in non-strict mode is visible and allowance is set to true for anyone to join.
**NOTE**: Intending participant must have amount in base currency sufficient to pay for unit amount plus gas fee (usually minimal).  



**`NOTE :`** _Quatre-finance does not have control over funds in any of the pools. In fact, we have no way to access it_. -->

---------------------------


<!-- #### Participating benefit

At Quatrefinance each pool matters as they help strengthening the protocol. For the participants, activating a pool qualifies them to participate in the farming of **Quatrefinance Token - QFT** while completing a cycle qualifies them to earn farmed reward also as burning mechanism. However, this is not to be confused for reward for staking as the base rate for the former is lesser than latter. -->

<!-- Benefits come in the following ways: 

- _Interest on lending and borrowing_
- _Benefits of utilizing the pool to generate more profits_
- _Reward for participating in the protocol_
- _Staking benefit_ -->

--------------------------
<!-- 
#### The goal
The target is to enable anyone across the globe to access 

 a moderate short-term loan by providing a quota with promise to return (without default) the full amount together with accrued interest, and direct it to any profit-yielding endeavor (s) of their choice or access credits using existing portfolio as collateral. We cannot also rule out the reward aspect where participants are rewarded for staking as well as participating in the protocol.  -->

-----------------------

**[API](https://github.com/Quatre-Finance/Q-paper/blob/main/q_core/API.md)** | **[FAQ](https://github.com/Quatre-Finance/Q-paper/blob/main/q_core/faq.md)**

:copyright: Quatrefinance | **[Farm](https://github.com/Quatre-Finance/Q-paper/tree/main/q_farm)** | **[Home](https://github.com/Quatre-Finance/Q-paper#concept-overview)**

