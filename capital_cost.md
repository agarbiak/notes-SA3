# Cost of capital <!-- omit in toc -->

- [Capital modelling](#capital-modelling)
  - [Benefits of capital allocation](#benefits-of-capital-allocation)
- [Performance measurement](#performance-measurement)
- [Components of capital cost](#components-of-capital-cost)
  - [Incorporating capital costs into premiums](#incorporating-capital-costs-into-premiums)
- [Capital allocation](#capital-allocation)
  - [Coherence of risk measures](#coherence-of-risk-measures)
- [Capital allocation methods](#capital-allocation-methods)
  - [Coherence of capital allocation principles](#coherence-of-capital-allocation-principles)
- [Incorporating capital costs](#incorporating-capital-costs)

## Capital modelling

- Aggregate capital requirements reflecting overall risk to company/group
- Essential part of risk governance strategy
- Manage downside risk
- Demonstrate ability to maintain solvency to regulators, rating agencies and policyholders
- Shareholders have interest in ensuring continued solvency of insurer
- Also concerned with efficiency of business
  - Measure by performance of company relative to capital resources it uses
- Capital modelling can assist day-to-day decision making and enhance performance
  - Depends on company's ability to use risk-based performance metrics (e.g. return on capital)
  - Include such metrics in underwriting and strategic decision making processes
  - Theoretical and practical challenge: capital allocation
- Capital allocation := allocation of overall capital requirement to component parts of business based on their contribution to the overall risk profile
  - Use the allocation to determine risk-based performance measures across business
  - Enables insurer to improve profitability as can identify and develop those areas of business and opportunities that make most efficient use of limited capital resources available
  - Identify areas with highest return on shareholders' equity

### Benefits of capital allocation

- Pricing: take account of cost of capital to support the business
- Risk selection: select risks that best employ available capital
- Performance measurement: assess performance of company/BU relative to capital
- Performance attribution: between BUs, classes, individual UWers => remuneration
- Strategic decision making: assess new opportunity / examine future UWing strategy
- Reinsurance planning
- Meeting regulatory requirements - SII
- Investment strategy

## Performance measurement

- Holding money dormant is considered a burden
- Capital allocation method should:
  - be consistent with the modelled capital for the whole business
  - reflect risk of individual business segments relative to one another and the whole business
  - reflect interrelationships between risks and different business segments
    - reflect benefit of writing non-correlating LoBs in reducing the aggregate volatiltiy of business (measured relative to exposure)
  - be justifiable and consistent
- aim is to make accurate assessment of true performance of units
  - performance assessment only as reliable as capital allocation method allows
- use approach retrospectively to establish historical return on capital by operating unit
  - KPI could serve remuneration basis for front office
- Business plans use prospecitve assessment of return on capital
  - KPI is expected underwriting profit => ignores capital needed to back business
  - Use allocated capital to translate into expected return on equity
    - Expected return on equity := expected profit / allocated capital
  - Allows insurer to identify high yielding, low volatility LoBs that make most efficient use of shareholders' capital
  - Highly dependent on planned business loss ratio assumed
- Allow for return of capital when assessing strategic acquisitions / expansions into new lines
  - Allow for insurer's current portfolio and impact of new business on overall risk profile
  - Identify risk-adjusted economic value of the opportunity := marginal return on capital added to existing business
    - If positive => opportunity adds to profitability of current business

## Components of capital cost

- Capital is a finite resource => need to use capital efficiently, achieves sufficient expected return to fund elements of capital cost
  - Use sufficient margins for costs of capital in premium rates (`capital load`)
- Capacity occupation cost == non-consumptive
  - Opportunity cost to compensate firm for missing out on other opportunities
  - Holding safe investments (regulatory restrictions) => lower return than freely deployed funds
  - == Minimum risk-adjusted hurdle rate
  - ~= borrowed capital ~= capital loan (captial could be used for other ventures)
- Capital call cost == consumptive
  - Risk loading compensation for potential erosion of capital through trasnfer to reserves and eventual payout in claim payments
  - Charge depends on likelihood of transfer taking place and the distribution of amount of such a capital call
  - ~= eroded capital (passed from free reserves to technical reserves and paid to PHers as claims)
  - cost loading into premiums is _possibility_ of capital being consumed
  - Also opportunity cost associated with reduction of future undewriting capacity as result of capital erosion (from _Donald Mango_)
    - Opportunity cost charged for _capacity downtime_ period
    - Equivalent to period until lost capital recouped (future returns / parental capital infusion)
    - Portion of capital held in respect of any given portfolio required until associate liability to pay claims is fully expired

### Incorporating capital costs into premiums

- One method: allocate capital, subsequently apply loads to allocated amount for both consumptive and non-consumptive costs of capital
  - Premium = `PV_rf(expected loss)` + `capital` x `{CoC_consume + CoC_non_consume}`
  - Ignores all other loadings: expenses, RI
- Analogous to pure pricing methods that loads for capital costs without allocating capital
  - Apparent when same target return on capital imposed across the business

## Capital allocation

- Difficultly is that marginal increase in risk profile of writing new line is not more than risk profile of portfolio in isolated
  - Allocation of capital must allow for diversification benefits across LoBs
- Purpose of capital allocation:
  - Individual risk measures provide reasonable basis to determine loads to compensate for frictional costs of holding capital
    - Frictional costs := costs that arise from company holding capital even if doesn't put apital at risk by selling more business
      - Examples: taxation on investment income, lowered investment return resulting from taking less investment risk in order to give PHers more security
    - Non-frictional cost: return required by shareholders for bearing risk
  - Individual risk measures not appropriate for cost of putting capital at risk
- Allocation of capital to a LoB / individual policy requires:
  - Appropriate risk measure
  - Capital allocation methodology

### Coherence of risk measures

- Risk measure := function of random variable X representing firm's net worth at specified point in future
  - Risk that firm's net worth so low in future it must stop its activities
- Risk measure chosen should be:
  - Easy to communicate
  - Easy to apply
  - Observable, measurable, not prone to manipulation
  - Consistent with management's perception of risk
  - Quantifies risk in manner understood by decision maker
  - Consistent with basis used to establish aggregate capital requirements
  - Internally consistent wrt allocation of diversification benefits
    - Additivity of allocations
  - Results in coherent allocation
- 4 conditions for risk statistic := `coherent`:
  - `Monotonicity` := if one portfolio always worth more than another, it cannot be riskier
    - Monotonic function preserves order
  - `Linear homogeneity` := scaling a portfolio by a constant will change risk by same proportion
  - `Sub-additivity` := combining two portfolios should not create more risk
    - `f(X + Y)` &#8804; `f(X) + f(Y)`
  - `Translation invariance` := adding known guaranteed outcome portfolio to an existing portfolio reduces the risk by the guaranteed outcome
- In practice:
  - Use convexity risk measure (relaxed coherence)
  - Use incoherent risk measure
- Common risk measures:
  - Variance, Standard Deviation, Semi-Variance - widely understood statistical measures of variability
    - Provide accessible means by which to support capital allocation
    - **Incoherent** - do not satisfy monotonicity: `Var(X)` &#8804; `Var(Y)` not always held for `X` &#8805; `Y`
  - Value at Risk (`VaR`) - provides point measure of downside potentail gor given risk
    - **Incoherent** - fails sub-additivity
    - Equivalent to Probable Maximum Loss (`PML`) with subtle difference
    - PML := maximum loss expected => calculate probability of ruin
    - VaR := gives threshold once set required probability of ruin
  - Tail VaR (`T-VaR`) - conditional mean of loss distribution above selected threshold set as percentile of loss distribution
    - **Coherent** risk measure
  - Expected policyholder default - expected loss beyond company's surplus capital threshold
    - **Incoherent** - fails linear homogeneity
  - Transformed loss measures - apply transformation to loss distribution to give more weight to key focus areas of loss distribution to decision maker
    - Generally **coherent**
    - Examples: Proportional hazard transforms, Wang transforms

## Capital allocation methods

- We may not allocate _all_ capital across the LoBs
  - May keep some unallocated capital for other business ventures
  - May keep some unallocated capital for whole account risks: operational risk, group risk, etc.
- Common methods:
  - Proportional
  - Marginal last in
  - Game theory
  - Equalise relative risk
  - Co-measures
  - Option pricing framework

**Proportional method**

- Determines capital allocation with reference to single risk measure
- Measure risk of overall firm and each individual BUs
- Allocate aggregate capital requirement across LoBs proportionally to value of risk statistic for LoB
- Scale resultant allocation (where necessary) to provide internally consistent allocation of diversification benefits
  - Such that Σ(individual allocations) == whole
  - => additive property
- Advantage: simply, easy to understand and apply
- Disadvantage: do not penalise highly correlated sub-portfolios
- Disadvantage: do not give credit for low correlation sub-portfolios
- Incoherent allocation even if underlying risk measure is coherent
  - Violates diversification benefit principle

**Marginal last in** == **incremental risk approach**

- Based on capital requirement of each LoB separately as if it was last BU added
- Allocate overall capital to each LoB in proportion to its incremental capital requirement calculated
- Variant on this method == Shapley method == Game Theory method
- Use risk measure as proxy for capital requirement
- Usually Σ(marginal capital contributions) < entire capital
  - Due to diversification
  - Unallocated capital needs to be allocated
- Allocate remaining capital in proportion to marginal capital
  - Allocate total capital between BUs in proportion to each BU's marginal capital requirement
  - Approach gives low capital allocation to uncorrelated sub-portfolios, penalises highly correlated lines
  - Can be too favourable for uncorrelated sub-portfolios => high allocation of capital to correlating sub-portfolios
    - Allocation for correlating sub-portfolios higher than if considered separately => violates diversification benefit principle
  - Incoherent allocation even if underlying risk measure is coherent
    - Violates diversification benefit principle

### Coherence of capital allocation principles

- **Note**: even if use a coherent risk measure to support allocation of captial does not imply resultant allocation is coherent
  - Allocation only coherent if risk measure is coherent
- Capital allocation principle coherent if meets:
  - Diversification benefit - allocation for sub-portfolio no greater than if considered separately
  - Symmetry - if risk of two sub-portfolios is same as measured by risk measure => allocation should be the same
  - Risk-free allocation - cash in sub-portfolio reduces allocation accordingly
    - Follows from translation invariance property for coherent risk measure
    - Cash == risk-free => already available to support risks in sub-portfolio

## Incorporating capital costs

- Methods in practice are simplest to apply both technically and computationally
- Care to allow for known limitations in applying allocation method
- Pay regard to potential implications of limitations in decision making process
- Methods not used in isolation
  - Allocate capital at different levels of business
    - Allocating group wide capital to individual subsidiries
    - Subsequently to individual lines / policies
- Pricing: allocate capital to individual lines and load premium rates to allow for costs of capital to ensure adequate returns achieved
- Portion of capital held in respect of portfolio required until associated liability to pay claims fully expires
  - Different insurance liabilities pay out over different timeframes
  - Capital held against different risks for different periods
  - Issue arises: multi-period capital requirements
- Risk measure may relate directly to capital requirement (regulatory / internal capital metric)
  - Risk measure underlying capital allocation => capital allocation itself is arbitrary
  - Methods give reasonable basis upon which to allocate capital
- Further complication is cost of capital rate:
  - Overall cost of capital vs. target return rate
  - Relationship between amount of capital allocated, different capital requirements faced by firm (regulatory vs. rating agency vs. internal) and actual amount of capital held
  - Whether cost of capital should be equal across all lines

**Challenges**

- Gathering sufficient quality data to support techniques
- Sensitivity to specific assumptions
  - Ensuring robustness
- Selection of appropraite risk measures
  - Understood and accepted across business
- Ensuring consistency with companies' broader enterprise risk management framework
- Communication and interpretation of results of capital allocation across business
- Sufficient staff and resources to embed capital considerations in real-time day to day decision making
- Incorporation of capital loads at a risk level
- Allowance for fixed capital costs such as operational risk
  - Seldom directly attributable to specific LoB
- Help underwriters appreciate the gearing of returns on capital
  - Hence significance of pricing terms and conditions
- Convincing senior management of benefits of return on capital considerations as way of enhancing business performance
  - Rather than just satisfying regulatory management requirements
  - Relies upon risk-based measures always remaining relevant, informative, up-to-date and timely
- Evolving methods over time as understanding of risks improves
- Solvency II requires insurers to satsify the _Use Test_
  - Demonstrate capital methods are embedded across the business
