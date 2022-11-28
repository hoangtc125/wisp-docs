---
sidebar_position: 1
---

WispSwap Protocol
=================

The design of a decentralized AMM was first proposed by Vitalik Buterin in 2016-2017 and later implemented by Uniswap and Bancor. Unlike centralized crypto exchanges with their order books, AMMs allows users to create liquidity pools with tokens of X and Y, where the initial ratio of the two tokens determines their starting relative price and the so-called liquidity curve (the change in price that results from each swap transaction).

Users can swap tokens by providing one side asset in exchange for another and paying a small fee. By contrast, liquidity providers provide both X and Y tokens and earn a share of the transaction fees. When depositing tokens X and Y in a pool, a liquidity provider receives special LP tokens in exchange, which represent their share in the pool and are needed to withdraw the deposited liquidity.

Most AMMs utilize a so-called **Constant Function** - a formula for calculating two tokens' relative prices that ensures that a pool will not be drained as a result of any liquidity event. The standard liquidity curve function, introduced by Uniswap v2, looks as follows:

x \* y = k

In the formula, X and Y are the amounts of the two tokens in a pool, and their product k is a constant. Any trade (swap) changes the amounts X and Y, but k remains the same. This formula is suitable for uncorrelated swaps (assets whose prices aren't correlated with each other) and works well in most cases, including on WispSwap.

_For swaps between stablecoins and other correlated assets, however, the simple constant product formula is not very effective. In such cases, WispSwap uses a different, more complex formula to minimize slippage even for large transactions._
