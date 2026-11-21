# NYC Airbnb Market Analysis & Revenue Insights

**Course:** IDS 509 – Case Study 1  
**Project Type:** Academic Group Project  
**Focus Areas:** Business Analytics · Python · Data Analysis · Statistical Modeling · Revenue Estimation · Generative AI

## Project Overview

This project analyzes over 40,000 Airbnb listings across New York City's five boroughs using data from [Inside Airbnb](https://insideairbnb.com/). The dataset was provided by the course instructor.

The goal was to understand NYC's short-term rental market from both a host and business perspective. We examined listing concentrations, rental prices, property characteristics, host growth trends, estimated host revenue, and potential Airbnb earnings under different fee assumptions.

The analysis translates data into practical insights and recommendations for current and prospective Airbnb hosts.

## Business Problem

Airbnb hosts operate in a competitive market where pricing, property characteristics, location, and competition can influence potential revenue.

This project addresses several business questions:

- Which NYC boroughs have the highest concentration of Airbnb listings?
- How do rental prices differ across boroughs and neighborhoods?
- What property characteristics are associated with higher nightly prices?
- How has the number of new hosts changed over time?
- Which hosts appear to generate the highest estimated revenue?
- What might Airbnb's NYC earnings look like under different fee assumptions?

## Tools & Technologies

- **Python** – Data cleaning, analysis, and statistical modeling
- **Pandas & NumPy** – Data manipulation and calculations
- **Matplotlib & Seaborn** – Data visualization
- **SciPy** – Statistical testing
- **Statsmodels** – Multiple linear regression
- **Google Colab** – Analysis environment
- **Google Gemini** – AI-assisted code generation through prompting within Google Colab
- **Excel/CSV** – Dataset handling and supporting analysis

## Analytical Approach

1. **Data Preparation:** Reviewed missing values, investigated duplicate listing identifiers, converted date and price fields, and developed a unique row identifier to preserve the original listing records.

2. **Exploratory Data Analysis:** Examined listing distributions, room types, borough-level pricing, and neighborhood-level patterns.

3. **Geographic Analysis:** Calculated distances to selected NYC landmarks and transportation hubs to explore relationships between proximity and listing prices.

4. **Statistical Analysis:** Applied correlation analysis, chi-square testing, ANOVA, and multiple linear regression to evaluate relationships between listing characteristics and prices.

5. **Host Analysis:** Examined host registration trends and developed review-based revenue estimates.

6. **Revenue Scenarios:** Estimated potential Airbnb earnings using alternative fee assumptions and an annualized revenue model.

7. **Business Recommendations:** Translated analytical findings into recommendations for existing and prospective hosts.

## Key Findings

### 1. Listing Distribution Across NYC

- Manhattan had the largest concentration of Airbnb listings, followed by Brooklyn.
- Together, these boroughs represented approximately 80% of the listings analyzed.
- Entire homes and apartments were the dominant listing types in several boroughs.
- Private rooms were relatively more common in the Bronx and Queens.

**Business Insight:** Manhattan and Brooklyn represent the largest concentrations of Airbnb competition, while boroughs differ in their mix of available property types.

### 2. Pricing, Affordability & Location

- Median nightly prices varied substantially across NYC boroughs.
- Manhattan had the highest median nightly price, while the Bronx had the lowest.
- Neighborhood-level prices varied considerably, even within the same borough.
- Distance from selected NYC landmarks and transportation hubs showed a negative relationship with listing prices.
- Listings closer to selected landmarks had a higher share of entire-home listings.

**Business Insight:** Location is associated with pricing differences, but it does not explain the entire market. Property type and neighborhood characteristics also matter.

### 3. Price Distribution & Room Types

- Manhattan had the highest median nightly prices among the boroughs analyzed.
- Its price distribution was strongly right-skewed, with a relatively small number of unusually expensive listings.
- Higher-priced listings were more prevalent in Manhattan than in other boroughs.
- Across NYC, hotel rooms and entire homes/apartments generally had higher median prices than private and shared rooms.

**Business Insight:** Room type and location create meaningful differences in pricing potential. Median prices provide a more representative comparison than averages when extreme listings are present.

### 4. Property Characteristics & Pricing Drivers

Statistical analysis identified several listing characteristics associated with nightly prices:

- Guest capacity showed a strong positive relationship with listing prices.
- Bedrooms, beds, and bathrooms were also positively associated with prices.
- Number of reviews showed a comparatively weak relationship with listing prices.

A multiple linear regression model was developed to examine how listing characteristics relate to log-transformed nightly prices.

