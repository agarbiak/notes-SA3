# Pricing large risks <!-- omit in toc -->

- [Large risk definition](#large-risk-definition)
  - [Large clients](#large-clients)
  - [Schemes](#schemes)
  - [Delegation](#delegation)
  - [Line slips](#line-slips)
  - [Features](#features)
- [Operating environment](#operating-environment)
- [Understanding the client](#understanding-the-client)
- [Risk appetite](#risk-appetite)
- [Understanding coverage](#understanding-coverage)
- [Data](#data)
  - [Source, Format, Frequecy](#source-format-frequecy)
  - [Types of data](#types-of-data)
  - [Terminology](#terminology)
- [Technical Rate](#technical-rate)
- [Technical Methods](#technical-methods)
  - [Burning cost approach](#burning-cost-approach)
  - [Frequency severity approach](#frequency-severity-approach)
  - [Simulation](#simulation)
  - [Exposure rating](#exposure-rating)
- [Negotiation](#negotiation)
- [Portfolio management](#portfolio-management)

## Large risk definition

- Risk / group of risks which are to some extent unique
  - Calculations done which are applied once to that one risk
  - Unique nature of risk => calculations carried out for other risks and portfolios limited use for large risk under consideration

### Large clients

- Large risks can be vastly different in terms of size (exposure) and in terms of occupation, construction, susceptibility to natural disaster
- Large and complex risks individually underwritten
  - Underwriter uses unqiue info about the risk to dictate terms and conditions
  - Underwriter can be flexible in approach
    - What cover is offered
    - How cover is applied
    - What pricing is needed to fit precisely coverage required
- As companies get larger / more complex => circumstances change => challenge for pricing actuary:
  - Larger companies typically carry out more than one type of work,in more than one location
  - Amount company can afford to spend on risk management increases
    - Differences between good / bad risk management more noticeable
  - Larger companies likely use captives for self-insurance
  - Level of each premium higher => underwriter spend more time looking at each risk
  - Exact terms and conditions of cover and levels of sums insured change from being same for each risk
    - Subject to negotiation, e.g. at each renewal
  - Potentially claims handled up to limit by client in-house
  - Potentially claims handled by client's preferred claims handling company
  - Claims handling company may change over time
  - Contract features (e.g. aggregate deductibles) that lead to greater volatility => futher consideration needed

### Schemes

- Contract between insurer and another institution wherby insurer insures group of thrid parties agreed under contract
- Not one insured risk but group of insured risks priced collectively under one contract
- Risks likely to be similar to one another
  - Similarity via trade association / affinity group
- Alternatively individual risks share a defined brand
  - Likely individual risks sourced via same intermediary
- Schemes cover personal and commercial lines
  - Nature of scheme affect approach used in pricing risks
  - Approaches vary widely
  - Example: commercial motor insurance scheme cover for cars and vans => priced similar way to personal lines scheme
    - Volume and data available for this scheme enables pricing exercise similar to book of private motor business (credibility approach: weight on fleet's past claims experience, weight on standard book rates)
  - Example 2: car dealership, policies in scheme are private motor insurance policies sold when dealership sells new/used cars
    - Affinity relationship: all policyholders bought new/used car from same dealership
    - Scheme mirros book of private motor business to some extent => priced similarly
- Where group of risks within scheme priced collectively with set of rates that apply only to that group of risks (scheme) => scheme := pseudo large risk
  - Example: Local authority scheme providing liability insurance for members (individual local authorities)
    - Individual risks share affinity since all local authorities
    - Volume and data available unlikely sufficient to price similar to personal lines business

### Delegation

- Most schemes involve element of delegation
  - Claims handling, underwriting, sales, etc.
- More functions delegated => less control insurer has over part of process and data associated with that function
- Managing general agents (`MGAs`) / coverholders / brokers can also perform underwriting, policy and claims handling
  - Insurer effectively operates as capacity provider, continues to take on the risk
- Schemes involve some form of profit share => profit commissions
- Schemes/MGAs can be shared across more than one insurer => coinsurance arrangement
- Coinsurance common for large commercial risks
  - One insurer alone does not have risk appetite / capital to carray risk itself

### Line slips

- Line slip := agreement between underwriters and broker whereby participating underwriters allow lead underwriter to underwrite and bind risks on their behalf
  - Lead underwriter takes significant share of risk
  - Following underwriters take smaller shares
- Follow underwriters want to know whether decision to participate in line slip is profitable
  - May also want technical advice whether to continue participating
- Binding authorities (`binders`) := contractual agreements setting out scope of delegated authority, allowing coverholders to enter into contracts of insurance and issue insurance documents on behalf of Lloyd's managing agents

### Features

**Distribution**

- Most large risks traded through traditional broker channel
- Broker channel changed significantly due to acquistive nature of some brokers recently
- Distribution channels for small and large risks very different
  - Both in constant flux
- Actuary practising in particular LoB should understand the distribution channels used
  - Distribution channels can affect remuneration methodologies
  - Understand market dynamics and business pressures of those whome actuary is advising

**Markets**

- Large commercial risks often traded in LM or Lloyd's
- _Verticalisation_ := different coinsurers have different terms (premium rates)
  - Leader terms better than follower's terms
  - Difference between lead and follower terms greater in soft market than hard market
  - Norm in aviation
  - Speculation EU wants to make it norm everywhere on competition grounds
- Most large risks coinsured due to size => no one insurer takes on 100% risk
  - Each insurer takes proportional share of risk
  - _Percentage of whole risk_ := percentage of 100% value of the layer / insured value
- Sometimes only certain percentage will reach market => some retained by insured or goes to another market
  - _Order percentage_ := percentage that reaches the market

**Unique coverage**

- Negotiation on terms and conditions for each individual risk
- Tailor unique coverages for client
  - Combination of policy wordings that do not exist elsewhere
  - Totally new policy wordings

## Operating environment

**SME risks**

- Long history of pricing actuaries involved
  - Role well established
  - Clearly understood by management, underwriters
  - Degree of formality: pricing committees, procedure notes, pricing reviews
- Technical rate often known with reasonable degree of accuracy
  - Past experience of similar risks => guide to future experience of new risk
- Technical rate built into systems to deliver market rate after agreement at pricing committee
- Price flexibility at point of sale not typically due to technical rate assumption being inaccurate but due to (for given distribution channel):
  - maximise commission,
  - maximise profit,
  - or maximise sales volumes

**Large risks**

- Pricing actuary has many roles, including:
  - Calculate minimum technical rate
  - Act as _"second pair of eyes"_
  - Assess adequacy of rates set by lead market
  - Audit
  - Sign off pricing and other terms & conditions as part of license process
  - General advice to underwriter
  - Design rate monitoring processes and systems that capture relevant data
  - Allow for accumulation control (monitor exposure)
  - Help negotiate and explain rates to third parties (e.g. RIers)
- Less developed, less structured role
  - Need to have right knowledge, experience, personality and support in the company
  - More direct contact with underwriters
  - Pressure to agree technical rate near underwriter's current market rate
- Management unclear as to exact role the actuary should play
- Large degree of uncertainty of the technical rate
- Consequence of significant mistakes => large losses, reputational damage to actuary and the profession
- Contact and influence over:
  - agents/brokers
  - client risk managers
  - underwriters and negotiators at insurance company
  - claims department
  - senior management

## Understanding the client

- Essential to understand the client behind risk being priced
- Data / knowledge held depends on new business proposition vs. renewal
- Debates and discussions with the underwriter, client, broker important to gain information not found on cover schedule / elsewhere

**Questions**

- _What claims have been experienced?_
  - Most fundamentla question
  - Challenging if claims handler changed over time
    - Inconsistent case reserving in historical data
  - Inconsistencies arise from:
    - changes in claims handling processes
    - level of product cover
    - legislation
- _Why is the client seeking insurance?_
  - Client's balance sheet bigger than insurer's so why does it want insurance?
  - Legal reasons: motor insurance, UK EL
  - Avoid volatility in the P&L from its underlying core operations that could arise if had to settle all potential claims itself
  - Cover for all claims / only proportion of them
    - Prepared to share risk with insurer via high deductibles / other methods
    - Pricing arrangement => understand why client interested in this approach / whether such approach is suitable/viable
- _Is the client a multinational, requiring cover in many territories?_
  - Should reflect local differences:
    - Claims consciousness
    - Different legal costs
    - Pro-plaintiff judgements
  - Insurer higher costs from multinational programmes as:
    - issues local policies to be legally compliant
    - survey costs
    - collecting premiums
    - claims handling
    - tax implications
- _Has the client changed significantly over time?_
  - M&A and disposals can alters risk profile of client => future claims experience
  - Implies past experience not necessarily guide to future
    - Example: Client requiring commerical property cover
    - Historically areas not prone to flooding
    - Now merged with company with large presence in several floodplains
    - Implies flood risk now much higher than previously
    - However separate flood risk of two companies prior to merger commmensurate with combined flood risk after merger
  - M&A and disposals can alter cover required by client
    - Example: Client previously owned large fleet of motor vehicles
    - Since last renewal disposed of fleet
    - Implies client no longer requires motor fleet cover
- _Has there been any changes in process used by the client that will affect nature of risks exposed to => claims experience?_
  - Example: Large printing establishment
    - Printing industry used to use large mechnical machines in production
    - Gives risk to injuries amongst print workers
    - Now process is mostly controlled by computers
    - Fewer injury claims seen for this type of machinery
- _What level of risk management does the client have?_
  - Risk management := tools and processes in place to reduce risks that can lead to potential claims
    - Financial tools:
      - RI
      - Underwriting
      - Diversification
      - Financial engineering
    - Non-financial tools:
      - Health & Safety training
      - Installation of sprinkler systems
      - Signs warning wet floors => less slipping claims
  - Large clients have good understanding of risk management
    - Improves claims experience
    - Reduces premium
  - Disparities on actual risk management controls
    - Influences assumption about future frequency & severity of claims
    - Assumptions influenced by changes in level of risk management over time
- _Is this client now more like another that has already been priced?_
  - Experience of another similar risk better indication of expected claims experience than client's own claims history

## Risk appetite

- Insurers agree how much risk proposed to take on
- Monitor amount of risk taken
- Regulatory requirement
- Rating agency requirement
- Defining and administering company-wide coherent risk appetite => not simple
  - Especially true for large multinationals operating in multiple markets and LOBs
- Separate risk management function
  - Led by Chief Risk Officer
  - Global and local departments
- Pricing actuaries should understand elements of risk appetite and risk control structure that affect underwriting and pricing of insurance contracts
  - Issuing one extra large risk policy could cause insurer to exceed risk appetite

**Insurer control structures**

- _Underwriter licensing_ := _underwriting guidelines_
  - Each underwriter has license to write risks of certain type / up to certain sum insured
  - Limit beyond which even head of LOB cannot expose insurer
    - Referred to board level
  - Limit exposure to accumulations of risk
  - Ensure sufficient scrunity given to largest / unusual risks before insurance written
  - Similar limits and processes apply for purchase of facultative reinsurance
- _Accumulation monitoring and control_
  - Some perils result in loss across more than one property / insured
  - Underwriter needs to consider accumulation issues when assessing / pricing large risks
  - Underwriter allows for additional volatility within pricing approach, treaty reinsurance charges, limiting capacity available for particular peril, increasing price to reflect scarcer capacity
  - Historically insurers over relied on model estimates of minimum return period (level of loss not to exceed more than once in x years)
    - Insurers would buy RI up to this level
  - Recent events shown dangerous to rely on such models considering risk to which company exposed
  - Insurers now look at probable maximum loss (`PML`) that could arise in one geographical area by defining geographical blocks of certain size and considering PML on all risks in each block
  - Control structure might mean once certain limit reached in PML block, no futher risks can be written in that PML block
    - Causes issues where large risk has one out of thousands of properties in PML block that is not at limit
  - `PML` (probable) := "_Attempt to quantify exposure, and is used in rating or to judge requirements for outwards reinsurance_"
  - `PML` (possible) := "_Implies the consideration of more remote scenarios than those for probable or estimated maximum loss and therefore carries a higher value_"

## Understanding coverage

- Large programmes require extensions / enhancements and higher limits than SMEs
- Businesses insured under multinational programmes have differences in cover between local and master policies
  - Master: primary details of cover
  - Locals: supplementary details of cover for each country (e.g. to comply with local legislation / different PHer needs)
- Non-standard covers
- Unique covers for each client
- Extract covers thrown in (sweetners in a soft market)
- Differing deductibles for different covers
- Issues vary from each large risk => understand cover and coverage specifically negotiated for risk being priced

**Liability coverage**

- Retroactive employers' liability / public/product liability covers
  - Policies where insured is covered for negligent acts, errors or omissions that are reported during policy term but where acts predate policies' inception
- Financial loss extensions
  - Example: adding consequential loss to standard liability cover
- Residual / excess employers' liability - providing cover in excess provided by underlying liability policy
- Excess motor liability
- Personal injury
- Vendor's liability - liability cover for vendors / exhibitors at exhibitions / trade shows
- Environmental pollution liability

**Property**

- Differences in condition (`DIC`)
- Differences in limits (`DIL`)
- Insurance company issue local policies in each area of multinational client's operations and properties
  - Write highest limits / more complex covers only under policies in certain country
  - Master policy need to cover DIC and DIL between local covers and those required under insurance programme
- Covers where insurer prefer local lower limits:
  - Business interruption extensions (suppliers' / customers' denial of access)
  - High risk catastrophe covers (e.g. CA EQ)
- Other coverages integrated with property _all risks_ covers
  - Goods in transit
  - Construction

## Data

- Less likely data available for large risks pricing
- If past data not available => terms offered reflect this

### Source, Format, Frequecy

- Source of underlying data:
  - client
  - broker / agent
  - insurer on its systems
  - combo
- Format of data:
  - pure underlying raw data download
  - processed data download
  - processed data in management information report
  - processed data sent in bordereau (high level financial figures)
- Frequency of data:
  - on request
  - monthly / quarterly
  - less frequently
- If underlying data processed on insurer's systems => superior quality than info from intermediary / client
  - Unless less flexible
- Intermediary most likely pass processed / summarised data
  - Insurer should ask for more insight / visibility of account performance
- Passing timely, accurate, appropraite data to insurer forms part of contract
  - Allow penalties if not honoured

### Types of data

- Policy data
  - List of policies
  - Rating factors
  - Sum insured
    - At each location
    - Potential accumulation risk from particular risks (wind, EQ, etc.)
    - Match claims back to individual asset (location)
  - Deductible information
  - Number of policies sold and premium written for period of report
  - Total sum insured for period of report
- Claims data
  - List of claims as at date of report
    - Associated dates, payments to date, current outstanding claims
  - Number of claims and total payments and outstanding as at date of report
  - Claims development triangles as at date of report
  - Large claims list above agreed threshold
  - Context of claims data:
    - if excess only => insurer misses attritional claims experience
    - if all claims := froun the ground up (`FGU`)
  - Poor claims data => push for completeness
  - Talk to claims handlers
    - Provide info not apparent in data
    - Provide explanations for oddities in data
  - How changing insurers / claims handlers could impact historical claims experience
- Other data
  - Survey reports
  - Client's website / annual report
  - Background information from broker / agent / client

### Terminology

Need to clarify terms

- Premium:
  - Earned or written?
  - Quoted net => net of what? Net of RI? Net of commission?
  - Delegated authority business:
    - estimated premium for policy period?
    - premium written?
    - premium received to date?
- Claims:
  - Just claims paid and case estimates?
  - Also IBNR estimated included?
  - All claims group up? Amounts and counts?
  - Just claims (and counts) above excess?
  - Rates of exchanged used?
  - Currency consolidation?
  - Changes in claims handling over time?
  - Claim frequencies:
    - Nil claims included?
    - Just non-nil claims?
  - Basis of claims reporting:
    - loss occurring
    - risks attaching
    - claims made
  - Summary claims format:
    - Losses-occurring basis => accident date grouping
    - Claims-made basis => reporting date grouping

## Technical Rate

Key stages in arriving at technical price:

1. Understanding aspects of risk and insurance terms and conditions that could lead to cash inflows / outflows
2. Technical pricing based on data available

**Cash inflows / outflows**

- Premium payment
  - Profit share payable after end of year (if claims experience is good)
  - Minimum level of premium with additional premium only paid when some measure related to claims exceed certain amount
  - Maximum premium
  - Minimum premium paid up front, adjusted after end of coverage period to allow for actual exposure
  - Premiums linked to claims experience
- Term of policy
  - Longer than 12 month policy
  - Long-term agreement (`LTA`), where premium is fixed for years at outset (e.g. 3 years)
    - Fixes premium inflow over three years
    - Outflow varies
    - RI costs vary significantly over three years
    - Insurer may end up paying more in RI than original premium
  - Break clauses (e.g. if claims experience deteriorates)
  - Multi-year risks (e.g. construction)
    - Sum insured varies by period
    - Premiums shown in original year proportionally
    - Re-rated subsequently based on actual exposure (re-signing)
    - Re-rated subsequently based on emerging experience
- Facultative reinsurance
  - Large risks often exceed risk appetite of insurer
  - Insurer writes risk but as coinsurance or by facultatively reinsuring some risk
  - Costs and profits of reinsurers need to be priced in
  - Need to know if underwriter will buy facultative covers, if so:
    - cost of facultative reinsurance
    - level of expected recoveries from contract
- Expenses
  - Insurer agree specific service levels with client
  - Each service level has implied cost to insurer
  - Example: new business team agree to dedicated claims team / telephone line for client
    - Need to allow correctly for such marginal costs
  - Pricing actuary needs to perform expense analysis
    - Expected number of claims
    - Current headcount of claims department
    - Claims handled per annum
    - Claims volume in excess of capacity?
- Commission
  - Some large risks: insurer pays fee instead of commission
  - Need to understand all premium deductions
  - Profit commission agreement with broker
    - Broker may pay rebate commission to original insured
- Cost of capital
  - Some subsidiary insurance companies, parent company require divident based on notional capital allocated to each company
    - Cost of capital is real outflow
- Investment income
  - Premium income generates investment income
  - Which party benefits from investment income
  - Build allowance into premium
  - Captial held by insurer also generates investment income
    - Allow for in premium

## Technical Methods

- Key difference between SME and large risks is potential for very large loss
- Often decision making drive for underwriter
- Relatively small nubmer of events
- Historical loss information difficult to assess
- Underwriter needs to allocate proportion of premium to _"large loss fund"_
  - Challenge: how much to allocate on insured-by-insured basis
- Portfolio managers can use reinsurance treaties to manage accumulation risk over small-risks portfolio
  - No single risk is likely to result in very large loss
- Large risk underwriters careful about insurer's capacity to accept risks and use treaties both to limit extent of individual large losses and accumulation potential
  - Can use price of reinsurance as rough guide to how much allowance should be made in original premium for large losses and accumulations
  - Pricing up to these limits challenging (lack of historical claims info)

### Burning cost approach

### Frequency severity approach

### Simulation

### Exposure rating

## Negotiation

## Portfolio management
