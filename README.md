# audits
4EYES protocol audits.

## Projects
### Lithos
#### Mining
- Part 3
    - [Audit](./lithos/4eyes_audit_lithos_mining_part3.pdf)
    - Comments
        - This part covers the revised collateral and rollup contracts.
- Part 2
    - [Audit](./lithos/4eyes_audit_lithos_mining_part2.pdf)
    - Comments
        - This part covers the rollups and LithosDex contracts. 
- Part 1
    - [Audit](./lithos/4eyes_audit_lithos_mining_part1.pdf)
    - Comments
        - This part covers the LIT emissions and collateral contracts.
### Machina Finance
#### Grid Trading
- [Audit](./machina_finance/4eyes_audit_machina_finance_grid_trading.pdf)
- Comments
    - This audit does not contain the T2T limit order contract since it was not fully implemented yet.
### Dexy Stablecoin
#### Dexy Gold
- [Audit](./dexy_stablecoin/4eyes_audit_dexy_gold.pdf)
- Comments
    - Exploits found that were missed in the initial audit:
        - BuyBack: When exchanging the oracle fees for GORT, could send it to any address instead of the BuyBack output.
        - LP: The LP box does not check that it is itself the box at INPUTS(0), but the Swap contract assumes it is. This caused a loss of funds in both the DexyGold and DexyUSD (USE) protocols totalling ~70k USD. Further explanation with on-chain analysis can be found [here](https://ergoforum.org/t/use-dexygold-lp-hack-postmortem/5362).
