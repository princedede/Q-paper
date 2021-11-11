
### Quatre LandB (Q-LandB)

Similar to **Q-core**, Providers in this category are lenders that singlehandedly provide liquidity in the amount they wish using the _[proxy]()_ - based account configured to their preferences. Here, we do not have a pool of persons but a fairly one-man who decides when to put his fund to use. The lender sets parameters such as the amount, collateral value plus the factor, interest rate, duration and a few other private settings. Going by the proxy pattern, the lender owns up to 50% level of control while rest is shared between the proxy and the borrower. We embedded some checks that analyzes the activities of both parties ensuring interests are protected. For fairness, there can only be one borrower in a round. That is, if for instance, the lender set duration to 14 days of use, then no other borrower will be allowed during this period until the current loan is settled. If the borrower defaults payments after the repayment period lapses, the right to liquidate the borrower remains with the lender. While yet not the reapayment period, lender has no means to put the other party in the liquidation state. However, this category does not qualify them for the Quatre farming reward.
One can also consider a p2p use case scenario where Bob does not want to sell off his **BNB** but need some stable asset, requests to borrow some from Alice. Because of trust issue coupled with the fear of default in payment, Alice may be reluctant to grant such request. With Q-Core, Alice can set up a (_[Proxy]()_) account funded with an amount, thereafter refer Bob to his account in the lenders pool.

Refer to the **[FAQ]()** for more detail.

---------------------------------

**[Previous]()** | **[Next]()**

:copyright: Quatrefinance | **[Home](https://github.com/Quatre-Finance/Q-paper#concept-overview)**