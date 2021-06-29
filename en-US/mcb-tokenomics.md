# MCB Tokenomics

Upon June 1th, 2021, 2,193,177 MCB has been issued, among which:

- 1 million MCB belongs to the team, advisors and investors:
  - Dev Team: 484K
  - Advisors: 75K
  - Angel investor: 109K
  - Private token sale: 332K, Price 2.5USD/MCB
- 1,174,036 MCB belongs to Liquidity providers
- 19,141 MCB belongs to community contributors

According to the approved [Proposal 19](https://forum.mcdex.io/t/proposal-19-mcb-new-tokenomics/262), the new Tokenomics states:

1. The total supply of MCB is 10,000,000;
2. MCDEX DAO is responsible for the specific usage of the newly issued MCB;
3. The speed of issuance will be under following restrictions:
   - It is plausible to issue 1 MCB for 1 USD captured by the MCDEX DAO vault
   - At least 0.2 MCB can be issued by one Ethereum block (approximately 1300MCB/day)
4. For every new issuance, 75% is for community incentive, and 25% belongs to the developers.


## Series A Fundrasing
Based on the approved [Proposal 20](https://forum.mcdex.io/t/proposal-20-raise-7m-fund-for-mcdex-dao/298), MCDEX DAO raised $7M from both institutin investors and community to bootstrap the liquidity when V3 launch. 

Total 700K MCB will distributed to the investors of this round. The MCB is from the community incentive part.

The vesting schedule is as below:

Since the MCB’s new tokenomics is performance-based, tokens for this round are restricted by this model. Details are :
```
R = MIN(MAX((V - 0.2) * 0.75, 0),  0.64614))
R: MCB Vested to investors per Ethereum Block
V: Value Captured in the block
```
Since the major source of the DAO value capture is the 0.015% vault fee, the formula can be written as: 
```
Daily Vested MCB  = MIN(MAX((Daily Volume * 0.015% - 1300) * 0.75, 0), 4200)
```
Daily Vesting Examples:

| Daily Trading Volume | Daily MCB may be issued|MCB for investors|
|------------------------------|-----------------------------------|------------------------|
| <= $8.7M | 1300 | 0 | 
|$10M | 1500|150|
|$40M|6000|3525|
|>= $46M|6900|4200|

When the trading volume is lower than $8.7M/day, investors cannet get any MCB. When the trading volume grows more than $8.7M, investors will start to collect according to the above rule. When the trading volume is above $46M/day, the investors will enjoy the maximum speed of vesting. The shortest time for investors to collect all tokens is 6 months.

This model closely binds investors’ benefits to MCDEX performance hence encouraging all investors to make continuous efforts to help MCDEX to achieve its long-term value.
