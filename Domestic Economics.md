# Domestic Economics

**The Labor Behind a Functioning Home.**

Domestic Economics is an AI-powered open source specification for measuring, valuing, and documenting the labor and economic contribution that takes place within a household.

The specification allows users to describe household duties in natural language and uses AI to identify tasks, classify domestic labor, match activities to comparable occupations, calculate current market wages, account for time and frequency, and produce an estimated economic value for the work performed.

Domestic Economics recognizes that household contribution extends beyond employment income. Cooking, childcare, education, cleaning, caregiving, transportation, household administration, mental labor, maintenance, planning, and other domestic responsibilities require time, skill, and labor. The specification provides a structured way to make that work measurable and economically visible.

## Core Principles

- Household labor is economically valuable even when it does not generate direct income.
- Domestic work should be measured at the level of individual duties and activities.
- Wage comparisons should use current and geographically relevant labor-market data whenever available.
- AI-generated classifications and calculations should remain transparent and reviewable.
- Users should be able to correct assumptions and override AI classifications.
- Historical valuations should preserve the wage data and methodology used at the time of calculation.
- Household labor value should remain distinct from taxable income unless applicable law explicitly provides otherwise.
- Household data should remain under user control.
- The specification should remain modular, vendor-neutral, and extensible.
- Core functionality should not depend on optional plugins.

## Core Modules

### Household Duty Entry

Allows users to describe household responsibilities using natural language.

Features include:

- Natural language household duty entry
- Recurring duty entry
- Duty templates
- Daily, weekly, monthly, and seasonal schedules
- Custom household activities
- Multiple household member support
- Actual and estimated time entry
- Optional time tracking
- Duty notes and descriptions

### AI Duty Recognition

Uses AI to identify and structure household labor from user-provided descriptions.

Features include:

- Natural language processing
- Household activity recognition
- Duty classification
- Contextual task interpretation
- Ambiguity detection
- Clarification requests
- Task categorization
- Assumption detection
- Human review and correction

### Task Decomposition

Breaks complex household responsibilities into measurable labor activities.

Features include:

- Complex duty decomposition
- Task splitting
- Task bundling
- Multi-occupation task identification
- Concurrent task recognition
- Recurring task recognition
- Seasonal task recognition
- On-call responsibility recognition

### Occupation Matching

Maps household activities to comparable paid occupations.

Features include:

- Comparable occupation identification
- Multiple occupation matching
- Occupational similarity scoring
- Alternative occupation suggestions
- Occupation classification transparency
- User occupation overrides
- Occupation mapping history
- Custom occupation definitions

### Wage Intelligence

Determines current market wages associated with comparable occupations.

Features include:

- Current wage data
- Hourly wage calculations
- Annual wage conversion
- Local wage data
- State wage data
- Metropolitan wage data
- National wage data
- Wage source comparison
- Wage data freshness tracking
- Wage dataset versioning
- Historical wage datasets
- Fallback wage sources

### Geographic Wage Adjustment

Adjusts household labor valuations according to the applicable labor market.

Features include:

- Local labor-market matching
- Metropolitan wage matching
- State wage matching
- National wage fallback
- Geographic wage comparisons
- Cross-region valuation
- Geographic data source tracking

### Time and Frequency Calculation

Calculates the amount of labor represented by each household responsibility.

Features include:

- Hours per occurrence
- Hours per day
- Hours per week
- Hours per month
- Hours per year
- Frequency calculations
- Seasonal schedules
- Variable-duration activities
- On-call availability
- Actual versus estimated hours
- Concurrent activity handling

### Labor Valuation

Calculates the market-equivalent value of household labor.

Features include:

- Hourly labor value
- Weekly labor value
- Monthly labor value
- Annual labor value
- Task-level valuation
- Occupation-based valuation
- Market replacement value
- Direct wage-equivalent value
- Multiple occupation valuation
- Confidence scoring

### Replacement Cost

Calculates what it could cost to replace household labor with paid services.

Features include:

- Individual duty replacement costs
- Complete household replacement costs
- Local market replacement costs
- Multiple worker calculations
- Employer cost estimates
- Benefits and overhead estimates
- Outsourcing comparisons
- Avoided household expenses
- Replacement assumptions
- Replacement confidence scoring

### Household Production

Measures goods and services produced within the household.

Features include:

- Meal production valuation
- Food production valuation
- Gardening production
- Food preservation
- Home education
- Child development support
- Household maintenance production
- Home improvement production
- Transportation production
- Care production
- Administrative production
- Household output categories
- Household production history
- Production value calculation

### Household Balance Sheet

Provides a broader view of household economic activity.

Features include:

