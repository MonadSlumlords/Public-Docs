# 🏦 The Vault: Staking, Fatigue & Taxes

Welcome back to the terminal, Junior Associate. Acquiring assets is only step one. At **BlackCoq**, an idle asset is a fireable offense. If you aren't actively draining a property's value, you are losing us money.

Here is your manual for the `PORTFOLIO.EXE` interface, where we turn concrete and misery into liquid $RENT.

***

## 🏦 Portfolio & Staking (The Vault)

The Portfolio module acts as your central staking vault, visualized in the `PORTFOLIO.EXE` interface. Real estate held in your local `WALLET` tab generates zero yield; it is dead capital.

To begin extracting `$RENT`, properties must be moved to the `STAKED` ledger, depositing them into the `PORTFOLIO` smart contract to initiate the yield accrual process. Once staked, the terminal provides real-time tracking for each unit's individual Yield, Fatigue, and Net Tax metrics.

***

## 📊 Staking Capacity Limits

The protocol strictly regulates portfolio sizes via the `STAKING_CAPACITY` monitor.

* **The Intern Cap:** All slumlords start with a hardcoded maximum staking capacity of 10 properties.
* **Corporate Ladder:** To scale beyond the initial limit, slumlords must allocate Skill Points into the "Staking Expansion" parameter.
* **The Ceiling:** You can allocate a maximum of 5 Skill Points to Staking Expansion. Each point permanently adds 2 staking slots, bringing the absolute maximum portfolio size to 20 active properties.

***

## 🏚️ Fatigue & Maintenance Mechanics (The Slumlord Tax)

Buildings degrade, tenants complain, and pipes burst. Once staked, properties begin accumulating "Fatigue" linearly over time, acting as a direct throttle on your gross extraction rate.

* **The Condemnation Threshold:** Fatigue will continuously accrue until it hits a hardcoded ceiling of 99% (`9900 BPS`). At this threshold, the property is effectively condemned, generating near-zero base yield. (At BlackCoq, we market this to new renters as "rustic, open-air living".)
* **The Extortionate Repair Bill:** Fixing a property is not a flat rate. The `RESET FATIGUE` operation calculates exactly 15% of your portfolio's modified base yield to execute the repair.

***

## 💊 Consumable Protocols (Temporary Steroids)

For those times when you need to juice the quarterly numbers, slumlords can purchase 24-hour consumables to temporarily manipulate their economic output. The `$RENT` cost for these actions scales dynamically with the size of your portfolio.

* **Slow Fatigue:** Activating this operation injects a 24-hour protocol that reduces your global fatigue accumulation rate by 10%.
* **Boost Yield:** This steroid protocol artificially inflates your portfolio's base yield by +20% for a strict 24-hour period.

***

## 🔥 The Protocol Tax Siphon & Deflationary Burn

At BlackCoq, the house always wins. Yield is not free, and the `PORTFOLIO` contract enforces a heavy maintenance tax on all extracted yield.

* **The Baseline Siphon:** The protocol extracts a baseline tax of 25% from your gross property yield, which can fluctuate wildly based on district Zone Modifiers and active Synergies.
* **Skill Point Mitigation:** By allocating Skill Points into "Tax Reduction," slumlords can permanently reduce their effective maintenance tax by 3% per point, up to a maximum reduction of 15%.
* **The Incinerator:** This extracted tax is not returned to a developer treasury; instead, the entirety of the taxed `$RENT` is processed through the protocol's automated distribution system to permanently burn tokens. This acts as a massive deflationary sink for the circulating supply.
