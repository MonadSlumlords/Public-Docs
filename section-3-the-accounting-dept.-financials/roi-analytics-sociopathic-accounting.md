# 📉 ROI Analytics: Sociopathic Accounting

Welcome to the Accounting Department, Junior Associate. At **BlackCoq**, we don't manage portfolios based on "gut feelings" or "tenant well-being." In the Slumlords ecosystem, your yield is a rapidly decaying asset. If you simply stake your properties and walk away, the protocol's degradation mechanics will bleed your portfolio dry.

The Finance module is your automated accounting department. It pulls live on-chain data to mathematically prove whether your current management strategies are actually generating profit or just burning gas.

***

## 💰 Treasury Reserves.SYS (Live Capital Tracking)

This module tracks your exact liquid capital across all vectors.

* **The Oracle Ping:** We don't rely on lagging third-party APIs. The OS pings the decentralized exchange's factory contract directly, reading the `reserve0` and `reserve1` ratios of the `$RENT/WMON` liquidity pool to calculate the real-time USD value of your holdings.
* **Total Ledger:** Your reserves combine your hard wallet balance with your accumulated, unclaimed pending yield currently sitting inside the `PORTFOLIO` contract.

{% hint style="info" %}
Live on-chain reserve reads ensure treasury valuations reflect real-time DEX liquidity ratios rather than stale price feeds.
{% endhint %}

***

## 📉 Maintenance ROI Analyzer (The 15% Rule)

Resetting fatigue is not a flat fee; the smart contract charges you exactly 15% of a property's modified daily base yield to execute a repair. This analyzer prevents you from making catastrophic management errors.

* **The Rookie Trap:** Constantly repairing a property at 2% fatigue is a net negative action because the 15% repair fee vastly outweighs the 2% yield you are losing.
* **Est. Payback Period:** The OS calculates exactly how many days it will take for the recovered yield (the yield you get back by resetting fatigue to 0%) to pay off the 15% reset cost.
* **Actionable Directives:** The system will explicitly instruct you to **DEFER MAINTENANCE** if the payback period is mathematically unfavorable. It will only flash a red **RESET FATIGUE** warning when your daily losses to degradation justify the immediate expenditure.

{% hint style="warning" %}
Do not manually repair properties without consulting the analyzer — frequent low-impact repairs drain reserves due to the fixed 15% reset cost.
{% endhint %}

***

## 💉 Yield Boost Analyzer.EXE (Consumable Arbitrage)

Evaluates the profitability of purchasing the 24-hour Yield Consumable steroid.

* **The Math:** Activating this protocol artificially inflates your portfolio's base yield by exactly +20% (`2000 BPS`) for 86,400 seconds. However, the cost to activate it scales dynamically with your portfolio size.
* **The Verdict:** The analyzer runs the math: _Will the extra 20% yield generate more `$RENT` than the cost to activate the consumable?_ If the Net Daily Profit is positive, the system recommends you **ACTIVATE BOOST**. If it is negative, you must **DEFER BOOST**.

***

## 🧾 P\&L Statement (24H Ledger)

A brutal, transparent look at your 24-hour extraction efficiency.

* **Gross Base Yield:** Your maximum theoretical income (Base Property Yield + Total Attached Upgrade Yield).
* **Avg Fatigue Impact:** The exact percentage of your gross yield currently being lost to structural degradation.
* **Effective Tax Rate:** The protocol tax actively being siphoned from your earnings. The base rate is 25%, but this ledger reflects your actual rate after accounting for Skill Point deductions ("Tax Reduction") and active District Synergies.
* **Net Take-Home Yield:** Your actual extracted profit after the protocol burns your taxes and penalizes your fatigue.

***

## 🔮 Revenue Projections (Forward-Looking Yield)

This matrix extrapolates your current daily Net Yield across 7-day (Weekly), 30-day (Monthly), and 365-day (Yearly) time horizons, denominated in both raw `$RENT` tokens and their estimated Fiat (USD) equivalent.

* **The Zero-Drift Caveat:** The OS projection engine is static. It assumes a _0% Fatigue Drift_ and perfectly stable market conditions. In reality, your properties are degrading every second. If you neglect your maintenance schedule and let fatigue climb, your actual revenue will aggressively underperform these projections.

{% hint style="danger" %}
Projections are optimistic baselines — they do not model ongoing degradation. Treat them as theoretical ceilings, not guaranteed income.
{% endhint %}

***

## 🏢 Asset Allocation & Capital Density

Real estate that isn't generating yield is dead weight. This module provides a real-time snapshot of your portfolio utilization.

* **Properties Owned:** Your total acquired real estate units across all wallets.
* **Active Portfolio:** Your current staking utilization rate versus your hardcoded max capacity (e.g., 10/10).
* **Installed Upgrades:** A raw count of active renovation modules attached to your staked properties. Because your portfolio size is strictly capped, maximizing this number is the only way to scale your empire vertically.

{% hint style="info" %}
Monitor utilization closely — unused capacity and uninstalled upgrades are opportunity costs in a capped portfolio.
{% endhint %}
