### THE FARM

------------------------------

#### What you can do in the farm

- Stake **QFT** to earn more **QFT**.
- Check pending reward.
- Unstake their **QFT**.

Majority of the functions are administative. They can only be called by an authorized address designated to the **[Quatre multisig account]()** which may later transform to a governance account. Some of these administative utilities are geared towards proper and effective administration on staking, burn etc. The decision to toggle transfer control switch is stripped from the deployer and given to the multisig to preserve trust. 

--------------------------

#### How to stake

User should have: 
- Enough **QFT** balance greater than the minimum stake threshold.
- A minimal amount in network asset to pay for fee (usually, this is very small).
- Click on the `stake(amount)` function with an amount.

`Note`: If an user already has stake running, and call the **stake** again, the previous one is unstaked, reward (if any) will be added to pending reward balance and both the new and old amounts are summed up and restaked.

----------------
**[API](https://github.com/Quatre-Finance/Q-paper/blob/main/q_farm/API.md)** | **[Q-Lend](https://github.com/Quatre-Finance/Q-paper/tree/main/q_lend)**

:copyright: Quatrefinance | **[Home](https://github.com/Quatre-Finance/Q-paper#concept-overview)**