Room type, borough, guest capacity, bedrooms, and bathrooms were among the variables associated with price differences in the model.

**Business Insight:** Property capacity and accommodation type appear more informative for pricing than review volume alone. These are statistical associations, not proof that changing one feature will cause a particular price increase.

### 5. Host Growth Trends

- New host registrations reached their highest levels during the earlier years represented in the dataset.
- The number of new hosts generally declined after the peak period.
- Borough-level trends differed, with the Bronx showing a different growth pattern from the larger markets.

**Business Insight:** The NYC Airbnb market has changed over time, and market entry trends are not uniform across boroughs. Historical growth should be considered alongside current competition and demand.

### 6. Host Revenue Estimates

The dataset does not include operating expenses, occupancy records, or verified booking revenue, so actual host profit could not be calculated.

Two approaches were used to explore potential host revenue:

- A simple price-times-review proxy to compare hosts.
- An annualized estimate using review activity, assumed review rates, assumed nights per booking, and listing prices.

The annualized analysis suggested that a relatively small group of hosts with multiple listings accounted for a meaningful share of estimated revenue.

It also highlighted the importance of distinguishing larger commercial operators from individual-style hosts.

**Business Insight:** High estimated gross revenue does not necessarily mean high profit. Operating costs, occupancy, property ownership, management expenses, and booking patterns would be needed for a more complete profitability analysis.

### 7. Estimated Airbnb NYC Earnings

Two fee scenarios were evaluated to explore potential platform earnings.

The analysis considered:

- A review-based booking-value proxy.
- An annualized gross booking-value estimate.
- Alternative host-fee and combined take-rate assumptions.
- Sensitivity analysis using different review rates and average booking lengths.

The results demonstrated how estimated platform earnings can vary substantially depending on fee structures and booking-related assumptions.

Manhattan and Brooklyn represented the largest estimated revenue contributions in the annualized analysis.

**Important:** These figures are illustrative estimates, not Airbnb-reported financial results. Actual fee structures can vary, and the estimates depend on review behavior and booking-length assumptions.

## Business Recommendations

### For Current Airbnb Hosts

- Compare pricing against similar listings in the same neighborhood and room category.
- Highlight property features associated with higher prices, such as guest capacity, bedrooms, bathrooms, and privacy.
- Use median neighborhood prices as a practical benchmark rather than relying on citywide averages.
- Do not assume that a higher review count automatically supports a higher nightly price.
- Evaluate profitability using operating costs and occupancy, not nightly price or estimated gross revenue alone.

### For Prospective Airbnb Hosts

- Evaluate neighborhood-level competition and room-type demand before entering the market.
- Consider how property size, capacity, and location fit the local market.
- Investigate affordability and potential demand in less expensive boroughs, while recognizing that lower prices do not automatically mean better investment returns.
- Build a financial plan that accounts for acquisition or rental costs, maintenance, operating expenses, regulations, and occupancy.

## Limitations & Assumptions

- The dataset is a listing-level snapshot and does not provide complete booking or occupancy records.
- Listing prices represent advertised nightly prices, not necessarily the prices guests ultimately paid.
- The dataset does not include host expenses, so actual host profit cannot be calculated.
- Reviews are used as an indirect indicator of booking activity; not every booking results in a review.
- Revenue estimates depend on assumptions about review rates, booking length, and fee percentages.
- The selected landmark-distance analysis does not capture every factor affecting location value.
- Regression and correlation results identify associations, not causation.
- Some listing fields contain missing values or potential data-quality issues.

The project therefore presents directional market insights and illustrative revenue estimates rather than audited financial results or investment guarantees.

## Project Context & Collaboration

This project was completed as part of an IDS 509 academic group case study using Inside Airbnb data.

The project involved collaborative data analysis, statistical modeling, visualization, and business interpretation.

**AI-Assisted Development:** Google Gemini was used through prompting within Google Colab to generate Python code for portions of the analytical workflow. The generated code was used as part of the project development process.

## Source Code Availability

The source code and detailed implementation for this project are not publicly available because the project was completed as part of an academic group assignment.

Recruiters, hiring professionals, or other interested individuals who would like to review the technical implementation are welcome to contact me to request access, subject to applicable course and team-sharing restrictions.

---

**Project Takeaway:** NYC Airbnb pricing and estimated revenue vary substantially by borough, room type, property characteristics, and location. Turning these patterns into useful business decisions requires looking beyond nightly prices to competition, operating costs, occupancy, and the assumptions behind revenue estimates.