---
sidebar_position: 7
---

Lending
=======

Coming soon!

Decentralized lending presents many opportunities as the next stage of DeFi evolution. Similar to decentralized exchanges, lending has two parties involved: the borrower and the supplier. Suppliers deposit assets into a pool to earn interest. Borrowers deposit assets for collateral, and borrows other assets. In order to borrow an asset, the borrower pays interest over time, paid to suppliers, with a share to the protocol.

This presents new opportunities for DeFi participants to further the growth of an ecosystem:

● Instead of staking tokens in liquidity mining programs, users can now lend out their tokens. This has the added advantage of earning yield on their tokens without impermanent loss and not having to hold two tokens at a fixed ratio as you must do when you liquidity mine.

● Users can deposit their tokens as collateral to borrow more tokens of another class. This presents the opportunity to trade on leverage.

The second point is crucial to our overall plan of turning Wisp Swap into a one-stop trading platform; lending and collateralization enables leveraged spot trading, and unlocks possibilities for derivatives.

However, these benefits are not risk-free. For borrowers, the main risk is liquidation and for suppliers, the main risk is not being able to withdraw your deposited tokens in a shortfall event.

**Lending**

Protocols such as Aave, Compound and Uniswap spurred the growth of DeFi with algorithmic, pool-based liquidity and lending strategies. Suppliers provide liquidity by depositing tokens into a pool contract. The pool of tokens can also be borrowed by placing tokens to the pool contract as collateral. Loans can instantly be issued without matching lenders to borrowers, instead relying on pooled tokens and state of the pool to calculate interest rates.

**Leveraged Trading**

Crypto exchanges such as Binance and FTX offer leveraged trading via margin or derivative trading. In this paper, we will focus on the leveraged spot trading use case. Leveraged spot trades can be decomposed to asset collateralization, borrowing, and then a trade.

For example:

● Margin long trades can be made by using tokens as collateral, and borrowing USDT for the long trade.

● Margin short trades can be made by using tokens or USD as collateral, and borrowing tokens for the short trade.

Exchanges such as FTX also allow users to participate in lending, by offering a two-sided market for lending and borrowing interest rates. We observe that leverage trading is a major use case for crypto token borrowing, and that similar synergy can also provide value for decentralized exchanges.

**Decentralized leveraged trading**

**_Sushiswap_**

Sushiswap is an Automated Market Maker (AMM) that also offers integrated lending, via their Kashi feature. Leveraged trades can be performed by providing collateral to and borrowing from Kashi, and then swapping tokens on the AMM. A key distinction of Kashi is its isolated lending pools.

Rather than borrowing tokens from a shared pool such as in Aave, Kashi loans are made from individual token pairs. For example, to borrow USDT against ETH collateral, the borrower would have to post ETH tokens against the specific ETH/USDT pool. The interest rate and loan risks are specific only to the ETH/USDT pool. Although Kashi is less prone to loan risk, it is less convenient for traders as there is added friction in comparing interest rates between different pairs.

Example:

● Assuming 1 ETH = $3000 and collateral factor is 65%.

● Deposit and collateralize 1 ETH to ETH/USDT pool.

● Borrow 1500 USDT from the ETH/USDT pool against the collateralized ETH.

● Swap 1500 USDT for 0.5 ETH

● User has used 1 ETH and swapped his borrowed amount for 0.5 ETH. So he is now 0.5x leveraged long on ETH.

**_WOWswap_**

WOWswap is a decentralized leveraged trading protocol that allows users to borrow tokens for leverage trades. The protocol itself facilitates token lending and borrowing, and then performs trades on behalf of users on integrated AMMs such Pancakeswap. In this design, the swapped tokens are held by the protocol as collateral against borrowed assets. This strategy may appear to be more convenient to the trader, as no additional collateral is provided before performing the trade. However, the custodial design with the trader receiving a proxy-token is effectively a derivative contract, with traders and lenders sharing exposure to the swapped asset.

Example:

● Send 1 BNB to contract and borrow 4 BNB.

● Contract swaps 5 BNB for 100 CAKE.

● Contract mints 300 proxy-CAKE tokens to the trader.

**Design**

Since its inception in 2020, many lending protocol variants have emerged. They can be largely classified into two categories:

● Isolated lending pool (Sushiswap Kashi, Impermax): Similar to a Uniswap v2 liquidity pair, an isolated lending pool only allows borrowing and lending between two assets, for example, AVAX-USDT. Furthermore, each pair requires two separate markets, each denoting which asset is the collateral asset and which is the borrowable asset. This has the added benefit of limiting risk to a certain pair, but at the cost of fragmenting liquidity significantly.

● Grouped lending pool (Compound, CREAM, Aave): All assets are grouped into a single pool, which means liquidity is not fragmented. However, the disadvantage is that if a risky asset is added then that could jeopardize the entire pool. As a result, protocols using this approach usually have a strict criteria for listing new assets.

We believe that a grouped lending pool provides several advantages for the purposes of offering leveraged trading. For example, if a trader wants to borrow tokens, a grouped lending pool offers more concentrated liquidity without needing to compare interest rates, compared to isolated lending pools. In order to offer leveraged trading for as many tokens as possible, we also considered an approach that can reasonably scale for long-tail assets.