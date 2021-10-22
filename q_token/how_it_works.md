
#### How it works: 
----------------------------------

In the Buy and Sell category for example, to keep the system healthy, a user who needs to create a seller account is required to hold `minimumStakeAmount` in **QFT** unstakeable only via a proxy account that will be generated in the process. When the `stake` is called, it switches the farmer to what we termed **_Sedentary mode_**. This is a state of unavailability that does reduces **totalSupply** by the staked amount. The balance is reflected in the **_allowances_** of farmer to the source contract - balance which is neither spendable nor withdrawable. 
Just as the mechanism renders the caller's staked balance inactive for the period as long as their proxy account is active, the only way to retrieve the staked balance is when **proxy account** is `closeOut`. To perform this action, user must first put the proxy in an inactive mode, then `unstake` and `closeOut` is performed in a single call. Thereafter, the **`stakedAmount`** is forwarded along with the accrued reward to the staker's EOA. It in-turn increases the amount of token in circulation with the **`stakedAmount`**. One can always verify total **QFOUR** Token in circulation from the source totalSupply.

`NOTE`: At some point, **`_CurrentSupply_`** may differ from **`_TotalSupply_`**. This however is not an anomally. Activation of fanTip will cause the two variables to differ.
