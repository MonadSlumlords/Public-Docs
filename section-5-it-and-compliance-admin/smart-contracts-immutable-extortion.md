# 💻 Smart Contracts: Immutable Extortion

**"Trust the ledger, verify the extortion."**

Welcome to the IT department, Junior. Slumlords OS is fully decentralized, which is corporate speak for "if something breaks, it's your fault, not ours."

The retro-terminal client you interact with is simply a visualizer for the underlying logic executing at blistering speeds on the **Monad** parallel EVM. For operators building custom MEV bots, automated extraction scripts, or for the paranoid auditors trying to find a loophole in our tax code (don't bother, we wrote it), the official contract architecture is detailed below.

{% stepper %}
{% step %}
### GAME\_NFT (`NFT.sol`) — "The Zoning Board"

* **Standard:** ERC-721 Enumerable
* **Function:** Handles base property generation, tier logic (T1/T2/T3), district zone assignment, and the dual-asset minting logic.
* **The Malice:** Enforces the strict 20,000 maximum supply cap and executes the automated 95% DEX liquidity routing. This is the contract that takes your **MON**, market-buys `$RENT`, and sets it on fire right in front of you.
{% endstep %}

{% step %}
### UPGRADE\_NFT (`Upgrade.sol`) — "The Renovation Racket"

* **Standard:** ERC-721 Enumerable
* **Function:** Handles the sequential minting of the 20-tier property renovation catalog.
* **The Malice:** Strictly enforces the manufactured scarcity of our tech tree. It mathematically guarantees that the "Penthouse Suite" upgrades remain hyper-scarce, while simultaneously mirroring the predatory 95% DEX sweep found in the base property contract.
{% endstep %}

{% step %}
### PORTFOLIO (`Portfolio.sol`) — "The Collection Agency"

* **Standard:** Custom Staking Vault
* **Function:** The central economic engine of BlackCoq. This vault escrows your staked properties and securely bolts your upgrade tokens to them.
* **The Malice:** Calculates and distributes your `$RENT` yield down to the second. It ruthlessly enforces the 764 BPS fatigue decay rate, automatically siphons the 25% base protocol tax, and manages all operator Skill Point logic and Synergy combinations. This contract is your boss.
{% endstep %}

{% step %}
### GAME\_TOKEN (`$RENT`) — "The Federal Reserve"

* **Standard:** ERC-20 Burnable
* **Function:** The utility and extraction token of the ecosystem.
* **The Malice:** Minted exclusively by the `PORTFOLIO` contract to pay your yield; aggressively and permanently burned by every other contract in the ecosystem to artificially pump the bags of the C-Suite.
{% endstep %}

{% step %}
### LIQUIDITY\_ROUTER — "The Laundromat"

* **Standard:** `IUniswapV2Router02`
* **Function:** The external decentralized exchange protocol operating on Monad utilized natively by the Slumlords OS to seamlessly swap between **WMON** and `$RENT`.
{% endstep %}
{% endstepper %}

{% hint style="info" %}
### 🔒 Security & Access Control (Why You Can't Hack Us)

We might be a morally bankrupt corporation, but our code is ironclad.

* **Reentrancy Protection:** All critical financial functions (minting, staking, claiming, purchasing upgrades) are protected by standard `nonReentrant` modifiers. We know you degenerates will try to execute recursive withdrawal attacks. We already blocked them. We are the only ones allowed to steal here.
* **No Pausable Ejection:** The `PORTFOLIO` contract does not feature arbitrary pausing mechanisms. The developers cannot lock your staked NFTs, and we cannot freeze the game. Why? Because pausing the game means pausing the yield taxes and the token burns. We want the extraction machine running 24/7/365. You can unstake your assets and return them to your dead wallet at any time.

Read the contracts. Understand the flow of capital. And get back to work.
{% endhint %}
