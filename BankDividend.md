# BankDividend
**Don't Let Your Cash Sit There.**
- HTML Mirror:  [https://roxanneardary.com/bankdividend-specification/](https://roxanneardary.com/bankdividend-specification/)  

---

BankDividend is an open source AI specification for discovering, retrieving, verifying, calculating, scoring, ranking, and explaining checking, savings, money market, certificate, and credit union account options based on user-defined criteria.

The specification is designed around a consumer-first principle: **maximize the user's net financial benefit from banking while minimizing fees, unnecessary requirements, and avoidable risk.** BankDividend does not simply rank accounts by advertised APY. It evaluates the actual economic value of an account based on the user's deposit balance, spending behavior, eligibility, account requirements, fees, rewards, insurance status, and other relevant conditions.

BankDividend is modular by design. Implementations can use the complete specification or deploy individual modules for account discovery, insurance verification, earnings calculations, fee analysis, behavioral simulation, ranking, or explanation. Optional plugin modules can extend the specification without requiring changes to the core system.

## Specification Goals

BankDividend is designed to:

- Find banking products that match user-defined criteria.
- Compare checking, savings, money market, certificate, and credit union accounts.
- Prioritize federally insured institutions by default.
- Verify FDIC insurance for eligible banks and savings institutions.
- Verify NCUA federal share insurance for federally insured credit unions.
- Display prominent red flags when federal insurance cannot be verified.
- Calculate expected interest and dividend earnings.
- Calculate cashback and other financial incentives.
- Calculate account-opening bonuses and promotional benefits.
- Identify monthly, annual, transaction, ATM, overdraft, and other fees.
- Identify minimum balance and activity requirements.
- Identify direct deposit requirements.
- Identify geographic, membership, employment, and eligibility restrictions.
- Calculate estimated net financial benefit.
- Simulate account performance based on user behavior.
- Recommend publicly traded and privately owned institutions without ownership-based preference.
- Explain why products receive their rankings.
- Distinguish verified information from estimates and promotional claims.
- Track the source and date of financial product information.
- Detect conditions that can reduce an advertised yield.
- Allow users to define safety, yield, fee, reward, and eligibility priorities.
- Help users identify opportunities where their cash can earn more rather than remaining idle.

---

## Core Principles

### Get Paid to Bank

BankDividend is built around the principle that consumers should seek banking products that provide measurable financial benefits rather than unnecessarily charging them for maintaining and using an account.

The system should prioritize products where:

**Interest + Dividends + Cashback + Bonuses + Rewards > Fees + Costs + Applicable Penalties**

The resulting calculation should represent the estimated net financial benefit available to the user.

### Federally Insured First

Federally insured deposit and share accounts are the default preference.

For banks and eligible savings institutions, BankDividend should verify FDIC deposit insurance.

For credit unions, BankDividend should independently verify federal share insurance through the NCUA and the National Credit Union Share Insurance Fund.

Being identified as a bank or credit union does not by itself establish federal insurance eligibility.

### Insurance Red Flags

When an institution or financial product does not have verified federal insurance, the implementation must make the absence or uncertainty prominent.

The result should display a bold red flag such as:

**RED FLAG: NO VERIFIED FEDERAL DEPOSIT OR SHARE INSURANCE**

The system should also flag situations where:

- Insurance status cannot be verified.
- An institution claims insurance that cannot be independently confirmed.
- The specific financial product is not an insured deposit or share product.
- Funds are placed into an uninsured investment product.
- Coverage depends on conditions that are not satisfied.
- The user's balance may exceed applicable insurance limits.
- The account structure creates potential coverage limitations.

An uninsured product must not automatically outrank a federally insured product solely because it advertises a higher yield.

### User-Centered Ranking

BankDividend ranks products according to the user's circumstances rather than allowing advertised rates to determine the result by themselves.

A high APY may not produce the highest actual return if the account requires:

- A large minimum balance.
- Direct deposit.
- Frequent debit transactions.
- Subscription fees.
- Membership fees.
- Restricted eligibility.
- A balance threshold.
- Limited promotional eligibility.
- Other conditions that reduce the user's actual benefit.

---

## Core Modules

### User Profile Module

The User Profile Module defines the financial criteria used to evaluate available products.

Supported criteria can include:

- Desired account type.
- Deposit amount.
- Average account balance.
- Minimum account balance.
- Monthly deposits.
- Direct deposit availability.
- Monthly debit spending.
- Expected debit transaction count.
- ATM usage.
- Expected withdrawals.
- Expected transfers.
- Geographic eligibility.
- Credit union membership eligibility.
- Employer or organizational eligibility.
- Preference for online or physical institutions.
- Preference for publicly traded institutions.
- Preference for privately owned institutions.
- Preference for credit unions.
- Required federal insurance.
- Maximum acceptable fees.
- Desired APY.
- Desired cashback.
- Desired bonuses.
- Risk preferences.
- Account access requirements.
- Banking features required by the user.

### Institution Discovery Module

The Institution Discovery Module identifies financial institutions offering eligible deposit products.

Supported institution types can include:

- Commercial banks.
- Community banks.
- Online banks.
- Savings institutions.
- Credit unions.
- Community financial institutions.
- Privately owned institutions.
- Publicly traded institutions.
- Other eligible deposit-taking institutions.

Institution ownership should be treated as descriptive metadata rather than an automatic ranking factor.

The module should identify:

- Institution name.
- Institution type.
- Ownership structure.
- Parent organization.
- Public trading status where applicable.
- Geographic footprint.
- Membership requirements.
- Federal insurance status.
- Available products.
- Product eligibility.

### Product Discovery Module

The Product Discovery Module retrieves available financial products and identifies the terms applicable to each product.

Supported products include:

- Checking accounts.
- High-yield checking accounts.
- Savings accounts.
- High-yield savings accounts.
- Money market deposit accounts.
- Certificates of deposit.
- Share certificates.
- Rewards checking.
- Cashback checking.
- Dividend-bearing accounts.
- Other eligible deposit or share products.

### Product Normalization Module

The Product Normalization Module converts account information from different institutions into a consistent structure so products can be compared.

Normalized fields can include:

- APY.
- Interest rate.
- Dividend rate.
- Balance tiers.
- Balance limits.
- Compounding frequency.
- Minimum opening deposit.
- Minimum balance.
- Monthly fees.
- Annual fees.
- Transaction fees.
- ATM fees.
- Overdraft fees.
- Direct deposit requirements.
- Debit transaction requirements.
- Cashback rates.
- Cashback limits.
- Promotional bonuses.
- Promotional periods.
- Membership requirements.
- Eligibility restrictions.
- Insurance status.
- Insurance limits.
- Account access methods.
- Account expiration or conversion terms.

### Insurance Verification Module

The Insurance Verification Module determines whether an institution and specific product have verified federal insurance.

The module should distinguish between:

- FDIC deposit insurance.
- NCUA federal share insurance.
- Private insurance.
- Other forms of protection.
- No verified insurance.
- Unknown or unverifiable insurance status.

The module should verify the insurance status independently from marketing descriptions whenever possible.

Insurance verification should include:

- Insurance provider.
- Institution identification.
- Product eligibility.
- Coverage category.
- Applicable coverage limits.
- Verification source.
- Verification date.
- Verification status.

### Eligibility Module

The Eligibility Module determines whether the user can actually open and maintain the account.

It should evaluate:

- Geographic restrictions.
- State restrictions.
- Membership requirements.
- Employer requirements.
- Association requirements.
- Age requirements.
- Minimum opening deposit.
- Direct deposit requirements.
- Credit union membership eligibility.
- New customer restrictions.
- Promotional eligibility.
- Other institution-specific requirements.

Products that the user cannot access should not be presented as directly available recommendations.

### Fee Analysis Module

The Fee Analysis Module identifies the actual costs associated with an account.

It should evaluate:

- Monthly maintenance fees.
- Annual account fees.
- Minimum balance fees.
- ATM fees.
- Out-of-network ATM fees.
- Overdraft fees.
- Returned payment fees.
- Excess transaction fees.
- Wire fees.
- Foreign transaction fees.
- Transfer fees.
- Paper statement fees.
- Account closure fees.
- Early withdrawal penalties.
- Membership fees.
- Required subscription costs.
- Other recurring or conditional fees.

The module should determine whether a fee can be avoided and whether the user is likely to incur it based on their profile.

### Earnings Calculation Module

The Earnings Calculation Module calculates expected financial returns.

It should support:

- Simple interest calculations.
- Compound interest calculations.
- APY-based calculations.
- Dividend calculations.
- Tiered interest rates.
- Balance-based rates.
- Promotional rates.
- Rate expiration.
- Partial-year calculations.
- Variable balances.
- Recurring deposits.
- Recurring withdrawals.
- Daily or periodic compounding where applicable.

The module should produce estimated earnings for configurable periods including:

- Monthly.
- Quarterly.
- Semiannual.
- Annual.
- Multi-year.

### Cashback and Rewards Module

The Cashback and Rewards Module evaluates non-interest financial benefits.

It should calculate:

- Debit card cashback.
- Cashback limits.
- Cashback eligibility.
- Transaction requirements.
- Account bonuses.
- Direct deposit bonuses.
- Relationship bonuses.
- Promotional rewards.
- ATM reimbursements.
- Other measurable account incentives.

Cashback calculations should account for exclusions and spending limits.

### Net Benefit Module

The Net Benefit Module combines earnings and costs into a single user-centered calculation.

The core calculation should evaluate:

**Net Financial Benefit = Interest + Dividends + Cashback + Bonuses + Rewards - Fees - Penalties - Other Applicable Costs**

The implementation should distinguish between guaranteed, conditional, promotional, estimated, and behavioral benefits.

### Behavioral Simulation Module

The Behavioral Simulation Module determines how an account is expected to perform under the user's actual financial behavior.

It can simulate:

- Average balance.
- Monthly deposits.
- Direct deposits.
- Debit purchases.
- ATM withdrawals.
- Transfers.
- Balance fluctuations.
- Qualification requirements.
- Cashback limits.
- APY tiers.
- Promotional periods.
- Minimum balance requirements.

This module allows BankDividend to answer:

**"What will this account actually earn for me?"**

rather than simply reporting the advertised APY.

### Yield Reality Module

The Yield Reality Module compares advertised rates with the user's expected effective return.

It should identify situations where:

- The advertised rate applies only to a limited balance.
- A promotional APY expires.
- A higher rate requires additional activity.
- A user does not meet the qualification requirements.
- Cashback is capped.
- Fees offset interest earnings.
- A minimum balance is required.
- Different portions of a balance receive different rates.

The module should clearly explain the difference between advertised and projected returns.

### Red Flag Module

The Red Flag Module identifies material conditions that could negatively affect the user.

Potential red flags include:

- No verified federal insurance.
- Unclear insurance status.
- Uninsured products.
- High or avoidable fees.
- Promotional rates.
- Significant minimum balances.
- Restrictive eligibility requirements.
- High transaction requirements.
- Cashback exclusions.
- Balance caps.
- Limited promotional periods.
- Early withdrawal penalties.
- Other material conditions.

Critical warnings should be prominently displayed and should not be buried beneath ordinary account features.

### Ranking Module

The Ranking Module scores and ranks products according to user-defined criteria.

Ranking factors can include:

- Estimated net annual benefit.
- APY.
- Dividend rate.
- Interest earnings.
- Cashback.
- Bonuses.
- Fees.
- Minimum balance.
- Qualification requirements.
- Insurance status.
- Eligibility.
- Account accessibility.
- User preferences.
- Risk constraints.

Users should be able to change the weighting of ranking factors.

A user may prioritize:

- Maximum earnings.
- Zero fees.
- Maximum cashback.
- Maximum APY.
- Federal insurance.
- No minimum balance.
- No direct deposit requirement.
- Credit unions.
- Publicly traded institutions.
- Privately owned institutions.
- Simplicity.
- Accessibility.

### Recommendation Module

The Recommendation Module converts ranking results into understandable recommendations.

Recommendations should include:

- Institution.
- Product.
- Account type.
- Advertised APY or dividend rate.
- User-specific projected earnings.
- Projected cashback.
- Projected bonuses.
- Estimated fees.
- Estimated net benefit.
- Federal insurance status.
- Eligibility requirements.
- Material restrictions.
- Red flags.
- Reason for recommendation.
- Source information.
- Information verification date.

The system should explain why the recommended product ranked above alternatives.

### Explanation Module

The Explanation Module converts calculations and rankings into plain-language explanations.

It should answer:

- Why was this account recommended?
- How much could the user earn?
- What fees could reduce earnings?
- What requirements must be met?
- Is the account federally insured?
- What happens if the user does not meet the requirements?
- How does this product compare with alternatives?
- Why did a lower APY account rank higher?
- Why was an uninsured product excluded or downgraded?

### Source Verification Module

The Source Verification Module records the origin of financial product information.

Relevant data should include:

- Source.
- Source type.
- Product page.
- Terms and conditions.
- Insurance verification source.
- Retrieval date.
- Last verification date.
- Data freshness.
- Verification status.

The implementation should favor authoritative institutional, regulatory, and official product sources when available.

### Change Monitoring Module

The Change Monitoring Module detects changes to financial products.

It should monitor changes to:

- APY.
- Dividend rates.
- Fees.
- Eligibility.
- Direct deposit requirements.
- Debit transaction requirements.
- Cashback.
- Bonuses.
- Balance limits.
- Promotional periods.
- Insurance status.
- Account availability.

When a material change occurs, previously generated recommendations should be eligible for recalculation.

---

## Optional Plugin Modules

BankDividend supports optional modules that extend the core specification without requiring every implementation to include them.

### Credit Card Rewards Plugin

Evaluates credit card rewards alongside deposit account benefits.

Capabilities can include:

- Cashback.
- Points.
- Miles.
- Annual fees.
- Introductory offers.
- Spending requirements.
- Effective rewards rate.

### Investment Yield Plugin

Compares deposit products with eligible investment or treasury alternatives while clearly distinguishing insured deposits from investment products.

The plugin should never represent an investment as an FDIC or NCUA-insured deposit.

### Tax Impact Plugin

Estimates the potential tax impact of interest, dividends, bonuses, and other taxable account benefits.

Tax calculations should be presented as estimates and should not replace professional tax advice.

### ATM Network Plugin

Evaluates ATM availability, out-of-network fees, ATM reimbursement programs, and geographic accessibility.

### Direct Deposit Optimization Plugin

Evaluates direct deposit requirements and determines whether a user's existing income or recurring deposits can satisfy account qualification requirements.

### Promotional Offer Plugin

Tracks promotional bonuses, introductory rates, expiration dates, eligibility restrictions, and new-customer requirements.

### Banking Relationship Plugin

Evaluates whether combining products at one institution produces additional benefits.

Examples include:

- Relationship APY bonuses.
- Fee waivers.
- Cashback increases.
- Account bundles.
- Preferred customer benefits.

### Credit Union Eligibility Plugin

Identifies credit unions for which a user may qualify through geographic, employment, organizational, family, or other membership criteria.

### Geographic Banking Plugin

Evaluates local banking access, branch availability, ATM networks, regional eligibility, and location-specific products.

### Public Company Plugin

Identifies publicly traded financial institutions and can provide relevant ownership and public-market information without allowing public ownership status to independently improve a banking product's ranking.

### Private Institution Plugin

Identifies privately owned, mutual, cooperative, community-owned, and other non-public financial institutions.

### Financial Goal Plugin

Optimizes recommendations for user-defined goals such as:

- Emergency savings.
- Short-term savings.
- Long-term savings.
- Cash reserves.
- Regular spending.
- Large purchases.
- Retirement cash reserves.
- Tax reserves.

### Notification Plugin

Provides alerts when a recommended account's:

- APY changes.
- Fees change.
- Promotional period expires.
- Cashback changes.
- Insurance status changes.
- Eligibility changes.
- Ranking changes materially.

### Affiliate Disclosure Plugin

Allows implementations that receive referral or affiliate compensation to disclose compensation relationships.

Compensation must not modify the underlying financial ranking unless the user explicitly requests compensation-based filtering.

### Audit Plugin

Creates an auditable record of:

- Source data.
- Calculations.
- Ranking factors.
- Insurance verification.
- Product changes.
- Recommendation decisions.

## Scoring Framework

BankDividend should support transparent scoring rather than relying exclusively on a proprietary or unexplained ranking.

A scoring implementation may consider:

- Net financial benefit.
- Insurance status.
- Fees.
- Yield.
- Cashback.
- Bonuses.
- Requirements.
- Eligibility.
- Account accessibility.
- User preferences.
- Data confidence.

The system should expose the major factors that materially affected a score.

A recommendation should never claim that a product is universally the "best" account. It should be presented as the best match **for the user's specified criteria and circumstances**.

## Zero-Fee Mode

BankDividend should provide an optional zero-fee mode.

When enabled, the system should prioritize products that have:

- No monthly maintenance fee.
- No annual account fee.
- No required paid subscription.
- No unavoidable minimum balance fee.
- No unavoidable transaction fee.
- No required paid membership beyond legitimate eligibility requirements.

Avoidable fees should be identified separately from unavoidable fees.

The system should allow the user to determine whether "no fees" means:

- No recurring account fees.
- No fees under expected behavior.
- No fees under any possible account use.
- No fees including optional services.

## Maximum Earnings Mode

BankDividend should provide a maximum earnings mode that attempts to maximize the user's projected net financial benefit while respecting the user's required safety and eligibility constraints.

The system should consider:

- Interest.
- Dividends.
- Cashback.
- Bonuses.
- Rewards.
- Fee avoidance.
- Balance optimization.
- Qualification requirements.
- Promotional expiration.
- User behavior.

Maximum earnings mode must not silently remove required insurance or safety constraints.

## Safety-First Mode

Safety-First Mode should prioritize verified federal insurance and account protection before optimizing returns.

The implementation should:

- Prefer FDIC-insured deposit products.
- Prefer federally insured NCUA credit union share products.
- Flag uninsured products.
- Flag unverifiable insurance.
- Identify potential coverage limits.
- Distinguish deposits from investments.
- Explain material protection differences.

## Comparison Engine

BankDividend should allow users to compare multiple products simultaneously.

Comparison results can include:

- Institution.
- Ownership.
- Account type.
- APY.
- Projected earnings.
- Cashback.
- Bonuses.
- Fees.
- Requirements.
- Minimum balance.
- Insurance.
- Eligibility.
- Projected net benefit.
- Red flags.

The comparison engine should make differences in account conditions visible rather than presenting rates without context.

## Explainable Recommendations

Every recommendation should provide an explanation of the major reasons for its ranking.

A recommendation can state:

- The projected annual earnings.
- The estimated annual fees.
- The estimated cashback.
- The estimated net benefit.
- The requirements that must be satisfied.
- The applicable federal insurance.
- The reason it beats competing products.
- Important limitations or conditions.

The explanation should distinguish verified facts from calculated estimates.

## Data Freshness

Banking products change frequently. Implementations should treat product information as time-sensitive.

Each material data point should have:

- A source.
- A retrieval date.
- A verification status.
- An appropriate freshness indicator.

Stale information should be identified rather than silently presented as current.

## Financial Calculations

Calculations should be transparent and reproducible.

The implementation should preserve:

- Input values.
- Assumptions.
- Rates.
- Balance values.
- Time periods.
- Fees.
- Rewards.
- Qualification requirements.
- Calculation methodology.

Users should be able to understand how projected earnings were produced.

## User Control

BankDividend should allow users to define their own priorities.

Users should be able to specify:

- Required federal insurance.
- Maximum acceptable fees.
- Minimum desired APY.
- Minimum desired cashback.
- Desired account types.
- Desired institution types.
- Geographic preferences.
- Credit union preferences.
- Public or private ownership preferences.
- Minimum or maximum balance.
- Direct deposit availability.
- Debit usage.
- Desired accessibility.
- Risk constraints.

The system should not override explicit user safety or eligibility requirements merely to produce a higher projected return.

## Transparency

BankDividend implementations should clearly distinguish:

- Advertised rate.
- Effective user-specific rate.
- Projected earnings.
- Guaranteed benefits.
- Conditional benefits.
- Promotional benefits.
- Estimated benefits.
- Fees.
- Insurance status.
- Eligibility requirements.
- Data confidence.

The system should not present marketing claims as independently verified facts.

## Conflict of Interest

BankDividend is designed to support consumer-first recommendations.

If an implementation receives:

- Affiliate commissions.
- Referral fees.
- Advertising revenue.
- Sponsorship payments.
- Lead-generation payments.
- Other compensation from financial institutions.

The implementation should disclose the relationship.

Compensation should not secretly influence rankings.

## API and Machine-Readable Design

The specification should support machine-readable representations of:

- Institutions.
- Products.
- Rates.
- Fees.
- Rewards.
- Requirements.
- Insurance.
- Eligibility.
- Calculations.
- Scores.
- Recommendations.
- Sources.
- Verification status.
- Red flags.

Implementations may expose these capabilities through APIs, local applications, AI agents, websites, command-line tools, or other interfaces.

## AI Agent Compatibility

BankDividend is designed to support AI agents that can:

- Discover financial products.
- Retrieve current product information.
- Verify insurance.
- Compare account terms.
- Calculate projected earnings.
- Detect fees.
- Identify requirements.
- Simulate user behavior.
- Score products.
- Explain recommendations.
- Monitor product changes.

AI implementations should avoid presenting uncertain information as verified fact.

When required information cannot be verified, the system should explicitly state that the information is unknown or unverified.

## Consumer Protection Principle

BankDividend should optimize for the user's financial interests while clearly communicating limitations, conditions, and risks.

The system should never hide:

- Fees.
- Requirements.
- Balance limitations.
- Promotional expiration.
- Insurance limitations.
- Eligibility restrictions.
- Material risks.
- Unverified information.

A higher advertised return should not automatically be treated as a better recommendation.

---

## Specification Branding License (SBL)
### Standard
- Fully AGPL-3.0+ compliant system
- Copyleft enforced for network deployments
- Required attribution:
  - Roxanne Ardary
  - https://www.roxanneardary.com/

### Optional

- **Specification Branding License (SBL)**
  - Attribution-free commercial deployment
  - Pricing based on scale, usage, and deployment scope
  - [https://roxanneardary.com/bankdividend/](https://roxanneardary.com/bankdividend/)  

---

## License & Notice Requirements

BankDividend is released under the **GNU Affero General Public License v3.0 or later (AGPL-3.0+)**.   
By contributing to any Open Arsenal project, you agree that your contributions will also be released under this license.

Please note the following:

- All contributions must comply with the **AGPL-3.0+** terms.  
- Under **Section 7** of the license, all redistributions, forks, and derivative works must preserve attribution to:  
  **Roxanne Ardary** and **[roxanneardary.com](https://www.roxanneardary.com/)**.
- BankDividend specifications are free to use with attribution. A Specification Branding License can be negotiated upon request.
- The project's **notice.md** file tracks attribution requirements and contributor acknowledgments.   
  Any update that adds new contributors or modifies attribution should also update `notice.md`. 
- When submitting a pull request, ensure that any new files maintain the attribution headers where applicable.
- Network-deployed versions of this software must also remain fully AGPL-3.0+ compliant, including exposure of source code modifications when applicable under the license.

For full legal details, please refer to the AGPL-3.0+ license and the project's `notice.md` file.