- Paid income tracking
- Domestic labor value
- Household production value
- Household expenses
- Outsourced labor costs
- Avoided replacement costs
- Economic activity summaries
- Historical household balance sheets
- Household economic comparisons
- Scenario-based balance sheets

The balance sheet keeps monetary income, unpaid labor value, household production, expenses, and replacement costs as separate categories.

### Mental Labor

Measures cognitive and organizational work required to operate a household.

Features include:

- Planning recognition
- Scheduling recognition
- Monitoring recognition
- Anticipatory labor recognition
- Decision-making measurement
- Household coordination
- Household memory tracking
- Research activities
- Administrative labor
- Cognitive workload measurement
- Cognitive labor valuation
- Invisible labor reporting

### Household Contribution

Aggregates documented household labor into a comprehensive contribution record.

Features include:

- Total household labor value
- Individual contributor values
- Household labor portfolios
- Workload distribution
- Paid and unpaid labor separation
- Household contribution statements
- Contribution trends
- Year-over-year comparisons
- Labor category comparisons
- Household contribution history

### Lifetime Contribution

Maintains a longitudinal record of household labor and economic contribution.

Features include:

- Lifetime labor records
- Historical duty tracking
- Lifetime hours
- Lifetime labor value
- Historical wage matching
- Life-stage analysis
- Lifetime household production
- Lifetime replacement costs
- Contribution timelines
- Lifetime contribution statements

### Inflation and Wage Growth

Tracks changes in the value and replacement cost of household labor over time.

Features include:

- Wage growth tracking
- Inflation adjustment
- Historical nominal values
- Current-dollar values
- Occupational wage trends
- Replacement cost inflation
- Historical comparisons
- Wage dataset versioning
- Real versus nominal valuations
- Domestic labor cost indexing

### What Would It Cost to Replace Me?

Generates a comprehensive replacement-cost report based on the user's documented household responsibilities.

The report can include:

- Total annual replacement cost
- Monthly replacement cost
- Hourly replacement cost
- Individual duty costs
- Comparable occupations
- Estimated annual hours
- Local wage rates
- Multiple worker requirements
- Employer-side costs
- Benefits and overhead
- Outsourcing comparisons
- Calculation assumptions
- Data sources
- Confidence levels

The report provides a practical summary of what the household could potentially have to spend if the documented unpaid labor were replaced with paid services.

### Reporting

Produces transparent and reusable household labor reports.

Features include:

- Household labor reports
- Contribution summaries
- Task-level reports
- Occupation equivalency reports
- Wage source reports
- Methodology reports
- Replacement-cost reports
- Lifetime contribution reports
- Historical reports
- Printable reports
- Machine-readable reports

### Research

Provides tools for studying household labor and domestic economic activity.

Features include:

- Research dataset generation
- Privacy-preserving data exports
- Aggregate labor statistics
- Household labor distribution analysis
- Time allocation analysis
- Economic contribution analysis
- Regional analysis
- Historical analysis
- Occupation mapping analysis
- Unpaid labor research
- Household production research
- Care economy research
- Mental labor research
- Economic policy research
- Research API

Research functionality should support anonymization and aggregation to prevent disclosure of identifiable household information.

### Data and Privacy

Protects household information and supports user-controlled data management.

Features include:

- Local-first operation
- User-owned data
- Local data storage
- Encrypted storage
- User-controlled deletion
- Data import
- Data export
- Minimal data collection
- Provider independence
- AI provider independence
- Audit records
- Calculation history

### Explainability and Auditability

Makes AI-generated valuations understandable and reproducible.

Features include:

- Calculation explanations
- Occupation mapping explanations
- Wage source documentation
- Geographic source documentation
- Time calculation documentation
- Assumption tracking
- User modification tracking
- Confidence scoring
- Calculation history
- Reproducible valuations
- Dataset version tracking

## Optional Plugin Modules

Domestic Economics supports optional plugins that extend the core specification without making specialized functionality part of the required core.

### Childcare Plugin

Provides specialized valuation for:

- Infant care
- Childcare
- Supervision
- Child transportation
- Activity coordination
- Developmental support
- Household childcare administration

### Eldercare Plugin

Provides specialized valuation for:

- Elder supervision
- Personal assistance
- Transportation
- Meal preparation
- Appointment coordination
- Household support
- Companionship
- Care administration

### Disability Care Plugin

Provides specialized valuation for:

- Personal assistance
- Mobility assistance
- Daily living support
- Specialized supervision
- Transportation
- Care coordination
- Household accessibility support

### Education Plugin

Provides specialized valuation for:

- Homeschooling
- Tutoring
- Educational planning
- Curriculum development
- Educational administration
- Learning supervision
- Research and preparation

### Cooking Plugin

Provides specialized valuation for:

