Discounted Cash Flow Valuation Tool

Developed a ratio-driven DCF valuation tool using HTML, CSS, and JavaScript, integrating with the Financial Modelling Prep (FMP) API via asynchronous calls to retrieve five years of financial statements, a company profile, a live quote, and earnings report history for 87 listed companies.

A discounted cash flow model values a business intrinsically rather than relatively: it forecasts the free cash flow the company will generate, discounts each year back at the weighted average cost of capital, and adds a terminal value for everything beyond the explicit forecast. The result is an enterprise value, bridged to equity via net debt and expressed per share, then compared against the market price to give an implied upside and annualised return.

Rather than guessing line items, the application calibrates every driver to the company's own history. EBIT margin, D&A, capex and working-capital intensity are measured as ratios of revenue over five fiscal years, with their direction of travel carried forward in damped, capped form rather than averaged away. Revenue is projected from recent earnings and the current growth trajectory, fading along that path across the forecast rather than resetting abruptly to the terminal rate, and terminal capex converges to D&A plus growth-sustaining reinvestment so the perpetuity carries only the capital spend needed to support its own growth.

Cost of capital is built from CAPM and an after-tax cost of debt weighted by market capitalisation and total debt, with selectable mid-year or year-end discounting. The Gordon-growth terminal value is cross-checked as an implied exit EV/EBITDA multiple against today's market multiple, and its share of enterprise value is reported so an over-reliant model is visible immediately.

Alongside the valuation, a recent-earnings panel shows consensus versus actual revenue and EPS for the last four reports with beat or miss and the size of the surprise, the next scheduled report, and the quarter-on-quarter shift in revenue and EPS.

Outputs include a full free-cash-flow forecast, a cost-of-capital and valuation bridge, a WACC × terminal-growth sensitivity grid, bear/base/bull scenarios, an auditable record of every input pulled from the API, a value waterfall from yearly PV through terminal value and net debt to equity, and a bear/base/bull price-path fan compounding today's price to the implied value.
