### THE FARM

The maximum supply of **QFOUR Token** of which `80%` is minted and `20%` percentage is anonymized at construction time which sets the totalSupply to 8 of 10 of _500,000,000_ **QFT**. See the _[tokenomics]()_ for details.

------------------------------

#### What user can do with the farm

- Stake **QFT** to earn more **QFT**.
- Check pending reward.
- ApproveAndStake: this allows user to stake from their locked balances. _[See more information on how balances work]()_
- Unstake their **QFT**.

Majority of the functions are administative. They can only be called by an authorized address designated to the **[Quatre multisig account]()** which may later transform to a governance account. Some of these administative utilities are geared towards proper and effective administration staking, perform burn, toggle token movement switch in the event that may warrant it hence the transfer may be paused where an emergency situation arises. The decision toggle transfer control switch is stripped from the deployer and given to the multisig to preserve trust. 

--------------------------

#### How to stake

User should have: 
- Enough **QFT** balance greater than the minimum stake threshold.
- A minimal amount of ETH or AVAX to pay for network fee.
- Click on the `stake(amount)` function with an amount.

`Note`: If an user already has stake running, and call the **stake** again, the previous is unstaked, reward (if any) will be added to pending reward balance and both the new and old amounts are summed and restaked.

:copyright: Quatrefinance | **[Return to home](https://github.com/Quatre-Finance/Q-paper#concept-overview)**