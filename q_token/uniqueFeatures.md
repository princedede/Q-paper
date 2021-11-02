#### Some unique features of QFOUR Token
----------------------------------------
In development...


<!-- - **`getBalances`** : We adopted a dual internal ledger to administer users' balances. Holders can choose to transfer their funds in two ways thus: via **ERC20 transfer standard** and alternatively **`locked Balance`** (a bit different from the traditional method specified in the _[ERC20 standard]()_). To use the locked feature, holder of **QFT** must explicitly call the `lockBalance` function with an `amount`, an `escape address` and `lock period` (in days). The user's regular balance is reduced by the specified amount and added to the locked balance. Calling `balanceOf(acount)` returns aggregate balance of **account**. if for any reason `unlockBalance` is called before the locked period elapse, a suspicious flag is raised which set off the user's balances and forwards it to an **escape address** previously set. 

Holder can choose to set **escape address** to `0x0000000000000000000000000000000000000000` notifying the nrtwork they do not wish to have an escape address set. If `unlockBalance` is called before the locked time finishes and no escape address was set, the transaction is reverted to previous state. Explicitly locking the balance with an escape address may help user regain their token if their account is compromised and the attacker is unaware of the unlock period since `transfer` only concerns itself with regular balances. 

------------------------

Let's examine a scenario where **Bob** receives 1000 `QFT` for the first time. **Bob** obviously does not have lock set. His regular balance is updated to 1000 `QFT` while locked balance is set to 0. If Bob decides to transfer 500 `QFT` to **Alice**, they can do so by simply calling `transfer(aliceAddress, amount)` and the usual transfer is done. 

Subsequent action will be reflected in a new state where _Bob's_ regular balance is now 500 `QFT`, regular becomes 0. If the recipient (_Alice_) already has lock set, her new state will cause her regular balance to remain unchanged while the locked balance is increased by the transferred amount.
<!-- 
A potential use case (A foreseable feature of Q-Wallet) is where an attacker successfully gained access to holder's externally owned account (EOA). If the user already set a lock on their fund and have it reside in the locked ledger balance, it becomes useless for the attacker as they cannot effect a transfer unless the passlock is provided. But in this case, the regular ledger becomes a victim. At any time, a holder can choose to lock the entire balances until they are ready to make another transaction or simply unlock an amount they wish to transfer at that point. -->

<!-- **Note the difference**
If a holder calls the `safeSignedTransfer` with the correct _'lock'_ and _'amount'_, the value of an _'amount'_ is deducted from the aggregate balance, send to recipient and the aggregate balance left is locked. -->

<!-- Alternately, a holder can use the `lockBalance` to move specific amount to the locked ledger or `unlockBalance` to move an amount to the regular ledger. The traditional _`transfer(sender, recipient, amount)`_ utility simply moves an amount from the sender's regular balance to the recipient's locked balance if they have lock in place otherwise effect change to the regular balance. For more information, please refer to the  _[API section]()_. --> -->

-------------------
:copyright: Quatrefinance | **[Return to home](https://github.com/Quatre-Finance/Q-paper#concept-overview)**