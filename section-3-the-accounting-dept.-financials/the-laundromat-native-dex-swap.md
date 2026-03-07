# 💱 The Laundromat: Native DEX Swap

**"We don't call it money laundering, Junior. We call it 'Bidirectional Capital Flow Optimization'."**

Welcome to the trading floor. You don't need to leave the terminal to liquidate your extracted yield or acquire fresh capital. Slumlords OS features an integrated native swap module (`LIQUIDITY_ROUTER`). This interface connects directly to the underlying Monad decentralized exchange router, allowing you to execute permissionless, high-frequency trades between `$RENT` and **WMON** directly from your command center.

Why use a third-party UI when you can dump on the market directly from the corporate intranet?

***

## 🔮 Market Oracle.SYS (Live Pricing & Surveillance)

At BlackCoq, we don't rely on delayed, third-party APIs like CoinGecko to tell us what our money is worth. We look straight into the ledger's soul.

* **The Factory Ping:** The `MARKET_ORACLE` module pings the decentralized exchange's factory contract directly. It reads the live `reserve0` and `reserve1` ratios of the `$RENT/WMON` liquidity pool to calculate the exact execution price before you trade.
* **Auto-Sync:** The terminal continuously re-fetches the on-chain ratio every 15 seconds. In a high-velocity ecosystem like Monad, price action moves at the speed of light. We ensure you are viewing the most accurate execution price down to the millisecond.
* **Fiat Estimation:** The Oracle cross-references the live on-chain ratio with a secondary external API to provide a real-time estimated USD equivalent for your `$RENT`. It's always nice to know exactly how many fiat dollars you just extracted from the working class today.

***

## ⚖️ Two-Way DEX Execution (The Flow)

The router allows for seamless bidirectional capital flow.

* **Acquiring $RENT (The Buy-In):** Swap your **WMON** for `$RENT` to secure the operational capital required for public mints, purchasing Upgrades from the catalog, or bribing the protocol via Skill Points.
* **Liquidating Yield (The Golden Parachute):** Instantly dump your harvested `$RENT` back into the liquidity pool in exchange for **WMON**. When it's time to cash out, you hit the red button and let the automated market makers absorb the impact.

***

## 📝 Authorization Protocol (Signing the Papers)

Because the OS interacts directly with a decentralized router, you must explicitly grant the smart contract permission to handle your funds before a swap can be executed.

{% stepper %}
{% step %}
### Corporate Authorization

Depending on the direction of your trade, the OS will prompt you to approve either the `$RENT` contract or the **WMON** wrapper contract. This is a standard ERC-20 security authorization. You are giving the BlackCoq router permission to move your money.
{% endstep %}

{% step %}
### Execution & Slippage

Once authorized, the terminal calculates the optimal mathematical path for your trade. The OS automatically pads your exact input calculations with a 0.5% slippage buffer. Why? Because the Monad dark forest is full of rival MEV bots waiting to front-run your transactions. The buffer ensures your trade executes successfully even if the pool drifts slightly during the sub-second block time.
{% endstep %}
{% endstepper %}
