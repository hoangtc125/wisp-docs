---
sidebar_position: 2
---

Pool Types
==========

WispSwap can currently construct 3 types of pools for liquidity providers and swappers:

**1\. General liquidity Pool**

WispSwap implements the`Uniswap-V2` constant product algorithm `XY=K` for creating a pool for general token swapping. Aptoswap users could use those pools for uncorrelated token swapping such SUI/USDC, SUI/USDT.

**2\. Stable Swap Pool**

WispSwap implements the`Curve` stable swap algorithm that is used for pegged assets swapping to centralize the liquidity to the pegged price. Users could use those pools for stable coin or pegged assets swapping.

**3\. Whirpool**

WispSwap implements the `Uniswap-V3` algorithm that allows liquidity providers to provide liquidity within a user-specified custom price range to centralize their liquidity and boost their rewards.