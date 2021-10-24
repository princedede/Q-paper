
## Understand QFOUR Token metrics
**QFOUR** Token (BEP20 : ERC20 standard : Binance smart chain : Ethereum network) is the native token of the QuatreFinance platform with enormously foreseeable use cases deployed and verifiable at [BScscan](http://bscscan.com) : [Etherscan](http://bscscan.com). 

_fig. 1.1_

**Name** | **QFOUR Token**
-------- | ---------------
**Token Type** | **BEP-20**, **ERC-20**
**Ticker(Symbol)** | **QFT**
**Decimals** | **18**
**Max Supply** | **500_000_000** x **10** ** **Decimals**
**Total Supply** | _vary_
**CurrentSupply** | **Total Supply** _(may vary)_

The **QFOUR Token** : initially emmitted from [[Source Address]](http://bscscan.com) at construction time is housed mintable and burnable only by the [[Farm Contract Address]](http://bscscan.com). Total amount of **`QFT`** the farm is able to mint in the contract lifeTime cannot exceed amount of **_Max Supply_** (See fig. 1.1). Access control is enforced on _[special functions]()_ like `burn()` available only to the Farmer is controlled by this _[multisignature account]()_. Such control however does not include the general public methods specified in _[ERC20 Token standard]()_. **QFOUR Token** is built with some internal safety and checks to reduce the risk of losing funds - please refert to our _[API section]()_.

### Token-Burn
We employed this mechanism to compiment the methods we have devised for creating scarcity to bring more value to **QFOUR Token**. As the farm owner, the farmer needs to have more control on what he produces and the quantity in circulation hence the answer to why and who burns token? **QFT** is designed to call for value via its use cases and a special staking algorithm which temporarily mops out token from circulation as need increases and similarly emits when unstaked. Such need is tied to virtually all QuatreFinance products.

The Quatre team will perform periodic burn on a quarterly basis or as the team deem fit which will be communicated in our various channels.

More information on _[how it works]()_.

----------------------

:copyright: Quatrefinance | **[Return to home](https://github.com/Quatre-Finance/Q-paper#concept-overview)**