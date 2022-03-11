### QuatreDigesu (Q-Core)
![IMG_20220223_072720 (1)](https://user-images.githubusercontent.com/35783747/157897718-5105cd09-ac12-43b3-8497-4df906247957.png)

<!-- ![IMG_20220223_072700](https://user-images.githubusercontent.com/87430168/155271873-ca4643f1-c4fd-4fca-ad85-8a62607d2529.png) -->

Modelling against a prominent ancient African financial scheme where few people from a community or related settings come together to fund one another by pooling resources passing it rotationally, Quaterfinance **Digesu** aims to uphold the social spirit while providing solutions to the shortcomings. Think of a group of people in a setting who have agreed to peer-fund one another to finance either new business, a project or non-profit endeavors, usually agreeing on a certain rules of participation, pool financial resource together to finance one another in a rotational manner. 

#### Problems
Since money and people are involved, `trust` is a major issue to deal with and questions such as:

- Will the next paticipants fulfill their obligation?
- WIll they pay back in full?
- How do we get our money if they default?
- Do we charge interest or not? etc

#### How we solve it
At Quatrefinance, we harness the potentials of blockchain technology to solve existing or emerging problems in the African societies and globally. Our solutions go beyond connecting the African communities but the world at large. This implies that anyone around the world can participate in the scheme in a decentralized manner. Our software (Digesu) will not only ensure cooperations but also enforces actions to protect the rights of every participants.
To ensure compliance, we introduce a collateral-like system which requires deposit in another crypto currency. 

We represent thus:
- With collaterized:
  **Minimum QFT Holding** = **unit per head** x **Quorum**

- Without collaterized
  **Minimum QFT Holding** = **unit per head** x **Quorum** x **collateral factor**

`NOTE`: The pool admin (creator) may raise the collateral index at creation point. If this happens, the effect will be a correponding raise in the amount of **QFT holding** needed to get financed.



#### How it works
--------------
- Visit the [app page](https://app.quatre.finance)

**1.** **Creating a pool**

  - Strict mode

Assume Bob, Alice and Gorimapa have agreed to set up a pool of three persons to raise funds among themselves with unit amount of **1 BNB** for a total cycle of 15 days. Agreeing to set collateral to 1.2 of the total pool using **BUSD** as the collateral base and an interest of 2%, we then have the following settings to launch a new pool:

  - **Amount** : **1 BNB**.
  - **Quorum** : **3**.
  - **Duration** : **5 days**.
  - **Collateral factor** : **1.2**. 
  - **APR** : **2%**.
  - **Collateral Address** : **BUSD Contract**.
  - **Participants** : **A list of participating addresses**.
  - **AllowExternal** : **false**.

**NOTE**: Setting the flag `allowExternal` to false will restrict anyone other than the broadcasted participants to make deposit to the pool. **As at the time of writing, only non-strict mode is available.**

#### onFinance

Soon as the quorum value is reached, the total pool amount becomes available to the first on the list as preserved at creation time. It continues in a rotational order if there is no default from the previous taker. This sets a temporary lock on their **QFT** holding until the loan is repaid. Participant whose turn is to get financed must possess **QFT** in their wallet of an amount not less than the unit funding multiplied by the **Quorum** (total number of particiants) only if the pool was not collaterized from the onset, otherwise, will not be less than the total pool amount multiplied by the collateral factor.

##### onDefault

Participant who get financed may decide to amortize the loan or pay all at once but must complete the total repayment amount before the duration elapsed. If the otherwise happens, anyone who must be a member of the pool may liquidate the defaulter. In this case, their **QFT** is confiscated and use to set off the loan. 


  - Non-Strict mode

In contrast to the strict mode, the creator may allow anyone to join their pool. This mean, as the creator, you do not have to explicitly add participants to your group. Anyone may select to join in but the initial setting wil slightly change from that of strict mode. Please use the designated function for this purpose. 

-----------------

**2.** **Joining existing pool**

A pool we created in non-strict mode is visible and allowance is set to true for anyone to join.
**NOTE**: Intending participant must have amount in base currency sufficient pay for unit amount plus gas fee (usually minimal).  



**`NOTE :`** _Quatre-finance does not have control over funds in any of the pools. In fact, we have no way to access it_.

---------------------------


#### Participating benefit

At Quatrefinance each pool matters as they help strengthening the protocol. For the participants, activating a pool qualifies them to participate in the farming of **Quatrefinance Token - QFT** while completing a cycle qualifies them to earn farmed reward also as burning mechanism. However, this is not to be confused for reward for staking as the base rate for the former is lesser than latter.

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