- Meal planning
- Food preparation
- Cooking
- Kitchen management
- Food storage
- Food preservation
- Nutrition planning
- Grocery coordination

### Cleaning Plugin

Provides specialized valuation for:

- General cleaning
- Deep cleaning
- Sanitation
- Kitchen cleaning
- Bathroom cleaning
- Surface maintenance
- Household organization

### Laundry Plugin

Provides specialized valuation for:

- Washing
- Drying
- Folding
- Ironing
- Clothing organization
- Linen management
- Laundry scheduling

### Transportation Plugin

Provides specialized valuation for:

- School transportation
- Work transportation
- Shopping trips
- Medical transportation
- Family transportation
- Errand coordination
- Vehicle-related household logistics

### Home Maintenance Plugin

Provides specialized valuation for:

- Routine maintenance
- Property upkeep
- Equipment maintenance
- Seasonal maintenance
- Inspection
- Preventive maintenance

### Home Repair Plugin

Provides specialized valuation for:

- Minor repairs
- Construction-related work
- Plumbing tasks
- Electrical tasks
- Carpentry
- Painting
- Fixture replacement

### Gardening Plugin

Provides specialized valuation for:

- Gardening
- Landscaping
- Lawn maintenance
- Food gardening
- Plant maintenance
- Harvesting
- Composting
- Food production

### Pet Care Plugin

Provides specialized valuation for:

- Feeding
- Grooming
- Exercise
- Cleaning
- Transportation
- Pet administration
- Routine animal care

### Household Administration Plugin

Provides specialized valuation for:

- Scheduling
- Recordkeeping
- Correspondence
- Filing
- Household planning
- Appointment management
- Service coordination
- Document management

### Financial Management Plugin

Provides specialized valuation for:

- Household budgeting
- Bill payment
- Financial recordkeeping
- Account management
- Expense tracking
- Financial research
- Household purchasing decisions

### Shopping and Procurement Plugin

Provides specialized valuation for:

- Grocery shopping
- Household purchasing
- Price comparison
- Product research
- Vendor selection
- Inventory management
- Procurement planning

### Event and Family Coordination Plugin

Provides specialized valuation for:

- Family events
- Celebrations
- Travel planning
- Appointment coordination
- Activity scheduling
- Family communications
- Logistics management

### Tax Policy Plugin

Provides an optional framework for modeling household labor recognition policies.

Potential functions include:

- Hypothetical household labor credits
- Caregiver credits
- Social contribution credits
- Tax policy simulations
- Jurisdiction-specific policy models
- Policy scenario comparisons

This module does not represent current tax treatment unless supported by applicable law.

### Benefits Plugin

Provides optional calculations for:

- Employer payroll costs
- Benefits
- Paid leave
- Insurance
- Retirement contributions
- Replacement employment costs

### Historical Wage Plugin

Provides specialized historical wage data for lifetime and longitudinal household labor calculations.

### Research Plugin

Provides additional functionality for:

- Academic research
- Economic studies
- Public policy research
- Household labor datasets
- Statistical analysis
- Aggregate reporting

### Custom Occupation Plugin

Allows users and organizations to create additional occupation mappings for specialized household duties.

## Interfaces

Domestic Economics can support multiple interfaces while maintaining the same underlying specification.

- Web interface
- Mobile interface
- Command-line interface
- API interface
- Local desktop interface
- Research interface
- Data import and export interfaces

## Extensibility

Domestic Economics is designed so that new labor categories, wage sources, geographic datasets, calculation methods, reporting formats, and specialized household domains can be added without modifying the core valuation system.

Optional modules can extend the specification while maintaining compatibility with the core household labor model.

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
  - [https://roxanneardary.com/domestic-economics/](https://roxanneardary.com/domestic-economics/)  

---

## License & Notice Requirements

Domestic Economics is released under the **GNU Affero General Public License v3.0 or later (AGPL-3.0+)**.
By contributing to any Open Arsenal project, you agree that your contributions will also be released under this license.

Please note the following:

- All contributions must comply with the **AGPL-3.0+** terms.
- Under **Section 7** of the license, all redistributions, forks, and derivative works must preserve attribution to:
  **Roxanne Ardary** and **[roxanneardary.com](https://www.roxanneardary.com/)**.
- Domestic Economics specifications are free to use with attribution. A Specification Branding License can be negotiated upon request.
- The project's **notice.md** file tracks attribution requirements and contributor acknowledgments.
  Any update that adds new contributors or modifies attribution should also update `notice.md`.
- When submitting a pull request, ensure that any new files maintain the attribution headers where applicable.
- Network-deployed versions of this software must also remain fully AGPL-3.0+ compliant, including exposure of source code modifications when applicable under the license.

For full legal details, please refer to the AGPL-3.0+ license and the project's `notice.md` file.
