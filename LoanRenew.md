# LoanRenew

## Deterministic Refinancing With Renewable Capital

LoanRenew is an open source specification for a personally owned refinancing business built around deterministic loan repayment, renewable lending capital, transparent profit allocation, investor participation, mortgage documentation, and public-record transparency.

The specification defines a modular financial architecture in which deterministic interest generated through refinancing becomes the business's profit. Thirty-three percent of realized profit is provisionally reserved for tax liabilities. The remaining profit is divided between renewable lending capital and an operating allocation that supports expenses, overhead, and investor dividends.

LoanRenew is designed to make the movement of capital independently understandable and auditable. Every major stage of the lending cycle can be represented through structured records, including capital contributions, refinancing transactions, mortgage records, deterministic repayment schedules, realized interest, tax reserves, reinvestment, investor capital growth, dividends, expenses, and public-record references.

## Specification Goals

LoanRenew is designed around the following principles:

- Deterministic refinancing economics
- Renewable lending capital
- Personally owned business architecture
- Separation of company ownership from capital participation
- Transparent investor accounting
- Automatic reinvestment of the lending allocation
- Optional reinvestment of investor dividends
- Annual tax-reserve reconciliation
- Mortgage and title transparency
- Public-record verification
- Immutable financial records
- Auditable capital allocation
- Modular architecture
- Vendor-neutral implementation
- Open source implementation under AGPL-3.0+
- Human-readable and machine-readable reporting

## Core Economic Model

LoanRenew begins with capital contributed by the principal owner and participating investors.

Capital is deployed into qualifying refinancing transactions using the LoanRenew refinancing and Solvra-based deterministic repayment model.

Loan repayments distinguish between:

- Principal repayment
- Deterministic interest repayment

Returned principal is capital recovery and is not treated as profit.

Deterministic interest that has been realized becomes business profit.

The basic allocation model is:

- 33% of realized profit is provisionally reserved for taxes.
- 67% remains available for business allocation.
- 60% of the remaining profit goes into the new-loan funding pool.
- 40% goes into the operating allocation.
- 10% of the operating allocation forms the investor dividend pool.
- 90% of the operating allocation is available for expenses, overhead, owner distributions, and tax-reserve shortfalls.

## Capital Renewal

The 60% reinvestment allocation is automatically returned to the lending system.

Each participating investor receives an exact proportional increase in their capital account based on their applicable percentage of participating capital.

For example, if an investor represents 1% of participating capital and the reinvestment allocation is $10,000, that investor receives a $100 increase to their capital account.

The reinvestment amount is not treated as a cash dividend. It becomes additional lending capital attributable to the investor.

This creates a renewable capital cycle:

Capital → Refinancing → Repayment → Interest Profit → Reinvestment → New Loans

## Investor Participation

Investor participation is based on capital contributed to the participating capital pool.

Investor participation percentage is calculated as:

Investor Capital ÷ Total Participating Capital

Capital participation does not automatically constitute ownership of the business.

Unless a separate agreement provides otherwise, participating investors do not receive company ownership, management control, intellectual property rights, or ownership of the underlying business.

Each investor maintains an individual capital ledger recording:

- Original contribution
- Additional contributions
- Reinvestment allocations
- Dividend reinvestments
- Cash dividends
- Withdrawals where permitted
- Current capital
- Current participation percentage
- Historical capital balances

## Investor Dividend Election

The investor's proportional share of the 10% investor dividend pool is an earned dividend.

Each investor may elect to:

- Receive the dividend as cash
- Add the dividend to the refinancing funding pool

The election must be established before January 1 of the applicable calendar year.

The election applies to eligible dividends earned during that calendar year.

If an investor elects cash distribution, the dividend is paid according to the applicable distribution schedule.

If an investor elects dividend reinvestment, the dividend is added to the investor's capital account and becomes additional lending capital.

The automatic 60% reinvestment allocation and the optional dividend reinvestment are tracked separately.

## Core Modules

### 1. Capital Module

The Capital Module establishes the foundational capital accounting system.

Responsibilities include:

- Recording principal owner capital
- Recording investor capital
- Maintaining total participating capital
- Calculating participation percentages
- Tracking capital balances
- Recording capital additions
- Recording permitted withdrawals
- Maintaining historical capital states
- Separating company ownership from capital participation
- Providing capital data to allocation modules

