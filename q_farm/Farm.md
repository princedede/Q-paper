### THE FARMER

The maximum supply of **QFOUR Token** is pre-minted to the Farmer at construction time which sets the totalSupply to zero hence **QFT** is mintable. The initial amount of _500,000,000_ **QFT** was planted in the Farmer's contract and only the farm has the knowledge of it. Each time an amount is minted, an external call is performed which subsequently increased the totalSupply in the source contract as well as the currentSupply from the farmer itself. The Farmer only reserves the authorization to mint **QFT** controlled initially by the deployer later switched to this **[multisig account]()**.

------------------------------

#### What user can do with the farmer

- Stake their **QFT** to earn more **QFT**.
- Check pending reward.
- ApproveAndStake: this allows user to stake from their locked balances. _[See more information on how balances work]()_
- Unstake their **QFT**.

Majority of the functions are administative. They can only be called by an authorized address designated to the **[Quatre multisig account]()** which may later be transformed to a governance account. Some of these administative utilities are geared towards giving the farmer access to administer staking, perform burn, toggle token movement switch in the event that may warrant it hence the transfer may be paused where in some emergency situation. The decision and power to pause or unpause transfer is stripped from the deployer and is given to the multisig address(later to governance) to preserve trust. 



**[Return to home](https://github.com/Quatre-Finance/Q-paper#concept-overview)**
