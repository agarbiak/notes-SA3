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
  - [Own Risk and Solvency Assessment (`ORSA`)](#own-risk-and-solvency-assessment-orsa)
- [Pillar 3 - Reporting requirements](#pillar-3---reporting-requirements)
- [Application to insurance groups](#application-to-insurance-groups)

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

- Equity risk capital requirement
  - 39% market value of Type 1 equities
    - Listed in regulated markets (members of EEA / OECD)
    - Shares of alternative investment funds authorised as European Long-term Investment Fund
  - 49% market value of Type 2 equities
  - Symmetric adjustment (additive) => avoids pro-cyclical effects
    - Equity stress smaller following decline in equity markets
    - Equity stress higher following strong performance of equity markets
    - 31 December 2018: -6.34% symmetric adjustment
    - 31 December 2020: -0.48% symmetric adjustment
  - 22% market value for strategic nature equity investments in related undertakings
- Interest rate risk capital requirement determined by stressing yield curve by specified percentages, varying by term to maturity
  - Affects value of certain classes of assets (e.g. fixed coupon bonds)
  - Affects value of liabilites (discounted to allow for time value of money)
- Property risk capital requirement
  - 25% market value of properties
- Currency risk capital requirement
  - 25% change in currency exchange rates w.r.t. net currency exposures
- Spread risk capital requirement - based on formula
  - Corporate bonds - loss on assets := f(duration of assets, credit rating of underlying bonds)
  - Lower requirements for public sector and mortgage-covered bonds
- Concentration risk capital requirement - applies to holdings > specified threshold
  - Based on exposure, rating and total assets held

**Counterparty default risk**

- Counterparty default risk capital requirement split:
  - Type 1 exposures := small number of counterparties (usually rated)
    - Based on loss distribution derived from LGDs and default probabilities
    - Example: RIers, derivative counterparties
  - Type 2 exposures := diversified mix of unrated counterparties
    - Based on immediate shock
    - Assume loss of 90% of receivables which have been due > 3 months
    - Assume loss of 15% on other receivables

### Internal Model Solvency Capital Requirement (`IM SCR`)

- Partial or full internal model
  - Must obtain prior supervisory approval
- Appropriate if risk profile of business differs materially from underlying in SF
- Appropriate if company already uses model for risk management / other decision-making purposes (pricing, investment strategy)
- Supervisor can require company to develop internal model if it considers SF inappropriate to risk profile of company
- Some circumstance, internal model potentially lead to less onerous overall capital requirements than if SF used
- Internal model must generate SCR based on stated requirements
  - Coverage of risk types
  - Provide protection of least 99.5% confidence level over 1 year time horizon
- IM must pass tests for supervisory approval:
  - Use test
  - Statistical quality standards
  - Calibration standards
  - Profit and loss attribution
  - Validation standards
  - Documentation standards

**Use test**

- (Re)insurer need to demonstrate IM widely used throughout all relevant areas of business
- IM needs to play significant role in:
  - internal goverance,
  - risk management,
  - decision-making processes,
  - economic and solvency capital assessments
  - capital allocation processes

**Statistical quality standards**

- IM complies with:
  - Methods used to calculate probability distribution forecast based on adequate, applicable, relevant actuarial & statistical techniques
  - Methods used to calculate probability distribution forecast based on current & credible information and realistic assumptions
  - Datasets used in the calculation of the probability distribution forecast updated at least annually
  - Data used for IM is accurate, complete and appropriate
  - Assumptions justified to the supervisory authorities
  - Cover all of the material risks to which (re)insurer exposed
  - Particular risks associated with financial guarantees and any contractual options must be accurately assessed where material
  - Risks associated with both PHer options and contractual options must be assessed including the impact that future changes in financial and non-financial conditions may have on the exercising of those options
  - All expected payments to PHers whether or not payments are contractually guaranteed must be allowed for
  - - May take account of dependencies within/across risk categories provided system used for measuring diversification effects is adequate
  - May take account of effect of risk-mitigation techniques, as long as credit risk and other risks arising from the use of risk-mitigation techniques are reflected
  - May take account of future management actions that would reasonably be expected in specific circumstances

**Calibration standards**

- Demonstrate output from IM calculates SCR which provides PHers with level of protection equivalent to VaR of basic own funds subjec to confidence level of 99.5% over 1 year time horizon
- Different time period / risk measure can be used for internal purposes
- May require IM run on relevant benchmark portfolios, external assumptions to verify calibration of IM
  - Check specification in line with accepted market practice

**Profit and loss attribution**

- Annual review required: causes and source of P&L for each major BU
- Requirement to demonstrate how categorisation of risk chosen in IM used to explain causes and source of actual P&Ls
- Categorisation of risk and attribution of P&Ls must reflect risk profile

**Validation standards**

- Required: regular cycle of model validation
  - Monitoring of performance of IM
  - Review ongoing appropriateness of specification
  - Testing results against experience
- Validation process includes:
  - Effective statistical process for validating IM enabling demonstration to supervisor resulting capital requirements are appropriate
  - Analysis of stability of IM => sensitivity of results of IM to changes in key assumptions
  - Assessment of accuracy, completeness, appropriateness of the probability distribution forecast
    - Compared to loss experience
    - Compared to all relevant significant new data and info

**Documentation standards**

- Required: document design and operational details of IM
- Demonstrates compliance with requirements
- Detailed outline of theory, assumptions, mathematical and empirical bases underlying IM
- Circumstance under which IM does not work effectively
- Major changes to IM

**Practical considerations**

- **Use test** = most challenging aspect of gaining IM approval
  - Embed model throughout company
  - Develop effective risk culture
  - Evidence this is the case
- Quality of data / assumptions
  - Historical data available to calibrate extreme events limited
  - Practice: industry consensus emerge over core stresses (e.g. 99.5th percentile equity fall based on benchmark index)
  - Companies adapt such standards to allow own specific features (e.g. extent actual equity holdings more/less volatile than underlying benchmark)
  - Setting correlation factos under extreme conditions = challenging
- IM structured any way provided tests met
  - Does not have to follow SF structure
  - Example: stochastic sims rather than stress tests + correlation matrices
    - Calibration of stochastic models requires care and expertise
- 6 month deadline: supervisory authority receives application for IM to approval decision
  - Challenging for resources of regulatory bodies
  - Regulators set up **pre-application** informal approach
    - Encourage companies engage early on in model development and refinement processes
    - PRA has [PAQC process](https://www.bankofengland.co.uk/-/media/boe/files/prudential-regulation/supervisory-statement/2018/ss1216update.pdf):
      - PRA and company: Scoping and planning discussions
      - PRA and company: SII requirements, content of application
      - Company: completes self-assessment against SII requirements
      - PRA and company: agree work plan
      - Company: monthly reporting to PRA on progress against plan
      - PRA and company: regular face-to-face meetings to review progress
      - PRA: review and assessment of IM related aspects of systems and controls

## Pillar 2 - Qualitative requirements

- Focuses on governance, risk management and required functions (internal audit and actuarial)
- Includes supervisory review process
- Insurers required to carry out an Own Risk and Solvency Assessment (`ORSA`)
  - To be reviewed by the supervisor
- Includes ‘prudent persons’ investment principles
- Supervisors can impose capital additions for governance failings

### Corporate governance

- Board has overall responsibility for ongoing compliance with SII
- Organsiation structure: clear segregation of responsibilities, minimum levels defined in Pillar 2 framework
- Effective system of governance for sound and prudent management of business
- Written policies for each function and ensure policies implemented:
  - Risk management
  - Internal control
  - Internal audit
  - Actuarial
  - Outsourcing (where such process applied)

### Risk management function

_Article 44 of Solvency II Directive:_ **Risk management**

> Insurance and reinsurance undertakings shall have in place an effective risk-management system comprising strategies, processes and reporting procedures necessary to identify, measure, monitor, manage and report, on a continuous basis the risks, at an individual and at an aggregated level, to which they are or could be exposed, and their interdependencies.
> That risk-management system shall be effective and well integrated into the organisational structure and in the decision-making processes of the insurance or reinsurance undertaking with proper consideration of the persons who effectively run the undertaking or have other key functions.

- Risk management system covers at least:
  - underwriting,
  - reserving,
  - asset liability management,
  - investments,
  - liquidity and concentration risk,
  - operational risk,
  - reinsurance and other risk mitigation techniques
- For (re)insurers using (partial) IM, risk management function covers at least:
  - Design and implement IM
  - Test and validate IM
  - Document IM and subsequent changes made to it
  - Analyse performance of IM and produce summary reports
  - Communicate performance of IM, suggest areas to improve, update on status of efforts to improve previous noted weaknesses

### Internal control

- Internal control system includes:
  - administrative and accounting procedures
  - internal control framework
  - appropraite reporting arrangements at all levels of undertaking
  - compliance function
- Compliance risk := potential threat to earnings/business of company resulting from failure to comply with laws/regulations/stipulated practices/standards
- Internal audit function:
  - responsible for evaluating adequacy and effectiveness of internal control system and other elements of system of governance
  - objective and independent from operational functions
  - communicate findings and recommendations
  - determine actions to be taken for findings/recommendations
  - ensure actions carried out

### Actuarial function

_Article 48 of Solvency II Directive:_ **Actuarial function**

> 1. Insurance and reinsurance undertakings shall provide for an effective actuarial function to:<br>
>    (a) coordinate the calculation of technical provisions;<br>
>    (b) ensure the appropriateness of the methodologies and underlying models used as well as the assumptions made in the calculation of technical provisions;<br>
>    (c) assess the sufficiency and quality of the data used in the calculation of technical provisions;<br>
>    (d) compare best estimates against experience;<br>
>    (e) inform the administrative, management or supervisory body of the reliability and adequacy of the calculation of technical provisions;<br>
>    (f) oversee the calculation of technical provisions in the cases set out in _Article 82_;<br>
>    (g) express an opinion on the overall underwriting policy;<br>
>    (h) express an opinion on the adequacy of reinsurance arrangements; and<br>
>    (i) contribute to the effective implementation of the risk-management system referred to in _Article 44_, in particular with respect to the risk modelling underlying the calculation of the capital requirements set out in _Chapter VI_, _Sections 4_ and _5_, and to the assessment referred to in _Article 45_.<br>
> 2. The actuarial function shall be carried out by persons who have knowledge of actuarial and financial mathematics, commensurate with the nature, scale and complexity of the risks inherent in the business of the insurance or reinsurance undertaking, and who are able to demonstrate their relevant experience with applicable professional and other standards.

_Article 82 of Solvency II Directive:_ **Data quality and application of approximations, including case-by-case approaches, for technical provisions**

> Member States shall ensure that insurance and reinsurance undertakings have internal processes and procedures in place to ensure the appropriateness, completeness and accuracy of the data used in the calculation of their technical provisions.<br>
> Where, in specific circumstances, insurance and reinsurance undertakings have insufficient data of appropriate quality to apply a reliable actuarial method to a set or subset of their insurance and reinsurance obligations, or amounts recoverable from reinsurance contracts and special purpose vehicles, appropriate approximations, including case-by-case approaches, may be used in the calculation of the best estimate.

### Own Risk and Solvency Assessment (`ORSA`)

ORSA := defined by EIPOA as

> The entirety of the processes and procedures employed to identify, assess, monitor, manage and report the short and long term risks an insurance undertaking faces or may face and to determine the own funds necessary to ensure that the undertaking’s overall solvency needs are met at all times.

- Identify **all** risks subject to and related risk management processes and controls
  - Includes some of qualitative risks not assessed under Pillar 1
  - Example: Reputational risk
- Quantify ability to continue to meet MCR and SCR over business planning horizon (usually 3 - 5 years), allowing for new business
  - Not at prescribed confidence level
  - Confidence level company feels appropriate
    - Own stated risk appetite
    - Achieving target credit rating
- Evidence to supervisor that ORSA used by senior management
  - Impact of ORSA considered in strategic decisions
- ORSA contains minimum components:
  - Assessmenet of overall solvency needs
    - Considering company's specific risk profile, approved risk tolerance limits and business strategy
  - Continuous compliance with capital requirements
  - Continuous compliance with TPs
  - Consider extent which risk profile deviates from assumptions underlying SCR
- ORSA policy
- ORSA integral part of businesss strategy
  - Considered in ongoing strategic decisions
- ORSA performed regularly (minimum annually)
  - Without delay following significant change in risk profile
- Requirement: inform supervisor results of each ORSA
- ORSA process and outcome documented and independently assessed
- Explain and justify following aspects:
  - methodology and assumptions
  - results and sensitivity of results to assumptions
  - appropriateness of methodology used
  - sources of data and systems & controls around data
  - approach for dealing with parameter uncertainty and fluctations
- Minimum documentation requirements:
  - description of areas included
  - description of process of conducting ORSA and responsibilities of key personnel involved
  - stress tests used and their results
  - amount of overall solvency needs
  - financial condition of undertaking - with sign off by administrative/management body
  - strategies for raising additional own funds where necessary
  - description of independent assessment and results of last assessment
  - frequency and contents of internal reporting

## Pillar 3 - Reporting requirements

- Comprises reporting and disclosure requirements
- Public Solvency and Financial Condition Report (`SFCR`)
  - produced annually
  - quantiative templates
  - solvency calculation details
  - risk management processes
  - can apply for certain items to not be disclosed if demonstrate confidential
- Reporting to the supervisory authority of a Regular Supervisory Report (`RSR`)
  - Solvency calculation details
  - Risk management processes
  - At least triennially with summary version for other years
  - ORSA at least annually
- The aim of public disclosures is to harness market discipline by requiring firms to publish certain details of their risks, capital and risk management
- Each document includes sufficient info to assess:
  - system of governance applied
  - business pursued
  - valuation principles applied for solvency purposes
  - risks faced
  - risk management systems
  - capital structure, needs and management
- SFCR and RSR contain sections:
  - summary
  - business and performance
  - system of governance
    - description of system of governance
    - assessment of its adequacy for risk profile
  - risk profile
    - separate description for each category of risk
    - risk exposure, concentration, mitigation and sensitivity
  - valuation for solvency purposes
    - separate description for assets, TPs and other liabilities
    - bases and methods used for valuation
    - explanation of major differences in bases and methods used in valuation in financial statements
  - capital management
    - structure and amount of own funds
    - quality of own funds
      - analysis of change compared to previous reporting period
    - info to allow understanding of main difference between underlying assumptions of SF and those of IM used for calculation of SCR
    - amount of non-compliance with MCR or significant non-compliance with SCR during reporting period
      - even if subsequently resolved
      - explain origins and consequences
      - explain remedial measures taken
  - additional voluntary information
- RSR also includes:
  - business and risk strategies
  - legal and regulatory issues
  - financial and non-financial objectives
  - explanation of variance to plan
  - future developments
  - disclosure of IM results
- EIOPA publish detailed quantitative reporting templates (`QRTs`)
  - quarterly and annual reporting of quantitative financial information under SII

## Application to insurance groups

- SII enables groups to be supervised more efficiently through **group supervisor** in home country
- Group supervisor co-operatates with other national supervisors
- Ensures group-wide risks not overlooked
- Enables groups to operate more effectively whilst providing PHer protection
- Each group must cover overall group SCR
  - Allows for diversification benefits across group
  - Subject to minimum of sum of MCRs of each sub
- Each insurance sub needs to cover its own SCR
- Group supervision carried out at top level company within EEA
  - Additional rules apply to subs/parents located elsewhere
  - Impose SII requirements or for non-EEA parent: establish EU holding company
- If 3rd country regulatory regiem ~= equivalent to SII
  - Regulated as if located in EEA
  - Replaces SII rules with those of 3rd country regulatory regime
  - Full 3rd country equivalence: Bermuda, Canada, Japan, Mexico, Switzerland, US
  - Temporary equivalence: Australia, Brazil
