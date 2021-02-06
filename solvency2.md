# Solvency II <!-- omit in toc -->

- [Pillar 1 - Quantitative requirements](#pillar-1---quantitative-requirements)
  - [Valuation of assets](#valuation-of-assets)
  - [Eligible capital](#eligible-capital)
  - [Technical provisions](#technical-provisions)
  - [Technical provisions - best estimate](#technical-provisions---best-estimate)
  - [Technical provisions - risk margin](#technical-provisions---risk-margin)
  - [Premium provision](#premium-provision)
  - [Contract boundaries](#contract-boundaries)
  - [Legal obligations basis for unincepted contracts](#legal-obligations-basis-for-unincepted-contracts)
  - [Data quality](#data-quality)
- [Pillar 1 - Capital requirements](#pillar-1---capital-requirements)
  - [Minimum Capital Requirement (`MCR`)](#minimum-capital-requirement-mcr)
  - [Solvency Capital Requirement (`SCR`)](#solvency-capital-requirement-scr)
  - [Standard Formula Solvency Capital Requirement (`SF SCR`)](#standard-formula-solvency-capital-requirement-sf-scr)
  - [Internal Model Solvency Capital Requirement (`IM SCR`)](#internal-model-solvency-capital-requirement-im-scr)
- [Pillar 2 - Qualitative requirements](#pillar-2---qualitative-requirements)
  - [Corporate governance](#corporate-governance)
  - [Risk management function](#risk-management-function)
  - [Internal control](#internal-control)
  - [Actuarial function](#actuarial-function)
  - [ORSA](#orsa)
- [Pillar 3 - Reporting requirements](#pillar-3---reporting-requirements)

## Pillar 1 - Quantitative requirements

- Risk-based capital requirements, firms to meet with assets and liabilities valued on a market consistent basis.
- Two capital requirements defining upper and lower end of a ladder of supervisory intervention
- Solvency Capital Requirement (`SCR`) := level above which no supervisory intervention for financial reasons
  - SCR calculated using standard formula or (with prior supervisory approval) insurer’s internal model or combination
- Minimum Capital Requirement (`MCR`) := level below which supervisor’s strongest actions are taken (e.g. removal of the insurer’s authorisation)
  - MCR calculated using a linear formula
  - Falls between 25% and 45% of the SCR
  - Capital add-ons may be exceptionally imposed by the supervisor where it believes risk profile of insurer significantly deviates from underlying SCR assumptions
    - Supervisor-imposed add-ons increase the SCR

### Valuation of assets

- Assets valued at amount which could be exchanged between knowledgable willing parties in arm's length transaction
- Default valuation approach: quoted market prices
  - Where quoted market prices unavailable: mark to model valuation used
- Recoveries expected from RI shown as asset
  - Adjusted to allow for best estimate of expected losses due to RIer default
  - Expected loss due to default := `LGD * PD`

### Eligible capital

- **Basic own funds** := assets - liabilites
  - ~= capital that already exists within insurer
  - Example: paid up share capital from ordinary and preferences shares (members' contributions in mutual)
- **Own funds** := assets - liabilites + ancillary own funds
- Ancillary own funds := capital that may be called upon in certain adverse circumstances, does not currently exist within insurer
  - Examples: unpaid share capital, LOCs, guarantees, calls on members of mutual to contribute capital
- Capital is tiered based on loss absorbency and permanency
  - Tier 1 := most loss absorbent and permanent form
  - Tier 3 := least (example: subordinated debt)
- Subordination criteria := must rank after claims of all PHers, beneficiaries and non-subordinated creditors
- No encumbrances criteria := unconnected with other transactions and no restrictions, charges or guarantees
- No mandatory fixed charges criteria:
  - Tier 1 / 2 := Suspension of redemption provided, coupons/dividends can be cancelled in case of breach of _SCR_
  - Tier 3 := Suspension of redemption provided in case of breach of SCR, deferral of coupons/dividends on breach of _MCR_

| Criteria                       | Tier 1                                                                                                                           | Tier 2                                                                                                                                                       | Tier 3                                                                                                                     |
| ------------------------------ | -------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------ | -------------------------------------------------------------------------------------------------------------------------- |
| Loss absorbency                | Immediately available to absorb losses<br>Absorbs losses at least on SCR breaches<br>Should not cause or accelerate insolvency   | Not necessarily immediately available to absorb losses<br>Should not cause or accelerate insolvency                                                          | Should not cause or accelerate insolvency                                                                                  |
| Sufficient duration            | Undated or of the same duration as the undertaking<br>Contractually locked in or replaced at least equivalently on breach of SCR | Undated or minimum 10 years maturity at issue<br>Contractually locked in or replaced at least equivalently on breach of SCR                                  | Undated or minimum 5 years maturity at issue<br>Contractually locked in or replaced at least equivalently on breach of SCR |
| Free from incentives to redeem | Only redeemable at the option of the insurer or reinsurance undertaking                                                          | Only redeemable at the option of the insurer or reinsurance undertaking<br>Limited incentives to redeem are permissible after 10 years from date of issuance | Only redeemable at the option of the insurer or reinsurance undertaking<br>Limited incentives to redeem are permissible    |

- Restrictions placed on quality of capital usable to cover MCR and SCR:
  - 80% of MCR must be covered by Tier 1 capital
  - Tier 3 capital cannot be used to cover MCR
  - 50% of SCR must be covered by Tier 1 capital
  - No more than 15% of SCR may be covered by Tier 3 capital
  - Some Tier 1 capital items restricted to < 20% of total Tier 1 capital covering MCR or SCR (e.g. preference shares)

### Technical provisions

- **Technical Provisions** (`TPs`) := amount insurance company would have to pay to transfer its obligations immediately to another company
- Comprises:
  - **Premium provisions** := future claim events covered by contracts that are required to be included in TPs
  - **Claims provisions** := claim events that have already occurred whether reported or not
- TPs = Best Estimate + Risk Margin

### Technical provisions - best estimate

- **Best estimate** := probability-weighted average future cashflows, discount to allow for time value of money
- All assumptions should be best estimate assumptions, no margins
- Take account of all relevant available data, internal and external when deriving assumptions that best reflect characteristics of underlying portfolio
- Risk-free interest rates used for each currency and maturity to discount future cashflows derived from interest rate swap rates, adjusted for credit risk
- Split and calculated separately: premium provision and claims provision

### Technical provisions - risk margin

- **Risk margin** (== Market Value Margin, `MVM`) := ensure value of the TPs is equivalent to amount that (re)insurance undertaking would be expected to require to take over and meet (re)insurance obligations
- Calculated by estimating cost of capital equal to SCR necessary to support the (re)insurance obligations over their lifetime in respect of risks which cannot be hedged:
  - Underwriting risk
  - RI credit risk
  - Operational risk
  - Unavoidable market risk
- Calculated using following steps:
  - Estimate future development of SCRs into future
  - Multiply future development of SCRs by cost of capital (`CoC`) (standard is 6% p.a.)
  - Discount resulting costs of capital using relevant risk-free interest rate term structures from EIOPA
- Note discounting must be performed back to `t = 0`, i.e. include SCR at `t = 0` multiplied by CoC (6%)
- Complex methodology => involve complex series of nested stochastic loops
  - Hierarchy of simplifications available for companies to use where appropriate
- Risk margin disclosed separately for each LOB
- Risk margin can be reduced to take into account diversification between LOBs up to legal entity level
  - Allocation of diversification benefit approximated by apportioning total diversified risk margin across LOBs in proportion to the SCR calculated on standalone LOB basis (or other methods if appropriate <= materiality)

### Premium provision

- **Best estimate** := best estimate of future cashflows in respect of unexpired exposures (not unearned proportion of written premiums)
- No credit taken for deferred acquistion costs
- No allowance made for claims equalisation provisions

### Contract boundaries

- TP assumption needed, boundary is set at point at which company:
  - Can unilaterally terminate the contract or refuse to accept premium
  - Or amend benefits / premiums in such a way that premiums fully reflect risks
- Boundary sets point at which premiums can be recognised on existing contracts
  - Within boundary, both contractual recurring premiums and premiums arising from PHer options to renew/extend policies considered on best estimate basis
  - Allowance for remaining years on contract for expected premiums and claims => TPs can increase/decrease depends on whether contract expected to be profitable

### Legal obligations basis for unincepted contracts

- TP assumption needed, contracts not yet incepted but corresponding liabilities cannot be waived or reduced by company as at valuation date
- Legal obligations basis material where business is written by:
  - Delegated undewriting authorities (e.g. binders)
  - Brokers <= backlog of aggregated pipeline premiums
  - Year-end renewals <= RIers entering 1/1 renewals prior to 31 December valuation date
  - Tacit renewal agreements := business automatically renewed unless PHer decideds to move cover to another provider

### Data quality

- Data quality requirements for calc of TPs, deemed crucial:
  - More complete and correct data => more consistent and accurate final estimate
  - Application of wider range of methodologies for calculating best estimate made possible, improving chances of application of adequate & robust methods for each case
  - Validation of methods more reliable => more credible conclusions
  - Effective comparisons over time and in relation to market data possible => better knowledge of businesses in undertaking operates and its performance
- Data quality relevant to solvency assessment: SCR
- Consistent approach to data quality across Pillar 1 needed without disregarding different objectives

## Pillar 1 - Capital requirements

### Minimum Capital Requirement (`MCR`)

- MCR calculated for each individual LOB, take sum of:
  - Factor applied to TPs (not including risk margin) for each LOB, net of RI, subject to min of 0
  - Factor applied to written premiums in each LOB over last 12 month period, net of RI, subject to min of 0
- MCR calibrated to VaR of basic own funds of (re)insurer subject to confidence level of ~85% over one-year time horizon
- MCR factors as in Delegated Regulation for each LOB in following table
  - Apply to direct, facultative RI and proportional RI
  - Non-proportional (`NPL`) RI separate LOBs

| Line of business                  | MCR % factor: premium risk | MCR % factor: reserve risk |
| --------------------------------- | -------------------------: | -------------------------: |
| Motor vehicle liability           |                        9.4 |                        8.5 |
| Other motor                       |                        7.5 |                        7.5 |
| Marine, aviation and transport    |                       14.0 |                       10.3 |
| Fire and other damage             |                        7.5 |                        9.4 |
| General liability                 |                       13.1 |                       10.3 |
| Credit and suretyship             |                       11.3 |                       17.7 |
| Legal expenses                    |                        6.6 |                       11.3 |
| Assistance                        |                        8.5 |                       18.6 |
| Miscellaneous financial loss      |                       12.2 |                       18.6 |
| NPL property                      |                       15.9 |                       18.6 |
| NPL casualty                      |                       15.9 |                       18.6 |
| NPL marine, aviation and casualty |                       15.9 |                       18.6 |

- Resulting MCRs summed across LOBs to obtain overall MCR
- MCR must lie \[25%, 45%\] of SCR

### Solvency Capital Requirement (`SCR`)

- SCR calibrated to VaR of basic own funds of (re)insurer subject to confidence level of ~99.5% over one-year time horizon
- SCR must cover at least following risks:
  - Non-life underwriting risk
  - Life underwriting risk
  - Health underwriting risk
  - Market risk
  - Credit risk
  - Operational risk - excluding risks from strategic decisions and reputation risks
- Range of methods to calculate SCR
  - Proportionate to nature, scale, complexity of risks undertaken
  - Standard formula
  - Standard formula with simplifications
  - Standard formula with undertaking-specific parameters (`USPs`)
    - Non-life UWing risk factors (prior supervisory approval) replaced with USPs based on undertaking's own claims experience
  - Partial internal model (prior supervisory approval via IMAP) in combination with standard formula for some risk factors
  - Full internal model (prior supervisory approval via IMAP)

### Standard Formula Solvency Capital Requirement (`SF SCR`)

- Calculated by combining number of separate capital requirements for each risk
- Allowing for diversification credits
  - via correlation matrices
  - or other methodologies
- Capital requirements for each individual risk determined as difference between:
  - Net asset value (assets - best estimate liabilities) in unstressed balance sheet
  - Net asset value in stressed balance sheet
- Individual capital requirements combined across risks within module using specified correlation matrix
- SF SCR comprises:
  - Operational risk (`SCR{op}`)
  - Adjustment, includes loss absorbing capacity of deferred taxes (could comprise reduction in any base balance sheet deferred tax liability, no longer fully payable in stressed scenario)
  - Market risk:
    - Interest rate risk
    - Equity risk
    - Property risk
    - Spread risk
    - Currency risk
    - Concentration risk
  - Non-life underwriting risk:
    - Premium and reserve risk
    - Catastrophe risk
    - Lapse risk
  - Life underwriting risk:
    - Mortality risk
    - Longevity risk
    - Disability/morbidity risk
    - Expenses risk
    - Revision risk
    - Catastrophe risk
    - Lapse risk
  - Health risk:
    - Similiar to life techniques (`SLT`) health risk
    - Non-SLT health risk
    - Catastrophe risk
  - Counterparty default risk
  - Intangible asset risk (`SCR{int}`)
- SCR = BSCR + Adj + SCR\{op\}, where:
  - **BSCR** := Basic SCR = `Sqrt(∑ Corr{i,j} x SCR{i} x SCR{j}) + SCR{int}`
  - Correlation coefficiences (`Corr{i,j}`) as per below matrix

|          | Market | Default | Life | Health | Non-Life |
| -------- | -----: | ------: | ---: | -----: | -------: |
| Market   |      1 |         |      |        |          |
| Default  |   0.25 |       1 |      |        |          |
| Life     |   0.25 |    0.25 |    1 |        |          |
| Health   |   0.25 |    0.25 | 0.25 |      1 |          |
| Non-life |   0.25 |     0.5 |    0 |      0 |        1 |

**Operational risk**

- Risk of losses occurring due to inadequate or failed internal processes, people and systems or due to external events
- Capital requirement = subject to max of 30% of BSCR, Greater of:
  - 3% of gross earned premiums during previous 12 months
  - 3% of gross TPs
- Assumption: no diversification credit between operational risk and other components of risk

**Non-life underwriting risk**

- Standard deviations used to calculate premium and reserve risk factors
- SF calculates 99.5% VaR factors = standard devs \* 3

| Line of business                  | Std Dev %: premium risk | Std Dev %: reserve risk |
| --------------------------------- | ----------------------: | ----------------------: |
| Motor vehicle liability           |                    10.0 |                     9.0 |
| Other motor                       |                     8.0 |                     8.0 |
| Marine, aviation and transport    |                    15.0 |                    11.0 |
| Fire and other damage             |                     8.0 |                    10.0 |
| General liability                 |                    14.0 |                    11.0 |
| Credit and suretyship             |                    19.0 |                    17.2 |
| Legal expenses                    |                     8.3 |                     5.5 |
| Assistance                        |                     6.4 |                    22.0 |
| Miscellaneous financial loss      |                    13.0 |                    20.0 |
| NPL property                      |                    17.0 |                    20.0 |
| NPL casualty                      |                    17.0 |                    20.0 |
| NPL marine, aviation and casualty |                    17.0 |                    20.0 |

- 99.5% VaR factors in respect of **premium risk** applied to max of:
  - Estimate of net earned premium for each LOB during forthcoming year
  - Net earned premiums for each LOB during previous year
- Premium risk factors derived from claims development data gross of RI
- Undertakings permitted to multiply premium risk factors for each LOB - intended to represent XoL RI in place for each LOB:
  - 80% for motor vehicle liability, fire and other damage, general liability
  - 100% for all other LOBs
- 99.5% VaR factors in respect of **reserve risk** applied to best estimate for claims outstanding for each LOB
  - After deducting amount recoverable from RI and special purpose vehicles
- Scope using specified formula for premium & reserve risk factors to be reduced by up to 25% for geographical diversification
- Allowance also made for:
  - Correlation coefficient of 0.5 between premium risk and reserve risk factors
  - Diversification by LOB

**Non-life catastrophe risk**

- Determined by complex series of formulae, comprises:
  - Natural catastrophe risk sub-module
    - Sub-divided between windstorm, earthquake, flood, hail and subsidience risk
  - Sub-module for catastrophe risk of non-proportional property RI
  - Sub-module for man-made catastrophe risk
    - Sub-divided between motor vehicle liability, fire, marine, aviation, liability and credit & suretyship
  - Sub-module for other non-life catastrophe risk

**Market risk**

**Counterparty default risk**

### Internal Model Solvency Capital Requirement (`IM SCR`)

**Use test**

**Statistical quality standards**

**Calibration standards**

**Profit and loss attribution**

**Validation standards**

**Documentation standards**

**Practical considerations**

## Pillar 2 - Qualitative requirements

- Focuses on governance, risk management and required functions (internal audit and actuarial)
- Includes supervisory review process
- Insurers required to carry out an Own Risk and Solvency Assessment (`ORSA`)
  - To be reviewed by the supervisor
- Includes ‘prudent persons’ investment principles
- Supervisors can impose capital additions for governance failings

### Corporate governance

### Risk management function

### Internal control

### Actuarial function

### ORSA

## Pillar 3 - Reporting requirements

- Comprises reporting and disclosure requirements
- Public Solvency and Financial Condition Report (`SFCR`)
- Reporting to the supervisory authority of a Regular Supervisory Report (`RSR`)
- Quantitative templates
- The aim of public disclosures is to harness market discipline by requiring firms to publish certain details of their risks, capital and risk management
