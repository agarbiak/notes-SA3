# Business planning <!-- omit in toc -->

- [Modelling](#modelling)
  - [Reasons for financial models](#reasons-for-financial-models)
- [Financial plan](#financial-plan)
- [Modelling assumptions](#modelling-assumptions)
  - [Time horizon](#time-horizon)
  - [Risk measure](#risk-measure)
  - [Economic environment](#economic-environment)
  - [Investment return](#investment-return)
  - [Insurance cycle](#insurance-cycle)
  - [Future written premium income](#future-written-premium-income)
  - [Future claims](#future-claims)
  - [Reinsurance](#reinsurance)
  - [Future expenses](#future-expenses)
- [Deterministic modelling](#deterministic-modelling)
- [Stress and scenario modelling](#stress-and-scenario-modelling)
- [Stochastic modelling](#stochastic-modelling)
- [Dynamic financial analysis (`DFA`)](#dynamic-financial-analysis-dfa)
  - [DFA Purpose](#dfa-purpose)
  - [DFA Functionality](#dfa-functionality)
  - [DFA Strategic Areas](#dfa-strategic-areas)
  - [DFA Model](#dfa-model)
  - [DFA Regulation](#dfa-regulation)
  - [DFA Issues](#dfa-issues)

## Modelling

- Primary objective = enable actuary to give insurer appropraite advice so it can be managed in sound financial way
- Use models to assist in day-to-day running of insurer and provide checks on business
- Model requirements:
  - Be valid, rigorous enough for its purpose
  - Documented, including limitations on its use
  - Model chosen capable of reflecting risk profile of financial products, schemes, contracts, transactions being modelled
  - Parameters used allow for all features business being modelled that could significantly affect advice given
  - Inputs to parameter values appropriate to business modelled, take into account special features of provider and economic & business environment operating within
  - Allow for appropriate joint behaviour of model variables
  - Principles of modelling easy to appreciate, communicate and clearly display results
  - Outputs capable of independent verification for reasonableness
  - Outputs communicable to whome advice given to
  - Not too complex that results difficult to interpret or communicate
  - Not too complex that model too long / expensive to run (unless required by purpose of model)
  - Avoid impression everything can be modelled
  - Capable of development and refinement (nothing complex can be successfully designed and built in single attempt)
  - Range of methods of implementation available to facilitate testing, parameterisation and focus of results
  - Meet regulatory requirements if used for regulatory purposes (e.g. capital setting under SII)
- Documentation clearly state where requirements above not met
- Four main types of financial planning models:
  - Deterministic
  - Stress and scenario
  - Stochastic
  - Dynamic Financial Analysis (`DFA`)

### Reasons for financial models

- Premium calculation
  - Derive risk premium per policy
  - Select rating factors
  - Determine premiums using experience-rating procedures
  - Estimate effect of changing level of cover by changing levels of deductibles
  - Estimate effect of changes in terms and conditions of policy wording
- Capital requirements / solvency
  - Assess and project capital requirements of company
    - Regulatory viewpoint (SII SCR, SII MCR)
    - Internal targets (TVaR, return on capital)
  - Allocate capital to different classes
  - Assess effect of changes in business mix in portfolio
- Business planning
  - Assess benefits and costs of reinsurance programmes
  - Assist design of suitable reinsurance programme
  - Estimate likely variability of claims experience
  - Reserve for uncertainty
    - Example: estimate possible effect of industrial diseases on reserves run-off
  - Value portfolios for purchase / sale
  - Optimise investment strategy and asset performance
  - Identify trends in claims at early stage
    - Example: decline in performance of certain contracts
  - Assist senior management's strategy decision making
  - Assist senior management develop business strategy

## Financial plan

- Aim = set out courses of action that support / meet company's short-term targets and longer-term strategic vision
  - Subdivided and explained to level of detail consistent with its purposes
- Insurer's management will agree such targets and vision with owners (e.g. shareholders)
- Financial plan should have:
  - one or more goals
  - strategy to follow to achieve goals
  - set of targets that enable success / failure of strategy to be measured
  - financial projections
- Actuarial control cycle forms basis for considerations behind any financial plan
- Key benchmarks in plan:
  - expected loss ratios (gross and net of RI)
  - new business volumes and renewal retention rates
  - capital implications
  - overall profitability of company moving forward
- Financial models support financial planning, often viewed over extended period
  - Example: takes time before profits realised as costs of entering new market is high
- Model needs to reflect:
  - nature, size and structure of insurer
  - future financial position of insurer under different scenarios
- Implementing plan costs money => insurer decideds if initial costs outweighed by future additional profits generated by implementing plan
- Can evaluate economic value of individual contracts sold by insurer using NPV techniques
  - Testing proposed premium rates by projecting possible levels of future business, claims, expenses, investment experience and profit
  - Could be simple model looking at business in isolation
  - Could be part of larger model, incorporating dependencies between other parts of business
  - Can project P&L and Balance Sheet accounts to determine expected future profits and future financial strength of company
    - Detailed short-term projections made
    - Long-term projections less detailed as greater uncertainty => spurious accuracy

## Modelling assumptions

- Many assumptions in modelling process
- Depends on purpose and level of model sophisticiation
  - More assumption may be required

### Time horizon

- Capitalisation horizon := number of years new business modelled
- Modelling horizon := number of future years cashflows projected
- Modelling horizon &#8805; capitalisation horizon due to run off
- Choose horizons based on type of liability modelling uncertainty
  - Year on year uncertainty (e.g. probability of insolvency over next year)
  - Uncertainty to ultimate
- Capitalisation horizon influenced by benchmarks from senior management / owners
  - Example: senior management may have specific targets looking to deliver at end of 5 years => model both existing and new business during the period
- Regulatory requirements influence horizons
  - Example: SII 99.5% One-year VaR

### Risk measure

- Each variable (e.g. NAV, loss ratio) determine risk measure
  - Examples: standard deviation, VaR, TVaR

### Economic environment

- Assumptions about future inflation, interest rates and currency exchange rates
- Allow for other features of economy
  - Example: increased claim frequencies associated with increased moral hazard during a recession

### Investment return

- Assumptions about future investment return depend on investment prospects and on current & projected future investment policy
- Assumptions should be in line with chosen economic environment
- Allow for defaults

### Insurance cycle

- Including impact on loss ratios and premium volumes
- Allow for different classes being at different stages in cycle

### Future written premium income

- Project separately for each LoB
- Time interval (monthly, quarterly, annually) depends on level of accuracy needed
- Potentially split figures by source of business
- Set assumptions based on discussions with sales managers and underwriters
- Allow for growth in business volumes expected after putting plan in operation
  - Consistent with target loss ratio
  - Example: if assumed loss ratio lower than market average => hard to justify high growth rate unless product price insensitive
- Projected premium income and attaching loss ratios should be consistent with underwriting cycle stage for LoB
  - Requires discussion with management to understand extent intend to follow underwriting cycle for each LoB
    - Example: strategic decision to maintain profitability in softening market => assumptions about loss of volume as competitiveness reduces

### Future claims

- May split future claims into loss types:
  - Attritional - based on loss ratio model
  - Large - frequency / severity model
  - Catastrophe - CAT model (where avaialble) or frequency / severity method
- Adequate reinsurance cover may limit effect of CATs => impact on cashflows reduced
- Sources of claims:
  - IBNeR claims (development of historical notified claims)
  - IBNR claims
  - Claims from unexpired risk period on existing business
  - Claims from future written business
- Seasonality to allow for actual vs. expected experience

### Reinsurance

- Reinsurance market cycle
- Existing arrangements
- Changes likely to be made to such arrangements
- Possible new arrangements that could be put in place
- Financial strength of reinsurers
- Exhaustion of reinsurance coverage from adverse development of historical claims
  - By exhaustion of limits
  - By reinsurer insolvencies
- Effect greater for smaller companies that purchase more reinsurance
- Availability and cost of reinsurance
  - Consistency with premium income and other assumptions
- Flex reinsurance assumptions => tailor ideal reinsurance package to find desired output

### Future expenses

- Some expenses = function of other assumptions in plan
  - Commission = % of written premium
    - Care needed if distribution mix is shifting => current average commission rate not applicable in future
- Other expenses more difficult to predict as depend on projected business growth and staffing plan
  - Examples: staff costs, rents
  - Discuss such assumptions with management

## Deterministic modelling

- Developing deterministic model steps:
  - Specify purpose of investigation
  - Collect data
  - Group and modify data into relatively homogenous LoBs
  - Choose form of model
    - Identify variables and parameters
  - Ascribe parameter values using past experience (where appropriate)
    - Use appropraite estimation techniques
  - Check goodness of fit is acceptable
    - Attempt to fit different model if not
    - Avoid overfitting
  - Run model using selected values for variables
  - Run model using estimates of values of variables in future
- Run model using different values for variables to assess sensitivity of results
- Judgement from suitably experience person required to help assess / select parameters
  - Data may be scarce
  - Data doesn't capture features we expect to occur

## Stress and scenario modelling

- Stress test assesses impact on financial plan of major change in single assumption in model
  - Example: major change in future inflation rate
- Main features of stress tests:
  - Assigns no probability to events considered
  - Only looks at extreme situations => needs to be coupled with other techniques (e.g. simulation) in order to understand full range of outcomes
  - Can be used to assess suitability of response strategies by assessing impact of stress in absence of any response and in presence of proposed response
- Scenario test assesses impact of combination of stress
  - Example: assess impact on solvency of a large catastrophe together with one or more reinsurers defaulting
  - Scenario analysis concerned with looking at results from model under various scenarios representing plausible sets of future conditions

## Stochastic modelling

- Stochastic model helps assess likely variability of claims experience
- Various methods to assess variability of claims experience:
  - Determine number of claims stochastically, assume deterministic mean claim cost
    - Divide claims into homogenous groups wrt claim size
  - Determine claims amounts stochastically for expected number of claims
  - Determine both claim amounts and frequencies stochastically using collect risk model
- Developing stochastic model steps:
  - Specify purpose of investigation
  - Set risk measure
  - Collect data
  - Group and modify data into relatively homogenous LoBs
  - Choose suitable density function for each variable to be modelled stochastically
  - Specify dependencies / correlations between variables
  - Estimate required parameters for chosen probability density functions
  - Check goodness of fit is acceptable
    - Attempt to fit different density functions if not
    - Avoid overfitting
  - Construct model based on chosen density functions
  - Run model many times, each time using random smaple from chosen density functions
  - Produce summary of results that shows distribution of modelled results after many simulations run

## Dynamic financial analysis (`DFA`)

- Dynamic financial analysis == Dynamic Solvency Testing == model office
- DFA := stochastic model that incorporates feedback loops and management intervention decisions
  - Enables evaluation of differences in financial results arising from alternative strategic decisions by:
    - Replacing one set of strategic decisions with another
    - Re-running model
    - Comparing range of possible outcomes under each decision path
- Four main risk areas for insurer:
  - Claims risks
  - Expense risks
  - Investment risks
  - Business risks
- Integrated DFA := DFA that combines many aspects of insurer's functions (investment, underwriting, pricing, etc.), enabling company to understand operation of each function and their interactions

### DFA Purpose

- Overall aim = enable management to make better-informed decisions by analysing more explicitly links between risk, capital and return
- Provide management with:
  - Information about interaction of decisions from all areas of company operations
  - Quantitative view of risk-return trade offs inherent in emerging strategic opportunities
  - Structured process for evaluating market alternatives
- Tool to allow management to acheive fundamental aims of insurer:
  - Absorb transfer of policyholders' risk
  - Earn appropraite return on shareholders' capital
  - Minimise company's exposure to insolvency

### DFA Functionality

- Apply same macroeconomic conditions across all divisions and departments of insurer
  - Interest rates, inflation rates, catastrophic events
- Allow management to consider operating needs and conditions in financial markets they make investment decisions
- Examine risk-return trade offs of investment and operating decisions for entire organisation
- Allow management to choose reinsurance programmes for various departments and coordinate them for entire company all at once
- Build in effects of changes in external influences

### DFA Strategic Areas

- DFA model supports strategic decisions across:
  - Realism of busines plan
    - Examples: explain why last year's plan failed, assess probability of not achieving next year's plan (and why)
  - Product and market development
    - Examples: investigate possible success of new product / advertising campaign, competitor responses to change in premium rates
  - Claims management
    - Example: analyse effect on reserves of new claims settlement philosophy
  - Capital adequacy
    - Example: assess probability of ruin given catastrophic claim event
  - Capital allocation
    - Example: ascertain most appropriate way of allocating capital across various LoBs given risk profile
  - Liquidity
    - Assess whether given liabilities of company assets are appropriate to ensure no cashflow problems
  - Reinsurance structure and cost
    - Assess extent / suitability of reinsurance programmes
  - Asset / investment strategy analysis
  - Rating agency support
    - Demonstration of risk management techniques
    - Showing rating agency that company's risk models are rigorous => improve (maintain) agency's perception and credit rating
  - M&A opportunities
    - Assessing whether price paid for acquisition reflect risks and possible outcomes
  - Closure of books of business

### DFA Model

- Means of gaining knowledge through combination of analysis, data and technology
- Only as valuable as information that comes out of it
- Results depends upon how well model reflects reality
- Spend considerable time testing and validating variables used
- Developing DFA model steps:
  - Select appropraite model structure
    - What business areas to include
  - Decide variables included and interrelationships
    - Examples: claim costs, premium growth
  - Determine scenario types to be developed and modelled, e.g.:
    - interest rate environment,
    - competitive environment,
    - insurance cycle
  - Estimate parameters that should be used for each variable (mathematics that specifies variable behaviour)
  - Test and validate reasonableness of assumptions and their interactions
    - Example: projection of future vs. historical levels of claim payments
- Confidence in DFA results depend on data and model used
- Continously update model => relevancy and changing environment insurer operates
- Model should continue to reflect reality

### DFA Regulation

- Many regulators require insurers to use DFA modelling if models used to set regualtory capital
- Many companies and all Lloyd's syndicates built internal capital models to calculate the SII one year SCR
  - Lloyd's Syndicates' models must also calculate the ultimate SCR
- Multi-underwriting year models / series of overlapping one year models also built to calculate ORSA capital
- Rating agencies typically expect DFA / VaR modelling
  - Important discussion area as gives rating agencies insight into insurer's financial risk tolerance (i.e. ruin risk)
  - If DFA / VaR modelling not undertaken => risk of downgrade => loss of business => possible insolvency

### DFA Issues

- Can be complex => results difficult to interpret
- Results difficult to communicate to Board of Directors
- Requires many assumptions, often subjective, especially on tail risk and tail dependencies
  - Substantial use of expert judgement
  - Requires experience and additional levels of validation and documentation
- Models specific to each group
  - => difficulties in consistency of approach
  - => difficulties in comparability of results
- Lack of market standards => issue for regulators and rating agencies
- Garbage in => garbage out
  - DFA model only as good as underlying data input allows
