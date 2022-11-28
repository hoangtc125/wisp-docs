---
sidebar_position: 3
---

Emergency brake
===============

As the Sui blockchain, the Move language, and Move VM are all very new technologies, it will take time for them to be fully verified and tested. For this reason, we have implemented an emergency brake to stop all liquidity minting and swaps, while simultaneously allowing liquidity providers to burn their LP tokens.

We hope that we will never have to activate the emergency brake, as we have also performed several security audits. Yet, we still want to keep the 'emergency button' in case of an unlikely event of a protocol-level or virtual machine-level issue.

The emergency feature is currently managed by the Wispswap team multisignature and can later be transferred to a DAO.

Once we have verified that the protocol is stable and secure enough, we may disable the emergency brake indefinitely.