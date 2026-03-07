# 🧮 The Quants: Raw Protocol Math

**"Trust the ledger, verify the math."**

Welcome to the basement, Junior. For slumlords building custom projection models, automated tracking scripts, or simply trying to optimize their capital deployment to the exact decimal, this section exposes the raw underlying mathematics hardcoded into the Slumlords OS smart contracts.

At BlackCoq, we don't rely on luck. We rely on algorithmic extortion.

***

## 📈 1. The Acquisition Bonding Curves (Extortion Economics)

The protocol utilizes two distinct bonding curves to price assets, heavily penalizing late adopters and rapid scaling.

**Property Mint Pricing (The Step-Curve)**\
Real estate costs escalate based on district density. The contract increases the base **MON** and `$RENT` minting cost by exactly 25% for every 5,000 units minted. Because the smart contract calculates this via an integer loop rather than continuous compound interest, the formula is a strict, brutal step function.

Let n be the total number of properties minted. The cost C is calculated as: $$C(n) = C_{base} \times (1.25)^{\lfloor \frac{n}{5000} \rfloor}$$

**Skill Point Pricing (The Quadratic Bribery Curve)**\
Skill point acquisition utilizes a harsh quadratic curve to prevent early whales from immediately maximizing their operator stats and buying out the city council on day one.

Let x be the current number of lifetime skill points owned. The cost to acquire the next single point is: $$C(x) = 50 \times (x + 1)^2 \text{ RENT}$$

If purchasing a batch of points k, the total transaction cost is the sum of the sequence: $$C_{batch} = \sum_{i=1}^{k} \left[ 50 \times (x + i)^2 \right]$$

***

## ⚙️ 2. The Yield Engine (Order of Operations)

Calculating your exact daily extraction rate requires following the strict order of operations hardcoded into the contract. Yield modifiers are multiplicative, not additive, meaning your corporate buffs stack aggressively.

{% stepper %}
{% step %}
### Combined Base

Add the property's raw tier yield to the sum of all attached upgrades.

$$Y_{gross} = Y_{base} + \sum Y_{upgrades}$$
{% endstep %}

{% step %}
### Fatigue Penalty

Apply the current structural decay. (A degraded property drags down the upgrade yield, too).

$$Y_1 = Y_{gross} \times \left(1 - F_{current}\right)$$
{% endstep %}

{% step %}
### Skill & Consumable Modifiers

Apply operator buffs (Max +25% from skills, +20% from consumables).

$$Y_2 = Y_1 \times \left(1 + B_{skills} + B_{consumable}\right)$$
{% endstep %}

{% step %}
### Zone Modifier

Apply the district's hardcoded yield variance.

$$Y_3 = Y_2 \times \left(1 + B_{zone}\right)$$
{% endstep %}

{% step %}
### Pairing Synergy

Finally, apply any active network pairings from your collusion matrix.

$$Y_{final} = Y_3 \times \left(1 + B_{pairing}\right)$$
{% endstep %}
{% endstepper %}

***

## 🏚️ 3. The Fatigue Decay Vector (Planned Obsolescence)

Properties do not degrade daily; they degrade by the second. The `PORTFOLIO` contract utilizes a `FATIGUE_RATE_PER_SECOND_BPS` constant of 764.

Without any skill points or consumables mitigating the damage, a property accrues roughly **66.0% fatigue per 24 hours** ($86400 \text{ seconds} \times 764 \text{ BPS} / 10000$). We essentially built the buildings out of wet cardboard.

The effective rate of decay R\_{eff} is mitigated by your operator attributes: $$R_{eff} = 764 \times \left( 1 - (B_{skill} + B_{consumable}) \right)$$

Therefore, the exact fatigue percentage F(t) at any given time Δt (in seconds) since the last reset is: $$F(t) = \min\left(0.99, F_{0} + \frac{\Delta t \times R_{eff}}{10000}\right)$$

_(Note: The contract hardcaps structural fatigue at 99%, or 9900 BPS. We have to keep it at 99% instead of 100% so the yield doesn't go completely negative, preventing a scenario where the protocol accidentally owes the tenants money.)_

***

## 🩸 4. The Net Tax Siphon (The House Cut)

The protocol extracts a baseline maintenance tax of 25% (2500 BPS) from all extracted yield. However, this is heavily modified by your skill allocations and the specific district the property resides in.

The net tax rate T\_{net} for a specific property is calculated as: $$T_{net} = 0.25 - \left(Points_{tax} \times 0.03\right) + M_{zone\_tax} + M_{pairing\_tax}$$

If your modifiers (like the Offshore Shuffle synergy) push the tax rate below 0%, the contract safely floors the tax at 0%.

The protocol automatically splits the final gross yield according to this percentage. You receive your portion, and the T\_{net} portion triggers the automated protocol burn event, permanently removing that `$RENT` from the circulating supply. The house always gets its cut, but at least we set it on fire afterward.
