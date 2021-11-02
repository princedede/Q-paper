
## Understand QFOUR Token metrics
**QFOUR** Token (ERC20 standard : Avalanche network) is the native token of the QuatreFinance platform with enormously foreseeable use cases deployed and verifiable at [Avascan](http://bscscan.com) : [Bscscan](http://bscscan.com). 

_fig. 1.1_

**Name** | **QFOUR Token**
-------- | ---------------
**Token Type** | **BEP-20**, **ERC-20**
**Ticker(Symbol)** | **QFT**
**Decimals** | **18**
**Max Supply** | **500_000_000** x **10** ** **Decimals**
**Total Supply** | _vary_
**CurrentSupply** | **Total Supply** _(may vary)_

The **QFOUR Token** : initially emmitted from [[Source Address]](http://bscscan.com) at construction time is housed mintable and burnable only by the [[Farm Contract Address]](http://bscscan.com). Total amount of **`QFT`** the farm is able to mint in the contract lifeTime cannot exceed amount of **_Max Supply_** (See fig. 1.1). Access control is enforced on _[special functions]()_ like `burn()` available only to the Farm is controlled by _[multisignature account]()_. Such control however does not include the general public methods specified in _[ERC20 Token standard]()_. **QFOUR Token** is built with some internal safety and checks to mitigate against losing funds - please refert to our _[API section]()_.

### Token-Burn
We employed this mechanism to compliment the methods we have devised for creating scarcity to bring more value to **QFOUR Token**. Based on our model, the farm needs to have more control on supply in circulation. **QFT** is designed to call for value via its use cases and a special staking algorithm which temporarily mops out token from circulation as need increases and similarly emits when unstaked. Such need is tied to virtually all QuatreFinance products.

The Quatre team will perform periodic burn on a quarterly basis or as the team deem fit which will be communicated in our various channels.

More information on _[how it works]()_.

----------------------

:copyright: Quatrefinance | **[Return to home](https://github.com/Quatre-Finance/Q-paper#concept-overview)**