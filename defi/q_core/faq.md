#### FAQ - Q-core

- **What is a session?**
This is a period of not greater than 7 days i.e period from the time fund was released to repayment period.

- ### What are public and private bands?

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

----------------------------


**[Previous](https://github.com/Quatre-Finance/Q-paper/blob/main/defi/q_core/QuatreDigesu.md)**

:copyright: Quatrefinance | **[Home](https://github.com/Quatre-Finance/Q-paper#concept-overview)**
