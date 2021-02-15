# Other Topics <!-- omit in toc  -->

- [Other Topics](#other-topics)
  - [PPOs](#ppos)
    - [Reserving for PPOs](#reserving-for-ppos)
    - [Capital for PPOs](#capital-for-ppos)
  - [Disruptors to GI market](#disruptors-to-gi-market)
  - [Emerging risks](#emerging-risks)
    - [Identifcation](#identifcation)
    - [Exposure](#exposure)
    - [Aggregation](#aggregation)
    - [Product development](#product-development)
    - [Cyber risk](#cyber-risk)
  - [Climate change](#climate-change)

## PPOs

- Certain circumstances, general insurer pay out claim as annuity rather than lump sum
  - Either: Legal court requirement to indemnify beneficiary this way,
  - Or: policy condition
  - Or: optional choice of claimant
- Claims settled this way known as **periodic payment orders** (`PPOs`)
- Equivalent to non-life annuities
- PPO := "_order made by court to pay compensation to victim of accident / act of malpractice, in form of series of regular payments rather than single lump sum_"
- Complications: size/term of payments, investment (inflation) considerations, capital requirements, RI recoveries, longevity risk, credit risk
- PPO claims arise from seriously/permanently injured, continuing & lifetime care and treatment
- Commonly awarded to young claimants => impact of injury on claimant's future life expectancy more uncertain
- PPOs rare for claims < £1m
- Introduced in 2005, prior to this **structured settlements** := optional annuity (very different characteristics / legal implications)
- Number of PPO awards grew significantly from 2008 court case "_Thompstone vs Thameside & Glossop Acute Services NHS Trust_"
  - PPOs permitted to be linked to **ASHE 6115** := index related to claimant's care costs (rather than RPI)
- Mostly arise from motor insurance
  - Also awarded for personal injury in other liability classes (e.g. EL, public liability)
  - Less common due to limits of liability (statutory minimum of EL cover in UK is £5m per event) => negates money management benefit of regular payments as stop once limit hit
- Common in medical negligence
  - NHS Resolution := body responsible for claims against public sector medical staff, large portfolio of PPO claims
- PPO form: specified sum paid every year until death, inflated in line with inflation index designed to reflect type of inflation relevant to award
  - Some PPOs have stepped payments := adjustments to annual payments (e.g. child reaches maturity => care needs change)
- Alternative to PPO is lump sum
  - If court authorises lump sum in place of PPO, calculation of lump sum based on prescribed set of mortality tables and discount rate (`Ogden tables`)

`Ogden tables` = set of tables used to calculate special damages and the present value of loss of earnings or annual expenses in personal injury and fatal accident cases. Tables provide multipliers which take account of life expectancies and a range of discount rates and are prepared by the UK Government Actuaries’ Department. The discount rate is set by the UK Lord Chancellor.

**Advantages and disadvantages of PPOs**

- Relative value of lump sum and PPO different depending on specific circumstances and risk averseness of insurer and claimant
- Longevity risk := Claimants find utility of large capital lump sum important but balance against risk of money running out while still in need of benefits
- Investment risk: insurer with PPO bears risk - difficult/impossible to match assets to liabilites
  - Nature of longevirty risk from set of young/impaired lives on small portfolio => difficult to match
  - Liabilities linked to earnings index => no matching assets
  - Long term nature => reduces appropriateness of match further
- Investment risk: claimant who takes lump sum if attempt to replicate payments received from a PPO
- Motor insurer expects handful of PPOs each year however stay on balance sheet until claimant dies (very long period)
  - Remainder of motor book mainly short term
  - Implies reserves for PPOs build up over time as proportion of overall book
- Capital requirements higher due to increased uncertainty from longevity, non-matching investment returns from assets to inflation, especially longer term
- Credit risk: Long-term nature of PPOs, increased risk of RI failure over lifetime of PPO
- Solvency II: additional reporting requirements fro non-life annuities, treated as life business once they come into payment

### Reserving for PPOs

- Approach varies by purpose (solvency, accounting, budgeting, commuting, transferring liabilty)
- Payments expected paid regularly in future, depends on annuitant survival, linked to inflation index
- Long term nature of liabilites, consistency with alternative lump sum => reserves discounted to PV
- Approach for annuity reserving varies by stage of development:
  - Annuities currently in payment
  - Incurred claims reported but not yet known whether settle as PPO
  - IBNR, some of which will settle as PPO
- Annuity payments in triangles distorts development patterns
  - Strip out such payments, value separately

**Annuities currently in payment**

- Cashflow valuation model with:
  - Current annuity level
  - Step up over time
  - Indexation
  - Life expectancy of claimant
  - Appropriate mortality table to use, include allowance for impairment
  - Discount rate (term dependent)
  - RI
- Allow for impaired mortality
  - Mortality rates based on standard published table
  - Impaired mortality allowed by loading mortality rates: additive / multiplicative adjustment or adjust age of claimant
  - Life expectancy based on medical expert in legal proceedings
- Most RI contracts have specific indexation clauses for PPOs => complicates net cashflows
  - RI contract may also **capitalisation clause** w.r.t. PPOs := if PPO settles in future, RI pay cedant lump sum to remove PPO liability from book

**Future PPOs**

- Allowance for large claims that may eventually be PPOs
- Cost of settling claim as PPO can be very different to settling it as lump sum - difference should be reserved for on claims that will settle as PPOs (but yet to do so)
- Covers claims not been settled but recognised as large / potential PPOs
- Also reserves needed for claims not yet recognised as large and claims not yet reported
- **PPO uplift** := extra amount reserved for claims that are going to be settled as PPOs
- Uplift severity calculated from insurer's average extra cost of settling claim as PPO opposed to lump sum - based on own data or market benchmark
  - Main factor: discount rate difference insurer uses to value PPO vs. used to calculate award if paid as lump sum
  - Possible uplift negative if insurer uses higher discount rate than used to convert to lump sums
- **Propensity** := frequency of PPO claim settlement
  - Little data to base this assumption
  - Care using industry benchmarks - different policy mix / claims processes
  - Depends on discount rate used to settle lump sums - claimant could receive higher lump sum as alternative to PPO => less likely to settle as PPO
- Uplift also for claims not yet reported that will become PPOs => adjustment to standard IBNR projection

### Capital for PPOs

- Capital implementations of non-life annuities complex
  - Long term nature of liabilities
  - Many risks not easily hedgeable: longevity, inflation
- High capital requirements from increased uncertainty:
  - Longevity
  - Non-matching investment returns from assets to inflation
  - Credit risk from long-term nature of PPOs
- Time horizon of SII capital measure = 1 year
  - Consider treatment for longer term uncertainties in the Own Risk and Solvency Assessment (`ORSA`) and MI
- Capital model that does not allow for PPOs => difficult to pass **Use Test**
- SII 1 in 100 stress test for longevity risk under standard form SCR => assume 20% drop in mortality rates
- Long-term risks inherent in running off PPOs will affect risk margin
  - Calculating it properly requres full investigation

## Disruptors to GI market

- Changing way insurance is transacted by disrupting incumbent approaches established over time
  - UK example: Direct Line - first personal lines insurer to offer insurance direct to consumer rather than brokers
- Recent disruption is advent of aggregators (== price comparison websites)
  - Pricing more transparent between insurance providers
  - Much wider choice offered to insureds
  - Consumers now more price sensitive, willing to shop around at renewal
- Most recent disruption: InsurTech companies
  - InsurTechs aim to improve efficiency in insurance through technological innovation
  - Find niche offerings, utilise alternative data sources, build state of the art systems to improve way insurance is transacted
  - Creates challenges to incumbents: margins competed away and anti-selection risk increases
  - Access to more and richer data => InsurTech improves risk selection and provides better service to customers

## Emerging risks

- No single agreed definition
- Emerging risk := risk which has not yet become apparent or prominent, i.e. not yet well understood, due to:
  - Not yet even know existence of risk (e.g. health implications of vaping) => **Unknown stage**
  - Not yet understand potential impact of risk (e.g. autonomous cars within motir insurance) => **Potential stage**
  - Not yet accurately and reliably quantify impact of risk (e.g. cyber risk)
  - Risk which was previously well-understood is changing such that current understanding is no longer appropriate (e.g. climate change)
    - => Current risk management techniques / analytics less appropriate over time
- Emerging risk challenges:
  - Identification
  - Exposure
  - Aggregation
  - Almost total lack of data to understand the risk

### Identifcation

- Mature LoBs => lots of experience and loss data
  - Easy to identify key risks company exposed to
  - Risks recorded and documented over time in risk register
  - Risks embedded in internal processes and policies
  - Risks in insurance policies themselves
- To identify emerging risks need to think creatively
- No single correct way to identify emerging risks
  - Use variety of approaches most effective method of identification
- Literature review
  - Emerging risk starts to become _mainstream_ => industry press and academic literature pick up on risk
- Brainstorming
  - Company asks employees / consultants to think of possible emerging risks
- What if analysis
  - Considering actual historical loss events (or near-misses), what other conditions prevailed at time, possible to identify risks which could have but have not yet emerged in past
- Process flowcharts
  - Considering each step of process in detail, what might go wrong, possible to identify risks previously gone unnoticed
- Trend analysis
  - Reviewing key datasets for trends may identify risks which no longer behave in way assumed to behave

### Exposure

- Extremely difficult to assess frequency and severity of emerging risk losses from historical data analysis alone
- Rely on expert judgement as to possible frequency and severity
- Minimise workload by initially completing at high level, then repeat at more granular level once key scenarios identified
  - Example: first identify events between: _low_, _medium_, _high_ frequency and (separately) severity
  - Risks that are high frequency, high severity warrant further investigations
  - Risks that are low frequency, low severity leave out at this stage
  - Risks that are extremely high severity investigated further regardless of assumed frequency, maybe no further action required but if risk sufficiently severe consider separately in any case
    - Due to uncertainty surrounding frequency => small underestimate of frequency of severe event could lead to ruin
- Each scenario which is further investgiated requires identification of current exposure and preferred target level of exposure
  - Identify limits / tolerances above which not willing to accept any more exposure
  - Identifying any of these items extremely difficult for most emerging risks

### Aggregation

- Monitoring aggregation of risks critical for emerging risks
- Mechanism by which losses are transferred from one area / insured / head of damage to another poorly understood until event crystallises
- Biggest challenge with emerging risks: little/no historical information on how losses accumulate when risks occur
  - Each insurer try to understand these processes
  - Involves huge amount of assumptions and uncertainty
  - Extremely hard to place reliance on these estimates
- Necessary to use very crude exposure management tools
  - Refuse to write such business at all
  - Strictly limiting total sum insued to manageable level

### Product development

- Lack of historical info => insurer doesn't adequately understand possible consequences of emerging risk
- Insurer cannot assess its current total exposure or desired level of total exposure
- Insurer cannot assess how individual contracts will aggregate, with each other or with rest of portfolio
- Result: refuse to offer cover (exclusion clauses, refuse to write standalone product) or offer very limited cover
- Always room for interpretation in assessing applicability of terms and conditions of a contract - even for well-understood risks, well-established legal prcedents / standard clauses
  - For emerging risk, risk event itself is vague, terms of contract are new / untested and no legal precedent exists
  - Under circumstances => insurer finds true exposure much higher/lower than originally intended when drafting contracts
- Leads to vicious cycle:
  - Lack of historical experience makes it hard for insurer to understand risk profile of emerging risks
  - => Few products offered
  - => Industry fails to gather new data and experience of risks
  - => Under-supply of relevant insurance relative to demand
  - => Pushes up prices
  - => Encourages firms to self-insure
  - => Increase profitability for insurers and incentivise them to develop tools/techniques/experience required to adequately manage these risk
  - However lengthy / difficult process suppresses innovation in associated industries => costly in long run

### Cyber risk

- Technology improves, host of devices increasingly interconnected => risks of errors / malicious use of technology becomes greater
- Cyber insurance relatively new product, developing over last 10 years
- Initially pricing / reserving relatively crude
- High-profile incidents of data breaches in recent times now being used to estimate frequency & severity of claims
- Accurate risk assessment is difficult => risk not yet well understood => coverage and policy wording not yet fully appropriate
- Cyber risk has massive accumulation risk
- Cyber risk large enough risk in own right => insurers offer product designed specifically for it
- Lloyd's attempts to assess cyber aggregations by asking syndicates to estimate losses to individual market-wide scenarios using the Lloyds' RDS regime
  - Provides information on aggregations within and between syndicates
  - Very crude in comparison to natural catastrophe aggregation modelling

## Climate change

- Good knowledge of extreme weather systmes
  - Hurricanes in US widely studied
  - Number of detailed comprehensive models exist for analysing risks of these event types
  - Understanding evolving but phenomena relatively well understood
  - Significant scientific literature
  - Significant historical data
- Global warming heats the earth => historical climate patterns are changing
  - Warmer seas lead to larger more powerful hurricanes
  - Higher sea levels lead to large, more dangerous storm surges
  - Existing wind and tidal processes change, creating/destroying existing feedback loops within indvidual weather systems => historical record not as relevant when considering range of possible outcomes
- Changing climatic patterns impacts range of policies
  - Example: agriculture / crop policies
  - Areas which are suitable for growth of crops changing
  - Species of plants and animals which can survive in areas is changing
  - Leads to some areas more suitable for agriculture, others less so
  - Changes likely claim frequency and severity of crop claims
  - Historical data records less relevant when considering likely claims experience
  - Changing climate common driver potentially affecting experience of greater number of agriculture policies
- Over time increasingly unable to rely on historical understanding of processes
- Affects ability of insurance industry appropriately pricing and managing associated risks
- Lead to certain perils becoming effectively uninsurable
- Lead to particular activities / geographical areas uneconomical for investment or large government schemes required
  - Example: National Flood Insurance Program (`NFIP`) in the US
  - Politically difficult - subsidising risk-takers using public funds
  - Schemes inefficient way to help encourage long-term investment in particular fields / areas
