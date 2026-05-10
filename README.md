# audits
4EYES protocol audits.

## Projects
### Machina Finance
#### Grid Tading
- [Audit](./machina_finance/4eyes_audit_machina_finance_grid_trading.pdf)
- Comments:
    - This audit does not contain the T2T limit order contract since it was not fully implemented yet.
### Dexy Stablecoin
#### Dexy Gold
- [Audit](./dexy_stablecoin/4eyes_audit_dexy_gold.pdf)
- Comments:
    - An exploit was found that was missed in the initial audit.
    - The bug was found in the BuyBack contract.
    - The BuyBack contract, when exchanging the oracle fees for GORT, could send it to any address instead of the BuyBack output.