The Capital Module is the authoritative source for participating capital balances.

### 2. [Solvra Loan Module Specification](https://gitlab.com/Roxanne_Ardary/solvra/-/tree/f569d9aed2f32e3e8cfdbcdc17b84f454a0b6040/)  
[https://roxanneardary.com/solvra/](https://roxanneardary.com/solvra/)  

The Solvra Loan Module provides the deterministic loan calculation framework used by LoanRenew.

Responsibilities include:

- Establishing loan principal
- Establishing deterministic interest
- Establishing loan terms
- Calculating scheduled payments
- Separating principal from interest
- Tracking payment history
- Tracking outstanding principal
- Calculating realized interest
- Tracking delinquency and loan status
- Providing repayment data to the Profit Allocation Module

The module must maintain a deterministic relationship between the original loan terms and the expected repayment schedule.

### 3. Refinancing Module

The Refinancing Module manages the deployment of renewable capital into refinancing transactions.

Responsibilities include:

- Identifying eligible refinancing transactions
- Determining available lending capital
- Allocating lending capital
- Creating refinancing records
- Linking refinancing transactions to capital sources
- Tracking deployed principal
- Tracking recovered principal
- Tracking realized interest
- Returning recovered capital to the available funding pool
- Feeding realized interest into the profit allocation system

### 4. Mortgage Module

The Mortgage Module manages the mortgage-backed structure of qualifying refinancing transactions.

Responsibilities include:

- Property identification
- Ownership verification
- Mortgage documentation
- Existing mortgage identification
- Mortgage payoff tracking
- Lien identification
- Mortgage recording
- Mortgage assignment tracking where applicable
- Mortgage release and satisfaction tracking
- Recording references
- Mortgage status
- Property-level loan relationships

The Mortgage Module connects the financial loan record with the legal mortgage record.

### 5. [Magistrate Title Services Module](https://gitlab.com/Roxanne_Ardary/magistrate/-/tree/cbae995772469aa33419bc90eb3ba08acad74b90/)  
[https://roxanneardary.com/magistrate-title-services/](https://roxanneardary.com/magistrate-title-services/)  

The Magistrate Title Services Module provides title-service integration for mortgage-backed refinancing.

Responsibilities include:

- Title research
- Chain-of-title verification
- Ownership verification
- Lien research
- Judgment research
- Tax-lien research
- Existing mortgage research
- Title exception tracking
- Payoff verification
- Closing documentation
- Recording coordination
- Recording verification
- Public-record references

The module is designed around the principle that qualifying mortgage transactions should have verifiable title and recording information.

### 6. Public Record Module

The Public Record Module maintains references to legally recorded documents associated with each mortgage transaction.

Responsibilities include:

- Recording jurisdiction
- Recording date
- Instrument type
- Recording number
- Mortgage recording references
- Release references
- Satisfaction references
- Assignment references where applicable
- Public-record verification
- Document status
- Public-record audit history

The module does not require unnecessary publication of private personal information.

Public-record transparency and personal privacy must be balanced according to applicable law.

### 7. Profit Allocation Module

The Profit Allocation Module applies the deterministic profit distribution rules.

For realized interest profit:

- 33% → provisional tax reserve
- 67% → distributable profit

The distributable profit is then divided:

- 60% → new-loan funding pool
- 40% → operating allocation

The module must record every allocation and provide sufficient information for independent recalculation.

### 8. Reinvestment Module

The Reinvestment Module manages the renewable capital system.

Responsibilities include:

- Receiving the 60% funding allocation
- Calculating each investor's proportional allocation
- Increasing investor capital accounts
- Increasing available lending capital
- Recording reinvestment transactions
- Maintaining reinvestment history
- Supporting compounding capital balances
- Preventing reinvestment allocations from being treated as cash dividends

The reinvestment allocation is automatic according to the applicable participation rules.

### 9. Investor Participation Module

The Investor Participation Module determines each participant's economic percentage.

Responsibilities include:

- Calculating capital participation
- Maintaining participation history
- Applying capital changes
- Calculating proportional reinvestment
- Calculating proportional dividend entitlement
- Maintaining investor capital records

Participation percentages must be reproducible from the underlying capital ledger.

### 10. Investor Dividend Module

The Investor Dividend Module calculates the investor dividend pool.

The investor dividend pool is:

Operating Allocation × 10%

Each participating investor receives their proportional share based on the applicable capital participation percentage.

The module tracks:

- Dividend earned
- Dividend election
- Cash distribution
- Dividend reinvestment
- Distribution date
- Capital impact
- Historical dividend records

### 11. Investor Election Module

The Investor Election Module records annual investor dividend preferences.

Each investor must establish their election before January 1 of the applicable calendar year.

Supported elections include:

- Cash Distribution
- Dividend Reinvestment

The election applies to eligible dividends generated during that calendar year.

The module maintains an auditable history of elections and their effective periods.

### 12. Tax Reserve Module

The Tax Reserve Module establishes a provisional reserve equal to 33% of realized profit.

The reserve is reconciled annually in January for the preceding fiscal year.

If the actual tax liability is less than the reserve:

The remaining balance is transferred into the new-loan funding pool.

The surplus becomes additional renewable capital and is allocated according to applicable capital participation percentages.

If the actual tax liability exceeds the reserve:

The shortfall is paid from the 90% portion of the operating allocation.

Tax reconciliation must not reduce an investor's earned 60% reinvestment allocation.

The module records:

- Provisional tax reserve
- Actual tax liability
- Taxes paid
- Reserve surplus
- Reserve shortfall
- Funding-pool adjustment
- Operating-allocation adjustment
- Annual reconciliation

The 33% reserve is a specification-level allocation rule and does not determine the actual legal tax liability of a business.

### 13. Expense and Overhead Module

The Expense and Overhead Module manages the 90% portion of the operating allocation.

Eligible categories may include:

- Business expenses
- Administrative expenses
- Servicing costs
- Professional services
- Insurance
- Technology
- Marketing
- Compliance
- Infrastructure
- Permitted owner distributions
- Tax-reserve shortfalls

Every transaction should contain sufficient information for reconciliation and audit.

### 14. Transparency Reporting Module

The Transparency Reporting Module is a mandatory core component.

It provides visibility into the financial, lending, capital, mortgage, investor, and operational aspects of LoanRenew.

Business-level reporting may include:

- Total participating capital
- Owner capital
- Investor capital
- Loans originated
- Loans outstanding
- Principal outstanding
- Principal recovered
- Interest realized
- Profit allocations
- Tax reserve
- Reinvestment
- Operating allocation
- Investor dividend pool
- Expenses
- Overhead
- Distributions

Investor reporting may include:

- Original investment
- Current capital
- Capital participation percentage
- Reinvestment earned
- Dividend earned
- Dividend paid
- Dividend reinvested
- Historical transactions

Mortgage reporting may include:

- Property identifier
- Mortgage status
- Recording jurisdiction
- Recording date
- Instrument type
- Recording reference
- Title status
- Lien status
- Release status

Personally identifying information must not be unnecessarily exposed through public transparency systems.

### 15. Capital Ledger Module

The Capital Ledger Module maintains the authoritative transaction history for participating capital.

Every capital event should be recorded.

Examples include:

- Initial capital contribution
- Investor contribution
- Additional capital contribution
- Automatic reinvestment
- Dividend reinvestment
- Permitted withdrawal
- Capital adjustment
- Annual tax-reserve surplus allocation

The ledger should permit reconstruction of historical capital balances and participation percentages.

### 16. Audit Module

The Audit Module independently verifies the economic calculations.

It should be capable of recalculating:

- Loan principal
- Deterministic interest
- Realized profit
- Tax reserve
- Remaining profit
- Reinvestment allocation
- Operating allocation
- Investor dividend pool
- Investor reinvestment
- Investor dividends
- Annual tax reconciliation
- Capital balances

The audit system should identify:

- Missing transactions
- Incorrect allocations
- Capital discrepancies
- Dividend calculation errors
- Reinvestment discrepancies
- Tax reserve discrepancies
- Loan accounting discrepancies
- Unauthorized capital movements

### 17. Governance Module

The Governance Module defines ownership, participation, permissions, decision rights, and specification governance.

It establishes the distinction between:

- Business ownership
- Capital participation
- Investor economic participation
- Management authority
- Loan ownership
- Intellectual property rights

Unless separately established by agreement, investor participation does not create company ownership.

## Annual Accounting Cycle

LoanRenew operates on a recurring annual cycle.

### Before January 1

Investors establish their dividend election for the upcoming calendar year.

### During the Year

The system:

- Originates qualifying refinancing transactions
- Tracks deterministic repayments
- Records realized interest
- Reserves 33% for taxes
- Allocates 60% of remaining profit to new lending
- Allocates 40% to operations
- Calculates investor dividends
- Applies investor dividend elections
- Records all transactions

### January Reconciliation

The preceding year's financial records are reconciled.

The system:

- Determines actual tax liability
- Compares actual taxes with the provisional reserve
- Transfers tax-reserve surplus to the funding pool
- Applies tax shortfalls to the 90% operating allocation
- Updates investor capital where applicable
- Reconciles all capital accounts
- Produces the annual transparency report
- Produces the annual audit record

## Public Transparency Architecture

LoanRenew is designed around a layered transparency model.

### Public Layer

Provides aggregated and legally permissible information such as:

- Capital totals
- Loan totals
- Aggregate repayment information
- Interest totals
- Reinvestment totals
- Tax-reserve totals
- Operating allocations
- Investor dividend pool
- Aggregate expenses
- Mortgage recording references
- Public-record references

### Investor Layer

Provides an investor with their own:

- Capital account
- Participation percentage
- Reinvestment
- Dividend history
- Election history
- Capital transactions

### Management Layer

Provides authorized operators with complete operational information necessary to manage the business.

### Public Record Layer

Links mortgage and title records to their applicable governmental recording references.

## Optional Plugin Modules

LoanRenew's core modules define the financial and transparency architecture without requiring a specific technology vendor.

Optional plugins can extend the specification.

### Payment Processing Plugin

Provides integrations for:

- Electronic payments
- ACH processing
- Payment reconciliation
- Automated repayment collection
- Payment status updates

### Banking Integration Plugin

Provides integrations for:

- Bank accounts
- Transaction feeds
- Capital transfers
- Reconciliation
- Funding accounts

### Accounting Integration Plugin

Provides integrations for:

- General ledgers
- Journal entries
- Expense management
- Financial statements
- Account reconciliation

### Tax Reporting Plugin

Provides integrations for:

- Tax preparation
- Tax reporting
- Tax-document generation
- Tax liability calculations
- Annual reconciliation

### Credit Assessment Plugin

Provides optional underwriting functionality for evaluating refinancing eligibility.

### Loan Servicing Plugin

Provides:

- Automated payment processing
- Borrower communications
- Delinquency tracking
- Payment schedules
- Servicing records

### Investor Portal Plugin

Provides investors with access to:

- Capital balances
- Reinvestment history
- Dividend history
- Election settings
- Annual statements
- Transaction records

### Public Transparency Portal Plugin

Provides a public-facing interface for:

- Aggregate financial reporting
- Loan statistics
- Capital statistics
- Reinvestment statistics
- Annual reconciliation reports
- Public-record references

### Document Generation Plugin

Provides automated generation of:

- Loan documents
- Mortgage documents
- Notices
- Statements
- Investor reports
- Audit reports

### Notification Plugin

Provides notifications for:

- Loan events
- Payment events
- Investor distributions
- Election deadlines
- Annual reconciliation
- Recording events

### Regulatory Compliance Plugin

Provides configurable compliance functionality for applicable jurisdictions and business structures.

## Data Integrity

LoanRenew implementations should preserve the integrity of financial and public-record data.

Core requirements include:

- Immutable transaction identifiers
- Timestamped records
- Transaction provenance
- Versioned records
- Reproducible calculations
- Audit trails
- Capital reconciliation
- Loan reconciliation
- Mortgage-record reconciliation
- Investor-account reconciliation

Any modification to a material financial record should preserve the original record and document the reason for the change.

## Deterministic Calculation Principle

A central requirement of LoanRenew is that financial outcomes must be reproducible.

Given the same:

- Loan terms
- Payment history
- Capital ledger
- Profit records
- Participation percentages
- Allocation rules
- Investor elections
- Tax reconciliation data

an independent implementation should produce the same:

- Profit
- Tax reserve
- Reinvestment
- Operating allocation
- Investor dividend
- Investor capital balance
- Annual reconciliation

This principle allows the financial model to be independently audited and implemented by multiple systems.

## Example

Assume:

- Principal owner capital: $100,000
- Investor capital: $1,000
- Total participating capital: $101,000
- Realized interest profit: $20,000

The investor's initial participation percentage is:

$1,000 ÷ $101,000 = 0.990099%

### Profit Allocation

Tax reserve:

$20,000 × 33% = $6,600

Remaining profit:

$20,000 × 67% = $13,400

New-loan funding:

$13,400 × 60% = $8,040

Operating allocation:

$13,400 × 40% = $5,360

Investor dividend pool:

$5,360 × 10% = $536

Investor reinvestment from the 60% allocation:

$8,040 × 0.990099% = $79.60

Investor dividend:

$536 × 0.990099% = $5.31

If the investor elected cash dividends, their capital becomes:

$1,000 + $79.60 = $1,079.60

and they receive:

$5.31 cash

If the investor elected dividend reinvestment, their capital becomes:

$1,000 + $79.60 + $5.31 = $1,084.91

and no cash dividend is distributed.

## Tax Reconciliation Example

Assume the provisional tax reserve is $6,600.

If actual annual tax liability is $5,000:

Tax reserve surplus:

$6,600 - $5,000 = $1,600

The $1,600 is transferred to the new-loan funding pool and allocated according to the applicable capital participation rules.

If actual annual tax liability is $7,500:

Tax shortfall:

$7,500 - $6,600 = $900

The $900 is taken from the 90% operating allocation.

The investor's earned 60% reinvestment allocation remains unchanged.

## Security and Privacy

LoanRenew implementations should protect financial and personal information while maintaining the transparency required by the specification.

Security controls may include:

- Encryption
- Access controls
- Authentication
- Authorization
- Audit logging
- Data minimization
- Secure document storage
- Separation of public and private records
- Protection of financial credentials
- Protection of borrower information

Public transparency must not be interpreted as permission to disclose protected personal information.

## Extensibility

LoanRenew is designed to support implementations ranging from a small personally owned refinancing operation to a larger software platform.

The core specification defines the economic rules and data relationships.

Plugins may provide jurisdiction-specific, technical, financial, banking, accounting, title, servicing, reporting, or compliance functionality without changing the core economic model.

## Specification Philosophy

LoanRenew is built around five fundamental principles:

1. **Deterministic Lending**
   
   Loan terms and repayment economics are established transparently and calculated consistently.

2. **Renewable Capital**
   
   A defined portion of realized profit continuously returns to the lending pool.

3. **Investor Participation**
   
   Investors receive proportional capital growth and may choose whether eligible dividends are distributed or reinvested.

4. **Public-Record Transparency**
   
   Mortgage and title activity is connected to verifiable public records whenever legally permissible.

5. **Auditable Economics**
   
   Every material allocation can be independently reconstructed from the underlying records.  

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
  - [https://roxanneardary.com/loanrenew/](https://roxanneardary.com/loanrenew/)  

---

## License & Notice Requirements

LoanRenew is released under the **GNU Affero General Public License v3.0 or later (AGPL-3.0+)**.
By contributing to any Open Arsenal project, you agree that your contributions will also be released under this license.

Please note the following:

- All contributions must comply with the **AGPL-3.0+** terms.
- Under **Section 7** of the license, all redistributions, forks, and derivative works must preserve attribution to:
  **Roxanne Ardary** and **[roxanneardary.com](https://www.roxanneardary.com/)**.
- LoanRenew specifications are free to use with attribution. A Specification Branding License can be negotiated upon request.
- The project's **notice.md** file tracks attribution requirements and contributor acknowledgments.
  Any update that adds new contributors or modifies attribution should also update `notice.md`.
- When submitting a pull request, ensure that any new files maintain the attribution headers where applicable.
- Network-deployed versions of this software must also remain fully AGPL-3.0+ compliant, including exposure of source code modifications when applicable under the license.

For full legal details, please refer to the AGPL-3.0+ license and the project's `notice.md` file.
