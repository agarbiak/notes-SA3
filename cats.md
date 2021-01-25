# CAT Models <!-- omit in toc -->

- [Why CAT models exist](#why-cat-models-exist)
- [CAT model development](#cat-model-development)
- [CAT model overview](#cat-model-overview)
- [Structure of CAT models](#structure-of-cat-models)
  - [Event module](#event-module)
  - [Hazard module](#hazard-module)
  - [Inventory module](#inventory-module)
  - [Vulnerability module](#vulnerability-module)
  - [Seconary uncertainty](#seconary-uncertainty)
  - [Financial analysis module](#financial-analysis-module)
  - [CAT modelled loss example](#cat-modelled-loss-example)
- [Perils in CAT models](#perils-in-cat-models)
  - [Tropical cyclones](#tropical-cyclones)
  - [Extra-tropical cyclones ("ETC")](#extra-tropical-cyclones-etc)
  - [Tornadoes](#tornadoes)
  - [Earthquake ("EQ")](#earthquake-eq)
  - [Non-natural perils](#non-natural-perils)
- [Non-modelled CATs](#non-modelled-cats)
- [Uses of CAT models](#uses-of-cat-models)
- [Problems with CAT models](#problems-with-cat-models)
- [Commercial CAT models](#commercial-cat-models)

## Why CAT models exist

- Low frequency, high severity:
  - observed losses don't reflect true underlying risks
  - time period observed shorter than return period of said losses
- Occur for naturally occurring hazards:
  - Hurricane, tornado, typhoon
  - Earthquake (with e.g. 250-year return period)
  - Flood
  - Hailstorm
  - Wildfire
  - Freeze
  - Disease
- Also for certain human-made events:
  - Nuclear disaster
  - Financial crash
  - Terrorism

## CAT model development

- Model development is iterative:
  - Hardware advancement
  - Geographical information systems software
  - Occurrence of events with detailed exposure and loss data
  - Scientific advances of understanding hazard
  - Physical measurement advancements
- Accuracy and level of detail of data available impacts reliability
- Examine historical events
- Research understanding of underlying causes of events (e.g. earthquake models use paleoseismology)

## CAT model overview

1. Create stochastic event set:

   - Examine historical events = past events,
   - From research of underlying causes = Set of possible future events

2. Calculate effect of events on insureds exposure
3. Apply terms of insurance contracts (deductibles, limits, peril sub-limits)
4. Apply reinsurance programme

## Structure of CAT models

Two types (depending on cost and time):

1. Aggregate models

   - Detailed exposurd risks not known
   - Use aggregate exposures (e.g. sums insured) in area
   - Use industry average losses
   - Works if actual risks ~= industry average

2. Detailed models

   - Individual insured risk information used
   - Likely loss for each insured risk calculated
   - Summed to get aggregate losses

Interlinked modules:

- Event module
- Hazard module
- Inventory module (`== exposure`) \[user input\]
- Vulunerability module
  - Secondary uncertainty option
- Financial analysis module \[user input\]
  - Secondary uncertainty option

### Event module

- Database of stochastic event set
  - Physical parameters
  - Location
  - Annual probability of occurrence (frequency)
  - Thousands of possible events (~ few hundred historical records)
  - Historical event set e.g. Hurricane Andrew - allows modelled exposure against insured portfolio

### Hazard module

- Hazard of each event at each location
- Consequence of event that causes damage:
  - Hurricane = wind speed
  - Earthquake = ground shaking

### Inventory module

- Exposure database of insured structures
- Age, occupancy, construction, number of storeys
- Irregulary building configuarations:
  - Hurricane models = Roof anchors
  - Earthquake models = Soft storeys

### Vulnerability module

- Degree of loss to structure resulting from exposure to given level of hazard (% of sum insured)
- Produces modelled loss ~ value of exposure insured (**not** actual insured limits)
- Models loss arising from business interruption arising from physical damage
- Known as **ground-up losses**

### Seconary uncertainty

- Reflects uncertainty surrounding exact impact of given event
- Uncertainty on exact **amount** of insured loss given event causes
- Complicates use of modelling results

### Financial analysis module

- Database of policy conditions to translate total ground-up loss into gross insured loss
  - Limits, excess, sub-limits, coverage terms
- Apply reinsurance programmes in place:
  - Inuring Fac, Risk XoL, Proportional cover applied first == _"net pre-cat"_
  - CAT XoL applied separately

### CAT modelled loss example

- Ground-up loss = `Vulnerability % * Structure Value`
- Gross loss = `Min[Ground-up loss - Deductible, Limit]`
- Net pre-cat loss = `Gross loss - RI recoveries (before CAT XoL)`

## Perils in CAT models

1. Windstorm, separately for:
   1. Tropcial cyclones (storms, hurricanes, typhoons)
   2. Extra-tropical cyclones (European windstorm)
   3. Tornadoes
2. Earthquake
3. Non-natural perils

### Tropical cyclones

**Physical details**

- Character: large low-pressure cetnre, numerous thunderstorms, strong winds, heavy rain
- Strength and location dictates naming:
  - Hurricanes = Northern hemisphere,
  - Typhoons = Southern hemisphere,
  - Tropcial storms / depressions = strength determined
- Classifications based on maximum sustained surface wind speed over set period (Saffir-Simpson = 1 minute, most others = 10 minutes)
- Facets of tropical cyclones:
  - Max sustained wind speed,
  - Track
  - Storm radius
  - Forward speed
  - Rate of decay of wind field (function: wind speed reduction, distance from storm centre)
  - Central pressure (lower = faster winds spiral around eye of storm)
- Annual frequency is **not** constant, varies by years / decades
- Minor climate effects significant impact on hurricane activity
- Two sets of event rates: `near-term` and `long-term`
  - `Near-term` (`= medium-term`) - conditioned on current climate observations (sea-surface temps)
  - `Long-term` (`= historical`) - unconditional estimate not affected by current climate
  - Two views = different results
  - Vendor recommendations, market practices, regulatory requirements influencce event rate set to use

**Models**

- Accuracy factors:

  - Frequency of different magnitudes
  - Quality of historical peril data
  - Quality & availability of current/historical exposure and claim data
  - Lenght of time data available
  - Existence of, level of adherence to, uniform building standards
  - Changes in demographics
  - Level of investment by model vendor
  - Model iteration

- Insured coverage modelled:

  - Damage to buildings
  - Damage to contents
  - Business interruption costs from damage to buildings/contents
  - Static inland marine risks (cargo, specie)
  - Watercarft (yachts)
  - Coastal fishing fleets
  - Auto physical damage
  - Offshore energy (rigs/platforms)
  - Livestock

- Limiations (not modelled):

  - Goods in transit (transient)
  - Ocean marine (transient)
  - Contingent business interruption

- Additional features:
  - Storm surge = rise in level of coastal water above usual tide level as cyclone moves over the water, potential flooding. Problematic coverage: 'wind' included but excludes flood (how much damage caused by hurricane vs. flood).
  - Demand surge = temporary increase in costs of materials, labour, temporary accomodation following a CAT. More severe & widespread => more significant this factor.
  - Loss amplification = demand surge + additional factors (coverage slippage = courts decide insured coverage broader than initially envisioned)

### Extra-tropical cyclones ("ETC")

- Character: area of low pressure at centre, most commonly seen in the UK & Europe, tendency for storms to cluster (not well modelled by static Poisson process)
- Not as seasonal / predicatable as US because weather characteristics form ~1-2 weeks ahead of European windstorms
- Frequency of major ETCs than cyclones => less data => less well modelled
- Modelling clustering => significant effect on results (especially on extreme tails of distribution)

### Tornadoes

- Character: rotating colum of air, in contact with ground, often visible as funnel cloud, erratic paths, last seconds - hours (usually a few minutes)
- Not as well defined a peril: one multiple-vortex tornado vs. separate tornadoes
- No long term forcasts
- Damage very localised (one side of street only)
- US tornado models available - less reliable than tropical cyclones, difficult to model the peril
- Factors affect output of model:
  - Only reliable tornado damage scale since 2007 (no retrospective reclassification) including a subjective elemenet of assessment
  - Doppler radio in 90s increased observed frequency
  - Treatment of multiple tornadoes spawned by same storm system
  - Lower level of investment by model vendors
  - Model iteration

### Earthquake ("EQ")

**Physical details**

- Character: sudden slip along fault due to build up of stress, accumualted energy released as seismic waves. Ground shaking, fault rupture, landslides, liquefaction, fire following EQ, tsunami, sprinkler leakage
- Losses:
  - Shaking => building damage, injury / loss of life
  - Fault rupture => permanent ground deformations
  - Landslides => destruction of buildings, loss of life
  - Liquefaction => sinking buildings / tipping over
  - Sprinkler leakage => contents damage / building damage
- Severity ~ amplitude, duration, frequency of ground motions
- Measured as `Moment magnitude` (Mw) = total energy of EQ
- Major EQs are rare, infrequent in populated areas => historic information derived from paleoseismic studies

**Models**

- Most significant in US and Japan (insured loss perspective)
- Factors affecting accuracy:
  - Quality, availability of historical event records and paleoseismic studies
  - Quality, availability of current/historical exposure and claim data
  - Quality, granularity of soil type data
  - Existence and adherence to building standards
  - Changes in demographics
  - Investment by model vendors
  - Model iteration
- Insured coverage modelling:
  - Damage to buildings, contents
  - Business interruption
  - Static inland marine risks
  - Workers' Compensation
  - Group life
  - Auto physical damage
- Limitations:
  - Transient inland marine not modelled
- Model parameters:
  - Moment magnitude
  - Focal depth
  - Total area of fault rupture
  - Fault type (convergent plate boundaries = highest hazard)
- Largest insured loss driver = Amount of ground motion (shake element of EQ peril)
- Attenuation (ground motion decay):
  - Greater decay => smaller area of damage
  - Varies by region, reflects geology (young/thin crust => quick attenuation)
- Event recurrence affected by time since last rupture on that fault and ruptures on other faults
- Frequency modelled as:
  - Staticial distribution (Poisson)
  - `Time Dependent` (predicatable) model - consider fault slip rate, time since last event
  - `Stress Transfer` (migration) model - occurence of EQ on one fault impacts occurence of EQ on nearby fault
- Additional features:
  - Sprinkler leakage
  - Fire following EQ
  - Demand surge
  - Results for WC and Group Life at peak / random times of day

### Non-natural perils

- Terrorism model constructured differently to natural CAT models
- Output used differently
- Model offer separate deterministic and stochastic modules
  - Deterministic module - asses portfolio's maximum expected loss from each of number of different types of terrorist attacks
  - Stochastic module - annual frequency for each of the types of attack considered within the model
- Very volatile nature of probability of attack => rely more on results of deterministic module
- Modelled types of attack:
  - Small scale: explosive devices carried by individual / vehicle bombs
  - Large scale: civilian aircraft hijack and crash
  - Extreme scale: weapons of mass destruction

## Non-modelled CATs

- CATs for an insurer who **has** exposures but does **not** have a model at region-peril
  - No model exists, chosen not to license / build own
  - Cost/benefit: exposure not material, business written is niche / not captured well
- Regions and perils not covered by CAT models - e.g. up to 2011 no Thai floods
- Seconary perils/effects not covered by CAT models - looting
- Classes and LoBs not covered by CAT models - personal accident, marine
- Coverages not covered by CAT models - complex offshore energy risks covers
- Identifying areas of non-modelled risks:
  - Top down initial approach to identify areas of material exposure in different regions, review perils covered there
  - Review existing models to identify gaps and consider if material
  - Review policy wording for ambiguities on potential losses
  - Review industry claims and own claims experience
  - Expert judgement - internal (UWers, CHers), external - CAT vendors, expert groups and risk engineers
- Quantifying non-modelled CAT risk:
  - CAT model modification - base expected losses on existing CAT model
  - Actuarial and statistical methods - requires loss data, use internal/exteranl data, make exposure/inflation/insurance penetration adjustments, fit distribution to frequency & severity of losses
  - Geospatial - requires risks mapped to defined geographic areas, apply factors to areas, complexity depends on extent of geospatial work
  - Expert judgement - particularly where no/little data
- [ABI's Non-modelled risks paper](https://www.abi.org.uk/globalassets/sitecore/files/documents/publications/public/2014/prudential-regulation/nonmodelled-risks-a-guide-to-more-complete-catastrophe-risk-assessment-for-reinsurers.pdf): _A guide to more complete catastrope risk assessment for (re)insurers_

## Uses of CAT models

- Use CAT models for:
  1.  Aggregate modelling - monitor aggregate insured loss
  2.  Pricing
  3.  Capital allocation
  4.  Purchasing RI
  5.  Reserving
  6.  Designing CAT bonds / ILS vehicles

**Aggregate modelling**

- Use CAT model to assess given peril (e.g. CA EQ), given portfolio (LoB, LE, book) the estimated loss from said peril at different return periods (1 in 10, 1 in 200)
- Set acceptable limits for such losses according to risk tolerance
  - 1 in 100 year loss from CA EQ should not exceed $50M => UWers manage book within these limits, regularly report adherence to these UWer guidelines, captured risk monitoring as part of ERM
  - Lloyd's Realistic Disaster Scenarios: syndicate required to report to managing agency board & Lloyd's on exposure to specified series of events (**not** perils). Lloyd's uses events to assess aggregate exposure across Lloyd's for Central Fund exposure. Note diversifcation (not simply adding each syndicate's 1 in 250 year event).
- Output from CAT models is a table:
  - **OEP** - Occurrence Exceedance Probabilities := Prob(loss forom single event) > given loss amount
  - **AEP** - Aggregate Exceedance Probabilities := Prob(annual aggregate loss) > given loss amount
  - **OEP** is **misleading** for high frequency perils and strong clustering perils

**Pricing**

**Capital**

**RI purchase**

**Reserving**

## Problems with CAT models

## Commercial CAT models

- AIR, RMS and CoreLogic
