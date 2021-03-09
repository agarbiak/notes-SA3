# Technical Provisions <!-- omit in toc -->

- [Overview](#overview)
- [Solvency II Directive](#solvency-ii-directive)
- [Best Estimate](#best-estimate)
  - [Claims Provision](#claims-provision)
  - [Premium Provision](#premium-provision)
  - [Contract boundaries](#contract-boundaries)
- [Reinsurance](#reinsurance)
- [Expenses](#expenses)
- [ENIDs](#enids)
- [Segmentation](#segmentation)
- [Risk Margin](#risk-margin)
- [Balance sheet presentation](#balance-sheet-presentation)
- [Validation](#validation)
- [Reporting](#reporting)
- [Communication](#communication)

## Overview

These notes are summarised version of [IFoA paper](https://www.actuaries.org.uk/system/files/documents/pdf/sii-tp-wp-paper-giro40.pdf)

- Value of technical provisions = best estimate + risk margin
  - Value best estimate and risk margin separately
- Best estimate := probability-weighted average of future cashflows taking account of the time value of money using the relevant risk-free interest rate term structure
  - Components: claims provision, premium provision
- Risk margin ensures technical provisions value is equivalent to amount that (re)insurance undertakings would be expected to require in order to take over and meet the (re)insurance obligations
  - Calculated as cost of providing an amount of eligible own funds equal to the Solvency Capital Requirement necessary to support the (re)insurance obligations over the lifetime thereof using the prescribed EIOPA cost of capital rate (6%)
- Claims and premium provisions should be valued separately
  - Calculated separately gross and for reinsurance
  - Key distinction is that the claims provision covers claim events occured at/before valuation date (future CFs relating to past exposure) vs. premium provision relates to CFs attributable to future exposure
- Calculated in accordance with the general provisions for the determination of technical provisions as set out in Articles 75 to 78 of the Level 1 text

## [Solvency II Directive](https://www.eiopa.europa.eu/rulebook-categories/directive-1382009ec-solvency-ii-directive_en)

- Article 76 - _General provisions_
  - > The value of technical provisions shall correspond to the current amount insurance and reinsurance undertakings would have to pay if they were to transfer their insurance and reinsurance obligations immediately to another insurance or reinsurance undertaking
- Article 77 - _Calculation of technical provisions_
  - > The value of technical provisions shall be equal to the sum of a best estimate and a risk margin
  - > The best estimate shall correspond to the probability-weighted average of future cash-flows, taking account of the time value of money, using the relevant risk-free interest rate term structure
  - > The calculation of the best estimate shall be based upon up-to-date and credible information and realistic assumptions and be performed using adequate, applicable and relevant actuarial and statistical methods
  - > The cash-flow projection used in the calculation of the best estimate shall take account of all the cash in- and out-flows required to settle the insurance and reinsurance obligations over the lifetime thereof
  - > The risk margin shall be such as to ensure that the value of the technical provisions is equivalent to the amount that insurance and reinsurance undertakings would be expected to require in order to take over and meet the insurance and reinsurance obligations
  - > The risk margin shall be calculated by determining the cost of providing an amount of eligible own funds equal to the Solvency Capital Requirement necessary to support the insurance and reinsurance obligations over the lifetime thereof
  - > The rate used in the determination of the cost of providing that amount of eligible own funds (Cost-of-Capital rate) shall be the same for all insurance and reinsurance undertakings and shall be reviewed periodically
- Article 78 - _Other elements to be taken into account in the calculation of technical provisions_
  - > In addition to Article 77, when calculating technical provisions, insurance and reinsurance undertakings shall take account of the following:
    - > all expenses that will be incurred in servicing insurance and reinsurance obligations
    - > inflation, including expenses and claims inflation
    - > all payments to policy holders and beneficiaries, including future discretionary bonuses, which insurance and reinsurance undertakings expect to make, whether or not those payments are contractually guaranteed, unless those payments fall under Article 91(2)
- Article 79 - _Valuation of financial guarantees and contractual options included in insurance and reinsurance contracts_
  - > When calculating technical provisions, insurance and reinsurance undertakings shall take account of the value of financial guarantees and any contractual options included in insurance and reinsurance policies
  - > Any assumptions made by insurance and reinsurance undertakings with respect to the likelihood that policy holders will exercise contractual options, including lapses and surrenders, shall be realistic and based on current and credible information. The assumptions shall take account, either explicitly or implicitly, of the impact that future changes in financial and non-financial conditions may have on the exercise of those options
- Article 80 - _Segmentation_
  - > Insurance and reinsurance undertakings shall segment their insurance and reinsurance obligations into homogeneous risk groups, and as a minimum by lines of business, when calculating their technical provisions
- Article 81 - _Recoverables from reinsurance contracts and special purpose vehicles_
  - > The calculation by insurance and reinsurance undertakings of amounts recoverable from reinsurance contracts and special purpose vehicles shall comply with Articles 76 to 80
  - > When calculating amounts recoverable from reinsurance contracts and special purpose vehicles, insurance and reinsurance undertakings shall take account of the time difference between recoveries and direct payments
  - > The result from that calculation shall be adjusted to take account of expected losses due to default of the counterparty. That adjustment shall be based on an assessment of the probability of default of the counterparty and the average loss resulting there from (loss-given-default)

## Best Estimate

- Cashflows should comprise:
  - all future claims payments and claims management expenses (both allocated and unallocated) arising from claims events that have occurred and future claim events
  - arising from ongoing adminstration of the in-force policies
  - expected future premiums stemming from existing policies
- Where claim events give rise to annuity payments, value of the technical provision should be separately calculated using appropriate life actuarial techniques
- Should allow fro time value of money by discounting at the EIOPA provided discount rates (EIOPA provides rates by major currency)
- Loss payment profile assumption less material as yields have been very low recently
  - Conversion from underwriting year cohorts to accident period via a transform, a simple lag may suffice provided simplification does not have a material impact
- Future premiums receivable should only include future premiums which are not overdue (accounted for separately on the SII balance sheet)
  - Easily confused between Finance and Actuarial => risk of double count or omission
  - Should be net of expected premium defaults

### Claims Provision

- Claims provision := Expected present value of future incoming and outgoing cashflows arising from **_claim events occuring before or at the valuation date_** including associated future premiums relating to these claims
- Calculation of undiscounted element similar to undiscounted claims reserves already estimated by (re)insurers on regular basis to fulfil existing regulatory requirements
  - Key changes: removal of any implicit/explicit margins for prudence and ENIDs
- Assumptions and methods must be chosen on a best estimate basis
  - Example: allowance for negative IBNR where expected future profit will emerge from existing case reserves
- PVs of CFs calculated by applying payment pattern to undiscounted reserves to generate future CFs which are then discounted (prescribed EIOPA rates for specific currencies) and summed

### Premium Provision

- Premium provision := Expected present value of future incoming and outgoing cashflows arising from the **_unexpired portion of business_** that the (re)insurer is obligated to at the valuation date
- Can be negative if EPV of cash inflows > cash outflows
  - Valued on a best estimate basis => takes account of expected profit to be recognised in the future
- Should include all future cashflows associated with contracts deemed to be existing at the valuation date determined on a legal obligation basis
- Future policyholder behaviour should be allowed for
  - Example: likelihood of policy lapse
  - Ignored on grounds of proportionality if future premium receivables are low (e.g. with annual premium policies)
  - Lapses likely material on personal lines where instalment premiums
- Often calculated using a loss ratio approach:
  - Apply loss ratio to unearned premium := total undiscounted claims
  - Apply payment pattern to generate future CFs => discount and sum to generate PV of FCFs
  - Derived from unexpired risk reserve (`URR`) is correct approach
  - Practice: not carried out unless expect premiums insufficient for a CoB
  - Alternative, readily available approaches: pricing loss ratios, plan loss ratios, burning cost method <= care needed to ensure appropriate

**Suitability of loss ratio approaches**

- Pricing loss ratios
  - Based on estimates of likely future experience, likely suitable for premium provision loss ratios
  - Exposure period for pricing loss ratios may differ to exposure period covered by premium provision
  - Annual uniformly written contracts over calendar year => premium provision exposure weighted towards first few months
  - Pricing loss ratios likely assume longer exposure period, if significant trend in claim costs => overstate trends for premium provision
- Plan loss ratios
  - Suitable if estimated on best estimate basis and either cover same exposure period or claim cost trends over time insignificant
  - Not suitable if plan loss ratios are out-of-date
    - Example: recent experience significantly different than expected
    - Example: type of business written different to what was expected when plan constructed
  - Not suitable if plan conservative / incorporates stretch assumptions
  - Not suitable if plan loss ratios do not represent reserving actuary's best estimate
    - Example: Lloyd's syndicates SBF process may upwards adjust plan loss ratios from Lloyd's review
- URR loss ratios
  - Typically start with recent loss experience analysis, projecting ultimate losses for recent accident years from the claims provision
  - Adjustments from historic experience to future unearned premium exposure period:
    - Exposure
    - Rating environment
    - Legal environment
    - Policyholder behaviour
    - Business mix
    - Inflation and other trends
    - Seasonality
    - Reporting and settlement delays / terms to payment
    - Lapse rates
    - Reinsurance coverage
    - Investment return (future risk-free rates of return)
    - Unusual / exceptional events
    - Coverage and policy wording
    - Socio-economic trends
  - URR loss ratios often updated less frequently than TPs => care needed to ensure still applicable
- Burning cost method
  - Project burning costs based on suitable exposure measure (e.g. policy count)
  - Multiple burning costs by exposure projection
  - Advantage: considers claim cost independently of premium charged and rating actions (do not always have proportional impact on claims costs)
  - Requires additional considerations:
    - Allowance for business mix - alter average cost per policy to reflect change in profile of policies written
    - Allowance for claim cost inflation (premium inflation lost when using burning costs)
    - Seasonality incorporated if claim costs influenced by time of year
    - Exposure measures need to be consistent with business volumes underlying the UPR figure

### Contract boundaries

- Determined on a legal obligations basis
  - All existing contracts must be valued whether contracts have incepted or not
- Distinctions:
  - Business incepted at valuation date:
    - Earned incepted business := gross claims cashflows within claims provisions
    - Unearned incepted business := gross claims cashflows within premiums provision
    - Incepted business := gross future premium receivable
  - Business not incepted at valuation date:
    - Unincepted business:= Gross future premium and claims cashflows for policies not yet incepted by valuation date but forming part of contractual obligations => part of premium provision
    - Generally include 1-1 renewals for a 31 December valuation
- In principle made on a per contract basis unless inpractical => higher level of granuality applied if immaterial difference to a per contract assessment
- Contract should be recognised as existing when the (re)insurer becomes party of the contract
- Contract derecognised as existing contract when obligation specified in contract discharged or expires
- Boundaries defined as follows:
  - Where insurer has unilateral right to cancel the contract, reject the premium or ability to amend premium / benefits to reflect underlying risk / re-underwrite risk at some point in future => premiums received beyond that point do not belong to existing contract
    - If such rights relate only to part of contract => this part only excluded from existing contract
  - Any future premiums (resulting CFs) which relate to options/guarantees that provide rights under which policyholder can renew the contract, extend the insurance coverage to another person, extend the insurance period, increase the insurance coverage / establish new insurance cover => belong ton existing contracts
  - All other cashflows relating to contract should be included in best estimate: future premiums (any resulting cash outflows) should be included if their payment by policyholder is legally enforceable
- Premium provision needs to include cashflows relating to policies with commencement date falling after valuation date due to:
  - Tacit renewals
  - Business written under a binding / delegated authority
  - Other policies written with a future commencement date

**Binding authorities / Delegated authorities**

- Binding authority == Delegated authority == binder == partnership agreement
- Binder := (re)insurer agrees to underwrite future busienss introduced by a third party under specified conditions
- Need to use a _look through_ approach with boundaires of actual underlying insurance contracts being tested
  - Can include estimations if data not immediately available

## Reinsurance

- Significant changes to the calculation of gross liabilities will apply equally to the calculation of reinsurance recoveries, challenges include:
  - consideration of reinsurance recoveries on a cash flow basis
  - consideration of how the requirement to allow for _all possible future outcomes_ may impact reinsurance valuation
- Further challenges when applied to reinsurance, due to lack of data or additional complexity including:
  - requiring consideration of the timing of defaults or disputes
  - the assessment of contract boundaries and what reinsurance contracts are treated as "_existing_" in determining which premiums and recoveries are to be included
- Need to also allow for expected non-payment due to default or dispute
- Range of possible simplifications that may be used for reinsurance, though these may only be used where appropriate and where they do not materially misestimate underlying values
- Contract boundaries:
  - **Principle of correspondence** should underlie the calculation of reinsurance recoveries in the best estimate when considering which contracts to include
    - Correspondence between the gross inwards claims and the reinsurance recoveries included within the valuation
  - Future reinsurance cover to be bought that will cover existing inwards contracts (e.g. Losses Occurring During (`LOD`) cover incepting 1st April for a year-end valuation) => By applying "_correspondence_", these contracts would be included as a future management action (assuming sufficient justification) and the expected proportion of the premium that applies to the existing inwards contracts would be included
  - On a best estimate basis, the reinsurers would aim to make a profit and so premium outgo would be expected to exceed recoveries. By adopting this approach technical provisions would increase as, in general, (re)insurers would not anticipate making money from buying reinsurance on a best estimate basis, unless there is very strong evidence to support this
  - Existing reinsurance contracts that will provide recoveries from inwards contracts that are NOT “_existing_” at the valuation date (e.g. Risks Attaching During (`RAD`) cover already purchased for the forthcoming year) => By applying correspondence only the expected recoveries on existing inwards contractswould be included Any future premium should be apportioned to only include the expected cost relating to existing inwards contracts
- Allowance for counterparty default:
  - Adjustment should approximate the expected present value of the losses whether due to insolvency, dispute or any other reason
  - Assessment for counterparty default must be made on a cashflow basis, taking into account the timing of defaults
  - The determination of the adjustment should take account of default events during the whole run-off period of the recoverables
  - The adjustment for default must take into account the risk that counterparties survive some years and default at some other point in the whole run-off period of the recoverables
    - In particular it is not sufficient to multiply the expected loss due to immediate default by the probability of default over the current year
  - The counterparty default adjustment should be calculated separately at least for each line of business, counterparty and separately for premium provisions and claims provisions
  - Where the probability of default and recovery rate of several counterparties coincide, and if calculations at the level of individual counterparty are an undue burden, then the adjustment for these counterparties could be calculated together
  - Where the (re)insurer has an internal model, the reserving specialist will need to ensure that the approach used for counterparty default risk is consistent with that used in the internal model
  - (Simplified) adjustment for counterparty default = `-max{(1 - RR) * BE_rec * Dur_mod * (PD / 1 - PD), 0}`, where:
    - `RR` := recovery rate of the counterparty
    - `BE_rec` := best estimate of recoverables before the expected loss due to default of the counterparty
    - `Dur_mod` := modified duration of the recoverables
    - `PD` := probability of default of the counterparty for the time horizon of one year

**Gross to net simplification**

- The calculation of best estimate recoverables can be performed either directly as the probability weighted average of future recoverable cash flows or indirectly as the difference between the gross and net best estimates
- Solvency II requirements state that the indirect method should only be used if it is expected to produce a result corresponding to the direct method
- One example of this indirect approach is the use of gross to net techniques
- The overarching requirement is that reinsurance recoverables calculated in this indirect manner are consistent with Article 81 of the Framework Directive (particularly in the allowance for timing differences and an adjustment for counterparty default risk)
- Simplifications may not be acceptable in cases:
  - Exposure analyses – direct/explicit reinsurance calculations are often available
  - Complex outwards reinsurance programmes – where simple or implicit methods would often be unsuitable
  - When consistency with gross calculation is required – e.g. if an average cost per claims method is employed (for a frequency severity model, explicit modelling of reinsurance would be preferable)
  - Where allowing for cover limits or exhaustion is required as simplification may not implicitly capture the risk appropriately

## Expenses

- Under Solvency II, the best estimate provisions should reflect all future cash flows arising from expenses that will be incurred servicing existing policies during their lifetime
- All future expenses that will be incurred in servicing existing
  insurance and reinsurance obligations should be taken into account, including:
  - Administrative expenses
    - Salaries
    - Property costs (including rent, depreciation, heating, lighting, cleaning)
    - IT costs
    - Expenses in relation to the management (actuarial, finance, risk, commercial, data) or administration of reinsurance contracts / SPVs
  - Other administrative expenses
  - Investment management expenses
  - Claims management expenses (including claims handling expenses)
  - Acquisition expenses (including commissions)
  - Costs associated with arranging and managing outwards reinsurance
  - Insurance premium tax
- Expense assumptions should include allowance for future cost increases
  - In particular, assumptions about future inflation should be made, which need to be consistent with the assumptions made elsewhere in the calculation of technical provisions and in the internal model, if there is one
  - The inflation rate used should be appropriate to the driver of the expense
- Assumptions about cash flows should consider future changes in the environment (such as legal, demographic, medical, technological, social or economic)
- Future expense cash flows should be expressed in the currency in which they are likely to occur and discounted at the appropriate EIOPA provided discount rate for that currency

**Claims expenses**

- ALAE are typically included in the claims data and therefore implicitly projected as part of the claims projection i.e. assuming the same payment pattern
- Adjustments may be required however, if the allocated costs are changing as a percentage of reported or paid losses, or if the timing of expenses is expected to be significantly different than that of claims
- For the premium provision, they are likely to be allowed for in the loss ratio assumption
- It is unlikely that any data will be available to discern a future payment pattern for ULAE though it seems reasonable to assume these will run-off in line with losses
- A common approach to estimate unallocated claims management costs is to look at historic paid unallocated claims management costs and relate them to paid losses over the same period. Typically adjustments are made to allow for the uneven incidence of expense over the life cycle of the claim, for example by allowing for different costs on opening and closing. Such an analysis tends to result in a percentage uplift that is applied to total outstanding losses

**Acquisition expenses**

- Required for premium provision calculation
- Need to allow for business that has been accepted prior to the valuation date for which cover has not yet commenced and the acquisition costs may not yet have been paid
- Commission is likely to be a large part of acquisition expenses and current commission rates should be reflected in the assumption

**Profit commission**

- May need to allow for profit commission in both the premium and claims provision
- Profit commission more complicated to calculate than acquisition costs because it is based on claims experience
- Some profit commission payments may be known, or estimated with reasonable certainty and the date upon which they are due may be fixed at some point in the future e.g. a contract anniversary
- Others may be quite complicated to estimate accurately due to a complex relationship with future claims experience - consider simplifying methods and/or assumptions on the grounds of proportionality

**Admin expenses / overheads**

- The best estimate needs to allow for all expenses that will be incurred including future administration costs and overheads
- If budgeted expenses are available, and are best estimate, these may be suitable to be used to derive loadings to cover administration and overheads
- Adjustments:
  - Level to best estimate basis
  - Allow for anticipated efficiency improvements
  - Exclude one-off costs (e.g. implementation of new systems/processes)
  - Allow for cost inflation
  - Cover exposure period considering vs. what period budgeted expenses apply 

**Investment expenses**

- Investment expenses cannot be allowed for by reducing the discount rate
- Investment expenses could be allocated based on the level of funds under management; they could be split into Solvency II classes using (net) best estimate provisions

**Reinsurance costs**

- The costs associated with purchasing and managing reinsurance should be allowed for in the gross claims and premium provisions
- As the technical provisions are calculated on a cashflow basis, one would generally allow for expenses as and when the cash flows occur
- However, applying the _principle of correspondence_ one may have to adjust expense cash flows associated with reinsurance so that only those relating to reinsurance cover corresponding to the inwards risks that the (re)insurer is obligated to at the valuation date are taken into account

## ENIDs

## Segmentation

## Risk Margin

## Balance sheet presentation

## Validation

## Reporting

## Communication
