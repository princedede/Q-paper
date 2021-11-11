
#### How it works: 
----------------------------------

In the Buy and Sell category for example, to keep the system healthy, to create a seller account, user is required to hold `minimumStakeAmount` in **QFT** unstakeable only via a proxy account that will be generated in the process. When the `stake` is called, it switches the farmer to what we termed **_Sedentary mode_**. This is a state of unavailability that does reduces **totalSupply** by the staked amount which is moved to the **_vault_** - balance which is neither spendable nor withdrawable until `minimumStakeDuration` has elapsed (if any).
Just as the mechanism renders the caller's staked balance inactive for the period as long as their proxy account is active, the only way to retrieve the staked balance is when **proxy account** is `closeOut`. To perform this action, user must first put the proxy in an inactive mode, then `unstake` and `closeOut` is performed in a single call. Thereafter, the **`stakedAmount`** is forwarded along with the accrued reward to the staker's EOA. It in-turn increases the amount of token in circulation with the **`stakedAmount`**. One can always verify total **QFT** in circulation from the totalSupply.

`NOTE`: At some point, **`_CurrentSupply_`** may differ from **`_TotalSupply_`**. This however is not an anomally. Activation of tip will cause the two variables to differ.

-------------------------

#### FanTip

We used this term to describe a condition where a holder of **QFT** has not reduce their balance for a period of 30 days at  a stretch. If they decide to withdraw thereafter, they automatically earn 1% of the total idle balance. However it does not apply to the regular balance.  

--------------------------------

**[Previous]()** | **[Next]()**

:copyright: Quatrefinance | **[Home](https://github.com/Quatre-Finance/Q-paper#concept-overview)**