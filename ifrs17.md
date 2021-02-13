# IFRS 17 <!-- omit in toc -->

- [Background](#background)
- [Level of aggregation](#level-of-aggregation)
- [General Measurement Model](#general-measurement-model)
  - [Discount rate](#discount-rate)
  - [Risk Adjustment](#risk-adjustment)
  - [Contractual service margin](#contractual-service-margin)
  - [Onerous contracts](#onerous-contracts)
  - [Reinsurance contracts](#reinsurance-contracts)
- [Premium Allocation Approach](#premium-allocation-approach)
- [Disclosure](#disclosure)

## Background

- International Financial Reporting Standards (`IFRS`) := accounting standards issued by the International Accounting Standards Board (`IASB`) and the IFRS Foundation
- Effective from 1 January 2023
  - Comparison needs to be given with equivalent figures for year ending 31 December 2022
- > IFRS 17 Insurance Contracts establishes principles for the recognition, measurement, presentation and disclosure of insurance contracts issued. It also requires similar principles to be applied to reinsurance contracts held and investment contracts with discretionary participation features issued. The objective is to ensure that entities provide relevant information in a way that faithfully represents those contracts. This information gives a basis for users of financial statements to assess the effect that contracts within the scope of IFRS 17 have on the financial position, financial performance and cashflows of an entity.
- Applies to (re)insurance contracts issued by entity and to reinsurance contracts entity holds
- Insurance contracts := _"contracts under which the entity accepts significant insurance risk from another party (the policyholder) by agreeing to compensate the policyholder if a specified uncertain future event (the insured event) adversely affects the policyholder"_

## Level of aggregation

- Requires level of aggregation := grouping of (re)insurance contracts into a single bucket (`portfolio`)
- Creates sets of portfolios that subsequently measured using prescribed measurement method
- `Portfolio` := aggregation of contracts subject to similar risks, managed together and have been issued not more than a year apart (covers one undewriting year)
- Insurer required to further separate contracts of each portfolio into three groupings, based on likelihood of contracts becoming loss-making (`onerous`):
  - Contracts that are onerous when measured at initial recognition
  - Contracts that are profitable at initial recognition and have no significant risk of becoming onerous
  - Contracts that could subsequently become onerous
- Initial recognition := point in time when contract first recognised as insurance obligation, earliest of:
  - beginning of coverage period
  - date when first payment from policyholder becomes due or has been recieved
  - time when insurer determined given group of contracts is onerous

## General Measurement Model

- Building Block Approach (`BBA`) - measures insurance contract by breaking it down into individual blocks:
  - Future cashflows that arise from provision of insurance contract
  - Discount rate to reflect the time-value of money
  - Risk Adjustment element for non-financial risks
  - Contractual service margin (`CSM`) representing unearned profit

**Estimate of future cashflows**

- Insurer identifies all cashflows that fall within boundary of contracts in a group
- Point at which contract boundary ends is:
  - Time when the entity can either change the price or level of benefits of the policy, **and**
  - Pricing of premiums for coverage up to the date when the risks are assessed does not take into account the risks that relate to periods after the reassessment date
  - Practical: relates to insurer's ability to re-price a contract
  - Some products: renewals guaranteed, policyholders do not have to go through assessment at renewal
  - Insurer could review prices based on all risks in portfolio considering all active risks until next renewal

### Discount rate

- All cashflows adjusted by discount rate that:
  - Reflects time value of money,
  - Reflects characteristics of the cashflows,
  - Reflects liquidity characteristics of the insurance contracts
  - Is consistent with observable market prices for financial instruments (consistent with those insurance contracts)
  - Excludes factors that influence market prices but not insurance contracts' cashflows (e.g. default risk)
- Two approaches allowed
- Bottom-up approach := Risk-free yield curve + illiquidty premium
  - Discount rate determined by adjusting reference risk-free yield curve to reflect differences in liquidity characteristics of financial instruments underlying the reference rate and those of insurance contract
  - Reference risk-free yield curve based on appropriate currency
  - Reference curve should have no / negligible credit risk
- Top-down approach := gross yield on reference portfolio - factors not relevant to liabilities
  - Discount rate derived from yield curve on reference portfolio assets and adjusted for characteristics that not relevant to insurance
  - Adjust out duration differences
  - Adjust out market premium for credit risk
  - Adjustment for differences between liquidity characteristics of reference portfolio and insurance contract **not** required
- Two approaches do not give same result
- Most insurers will find top-down approach difficult - hard to find suitable replicating portfolios

### Risk Adjustment

- Reflects compensation that insurer requires for bearing uncertainty about amount and timing of cashflows
- Relates to non-financial risks only
  - Insurance risk
  - Lapse risk
  - Expense risk
- Risk Adjustment indicates amount an entity would require to make it indifferent between
  - fulfilling fixed liability
  - fulfilling variable liability with same expected present value
- No prescribed methods for determining the Risk Adjustment
- Required to disclose percentiles

### Contractual service margin

- Contractual Service Margin (`CSM`) := unearned profit that relates to the period after the balance sheet date
- Positive CSM indicates expected profit
  - Earned over time as insurer fulfils its obligation
- Negative CSM indicates a loss
  - Recognised immediately in the P&L

### Onerous contracts

- Onerous contracts := contracts expected to be loss making at initial recognition
- Required to be grouped separately
- Expected loss recognised immediately in the P&L
- Contracts that were profitable at initial recognition could become onerous at subsequent measurement
  - Generally driven by changes in assumptions
  - Example: sudden adjustments in regulatory discount rates

### Reinsurance contracts

- Reinsurance contracts issued are treated similarly to insurance contracts
- Must be accounted separately from underlying insurance contracts

## Premium Allocation Approach

- Premium Allocation Approach (`PAA`) := simplified measurement model
- Only allowed to use it iff at initial recognition:
  - Reasonable expectation that the PAA would not produce measurement of liability materially different from the General Measurement model, **or**
  - Every contract in group of modelled contracts have coverage period of one year or less
- Most non-life insurance expected to be PAA allowable
- Materiality threshold not specified
- Liability for remaining coverage at initial recognition := premiums unearned net of insurance acquistion costs
- Under PAA there is no CSM

## Disclosure

- Covers additional information that insurers required to disclose in notes to financial statements
- Includes impact of contracts on entity's financial position, financal performance and cashflows
- Qualitative and quantitative information regarding:
  - amounts recognised in financial statements
  - significant judgements and changes in those judgements
  - nature and extent of risks within scope of contracts
- Disclose significant judgements (and changes) used to measure insurance contracts, including:
  - inputs
  - assumptions
  - estimation techniques
  - methods
  - inputs to those methods used for measurement of insurance contracts
- Specific disclosure on approach to determine the risk adjustment
  - Confidence levels represented by the risk adjustment
- Disclose information that allow users of financial statements to evaluate nature, amount, timing and uncertainty of future cashflows
