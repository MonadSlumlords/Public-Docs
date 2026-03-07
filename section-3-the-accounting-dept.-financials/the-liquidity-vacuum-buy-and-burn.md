# 🌪️ The Liquidity Vacuum: Buy-and-Burn

**"Inflation is a tax on the lazy. Deflation is a weapon for the active."**

Welcome to the heavy machinery, Junior. In most Web3 ecosystems, reward tokens inevitably hyper-inflate because the emissions from staking outpace the utility sinks. Slumlords OS solves this entirely by turning every single property and upgrade mint into a hyper-deflationary market event.

This is not a passive, lazy burn mechanism where tokens are just sent to a dead address and forgotten. The `GAME_NFT` and `UPGRADE_NFT` smart contracts act as automated, aggressive trading bots. They actively sweep the liquidity pool to suffocate the circulating supply of `$RENT` while simultaneously enforcing constant, unyielding buy pressure.

Here is the exact step-by-step anatomy of what happens on the Monad blockchain the moment a Slumlord hits "MINT".

***

## 🗜️ 1. The Dual-Asset Squeeze (The Entry Toll)

To execute a public mint or buy a shiny new upgrade, the protocol forces the operator to provide two separate assets upfront:

* A base fee in **MON**.
* A specific token fee in **$RENT**.

Because `$RENT` is required just to play the game, prospective slumlords must constantly interact with the decentralized exchange to acquire it, creating a strong organic baseline of trading volume. But the true macroeconomic lever is what our contract does with these assets once it gets its hands on them.

***

## ⚙️ 2. The Smart Contract Execution Sequence

When the transaction is submitted, the contract autonomously triggers its internal protocol, executing the following chain of events in a single, brutal block:

{% stepper %}
{% step %}
### Step A — The Seizure

The contract takes absolute custody of the `$RENT` tokens you just paid for the mint requirement.
{% endstep %}

{% step %}
### Step B — Brokerage Extraction

The protocol calculates and extracts a standard operational brokerage fee from your raw **MON** payment to fund "ongoing network operations" (the C-Suite yacht fund).
{% endstep %}

{% step %}
### Step C — The Market Sweep (The Pump)

The protocol takes the entirety of your remaining **MON** and instantly wraps it into **WMON**. It then routes this capital directly into the decentralized exchange and executes an automated market-buy, purchasing `$RENT` directly off the liquidity pool at live market rates.
{% endstep %}

{% step %}
### Step D — The Deflationary Nuke (The Burn)

The contract now holds two massive pools of `$RENT`: the tokens you originally paid, and the fresh tokens it just bought from the DEX. The contract targets its total `$RENT` balance and permanently calls the `burn` function, completely erasing all of those tokens from the total circulating supply.
{% endstep %}
{% endstepper %}

***

## 📈 The Macroeconomic Consequence

Read that carefully. By forcing market buys directly from the liquidity pool with the user's MON _before_ destroying the tokens, every single mint acts as an automated, price-positive market order. We literally use their own entry fee to pump the token, and then we burn the evidence.

As player acquisition scales, the constant demand for real estate and upgrades forces the protocol to continuously sweep the `$RENT/WMON` pool. This sustains upward price pressure via the automated buys while mathematically suffocating the circulating supply via the burn, intensely rewarding the Slumlords who hold optimized, yield-generating portfolios.
