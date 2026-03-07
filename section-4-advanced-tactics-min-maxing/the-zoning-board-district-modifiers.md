# 🏙️ The Zoning Board: District Modifiers

**"Location is everything. If you build a penthouse in a desert, you still only get sand."**

Welcome to the city planner's office. When you execute a mint on Monad, your property is randomly assigned to one of 12 distinct geographic zones via on-chain entropy. These zones are not cosmetic flavor text; they act as hardcoded economic modifiers that drastically alter how your property performs inside the `PORTFOLIO` staking contract.

Some districts are highly lucrative but will literally rot away in days due to massive fatigue modifiers. Others offer terrible base yield but feature heavily subsidized protocol tax rates. A true slumlord builds a portfolio that weaponizes these extremes.

***

## 🏙️ The District Directory (Zone Modifiers)

Every property inherits a baseline yield based on its Tier, a base protocol tax of 25%, and a baseline fatigue decay rate. The district your property resides in applies flat percentage increases or decreases to these base metrics.

{% stepper %}
{% step %}
### Foreclosure Fields

High turnover, reliable extraction. The banks do the dirty work for you, but the locals are restless.

* **Yield Modifier:** +10% (`+1000 BPS`)
* **Fatigue Modifier:** +10% (`+1000 BPS`)
* **Tax Modifier:** +15% (`+1500 BPS`)
{% endstep %}

{% step %}
### Eviction Alley

A desolate strip. It's nearly impossible to squeeze rent out of these tenants, but the protocol essentially ignores you when it comes time to collect taxes.

* **Yield Modifier:** -15% (`-1500 BPS`)
* **Fatigue Modifier:** 0%
* **Tax Modifier:** -15% (`-1500 BPS`)
{% endstep %}

{% step %}
### Gentrification Gardens

The crown jewel of immediate extraction. You can hike the rent to the moon, but the faux-luxury builds degrade incredibly fast.

* **Yield Modifier:** +20% (`+2000 BPS`)
* **Fatigue Modifier:** +15% (`+1500 BPS`)
* **Tax Modifier:** +10% (`+1000 BPS`)
{% endstep %}

{% step %}
### Mortgage Mountain

Solid returns, but the protocol levies a heavy maintenance tax on properties located at this elevation.

* **Yield Modifier:** +10% (`+1000 BPS`)
* **Fatigue Modifier:** +5% (`+500 BPS`)
* **Tax Modifier:** +20% (`+2000 BPS`)
{% endstep %}

{% step %}
### Rentpayer's Ravine

The definition of average. Modest buffs across the board with no catastrophic drawbacks. Perfect for the uninspired middle-manager.

* **Yield Modifier:** +5% (`+500 BPS`)
* **Fatigue Modifier:** +10% (`+1000 BPS`)
* **Tax Modifier:** +5% (`+500 BPS`)
{% endstep %}

{% step %}
### Subprime Suburbia

A predatory paradise. Good yield, but the protocol knows you're over-leveraged and taxes you into oblivion to compensate.

* **Yield Modifier:** +10% (`+1000 BPS`)
* **Fatigue Modifier:** +5% (`+500 BPS`)
* **Tax Modifier:** +25% (`+2500 BPS`)
{% endstep %}

{% step %}
### Default Desert

A barren wasteland of broken dreams. Awful yield, but because nobody lives here, the property barely degrades.

* **Yield Modifier:** -10% (`-1000 BPS`)
* **Fatigue Modifier:** -5% (`-500 BPS`)
* **Tax Modifier:** -10% (`-1000 BPS`)
{% endstep %}

{% step %}
### Landlord Lagoon

A premium coastal trap. Incredible yields, but saltwater erosion and high municipal taxes will eat into your margins.

* **Yield Modifier:** +15% (`+1500 BPS`)
* **Fatigue Modifier:** +10% (`+1000 BPS`)
* **Tax Modifier:** +20% (`+2000 BPS`)
{% endstep %}

{% step %}
### Tax Haven Terrace

An offshore exploit. It doesn't generate massive rent, but the structures are practically immune to decay. _(Note: Despite the name, this zone actually increases your protocol tax slightly while heavily buffing your fatigue rate)._

* **Yield Modifier:** +5% (`+500 BPS`)
* **Fatigue Modifier:** -10% (`-1000 BPS`)
* **Tax Modifier:** +10% (`+1000 BPS`)
{% endstep %}

{% step %}
### Tenant's Trap Canyon

An absolute concrete bunker. The yield is terrible, but the properties are indestructible and enjoy a small tax break.

* **Yield Modifier:** -10% (`-1000 BPS`)
* **Fatigue Modifier:** -20% (`-2000 BPS`)
* **Tax Modifier:** -5% (`-500 BPS`)
{% endstep %}

{% step %}
### Speculation Springs

The ultimate high-risk, high-reward zone. Massive gross yield generation, offset by vicious structural decay and brutal tax brackets.

* **Yield Modifier:** +25% (`+2500 BPS`)
* **Fatigue Modifier:** +15% (`+1500 BPS`)
* **Tax Modifier:** +20% (`+2000 BPS`)
{% endstep %}

{% step %}
### Repossession Ridge

The repo-man's stomping ground. A completely flat 10% penalty/buff applied evenly across your entire ledger.

* **Yield Modifier:** +10% (`+1000 BPS`)
* **Fatigue Modifier:** +10% (`+1000 BPS`)
* **Tax Modifier:** +10% (`+1000 BPS`)
{% endstep %}
{% endstepper %}
