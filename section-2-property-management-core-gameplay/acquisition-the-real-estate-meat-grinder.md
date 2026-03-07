# 🥩 Acquisition: The Real Estate Meat Grinder

**"Buy land, Junior. They aren't making any more of it, and the people need somewhere to sleep before their shift at the wagie factory."**

**Overview**\
To generate yield, you must first acquire real estate. The smart contract strictly caps the global property supply at 20,000 units. Assets can be acquired through two distinct operational phases: the Whitelist Mint (for the well-connected) and the Public Offering (for the masses).

***

## 🎟️ Whitelist Phase: The VIP Backroom & Liquidity Generation

Before executing a priority mint, slumlords must secure authorization by purchasing a Whitelist Spot. We don't just hand these out; you have to pay for the privilege of being a Slumlord.

* **Strict Supply Cap:** The protocol hardcaps whitelist access to exactly 250 spots.
* **The Entry Fee:** Purchasing a spot requires a flat, upfront fee of **1500 MON**.
* **Strategic Advantage (Nepotism):** Securing a spot locks in your actual property minting cost at a fixed, discounted rate of **1125 MON** per unit (up to 10 max). Compare this to the Public Offering, which starts at a base price of 1500 MON and rapidly scales up by 25% every 5,000 mints. More importantly, whitelist access grants you total immunity from the $RENT token burn requirement that heavily penalizes public minters.
* **Liquidity Pool Routing:** What happens to that massive 1500 MON entry fee? 100% of the MON raised from selling these 250 spots is routed directly to the DEX to deploy and heavily back the initial $RENT/WMON liquidity pool. We literally use your entry fee to build the casino.

***

## 🥩 Operational Protocol: Public Offering (The Meat Grinder)

Once the protocol's scheduled deployment time is reached, the contract automatically unlocks the Public Offering phase. The public mint operates against the hard global cap of 20,000 properties.

### The Algorithmic Market Sweep (Buy-and-Burn)

The public mint isn't just a sale; it's a hardcoded supply-shock weapon. When a public slumlords mints a property, they must pay both a MON fee and a $RENT token fee. The smart contract autonomously performs the following sequence:

{% stepper %}
{% step %}
### 1. The Brokerage Cut

Exactly 5% (500 BPS) of the MON payment is extracted for BlackCoq corporate operations.
{% endstep %}

{% step %}
### 2. The DEX Nuke

The remaining **95%** of the MON is instantly wrapped into WMON, pushed to the decentralized exchange router, and used to market-buy $RENT directly off the liquidity pool at live rates.
{% endstep %}

{% step %}
### 3. The Incinerator

The contract then takes _all_ the $RENT it just bought off the market—plus the $RENT the user paid as their mint fee—and calls the burn function, permanently destroying it all in a single transaction.
{% endstep %}
{% endstepper %}

This mechanism mathematically guarantees that every single public mint acts as an automated, unstoppable market order. We literally use 95% of their purchase money to pump our own token, and then we burn the evidence.

***

## 📈 Dynamic Pricing Tiers (The FOMO Curve)

The cost of real estate increases with district density. We use a predatory step-based bonding curve that triggers every 5,000 properties minted.

When the current supply crosses into a new bracket, a pre-calculated cost escalation of exactly 25% (2500 BPS) will activate for both the MON and $RENT costs. Slumlords who deploy capital early secure assets at a significantly lower overhead than late adopters. If you wait, you pay the premium.

***

## 🎲 Tier Rarity: The Zoning Lottery

When the mint protocol is initiated, the contract utilizes on-chain entropy to determine the property's Tier, which dictates its economic output and renovation potential:

* **Tier 1 (T1) - The Shoebox:** The standard unit. (75% Probability).
* **Tier 2 (T2) - The "Luxury" Studio:** Upgraded base yield + 3 Upgrade Slots. (20% Probability).
* **Tier 3 (T3) - The C-Suite Penthouse:** Maximum base yield + 4 Upgrade Slots. (5% Probability).
