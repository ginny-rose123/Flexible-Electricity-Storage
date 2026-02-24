# Flexible-Electricity-Storage

**⚡️ Background**

Flexible electricity storage expansion is the growth of technologies that shift electricity across time: charging when power is abundant and cheap, then  discharging when scarce and expensive. It is critical for integrating large renewable generation into the grid, while limiting price volatility and maintaing reliability.

**❓ Problem Statement**

This project uses publicly available data on the EU to analyse which countries are most primed for expanding flexible electricity storage. It could be used to inform international expansion of companies.

**👩‍💻 Analytical Approach**

To identify which countries are primed for flexible storage expansion, I analysed: 1) market readiness, 2) market opportunity. 

**Market readiness** is the ability for the country to expand electricity storage to capitalise on increased renewable generation and benefit from smoothing supply to the grid. It is measured as: 
1) EV chargers per million - used as a proxy for previous investment in new electricity infrastructure and grid modernisation.
2) Renewable generation - exposure to renewable electricity fluctuations and generation levels.

**Market benefits** is the scale of opportunity of smoothing renewable electricity supply over time through greater storage. It is measured as: 
1) Electricity price variation - standard deviation of day-ahead electricity prices, potentially due to fluctuations in the supply of renewable electricity.
2) Negative price instances - instances where supply is outstripping demand such that generators are paying to supply to the grid, potentially due to oversupply of renewables.

Each measure is scaled, then measured from 1 to 25. The total opportunity score is measured out of 100. Colour density on the dashboard is measured as Top 5, Top 10 and 'Other' based on the selected metric or compostie score. 

Data was cleaned, manipulated and merged in Python then exported to Tableau for visualisation. 

**📄 Data and Supporting Documents**

[Published Dashboard](https://public.tableau.com/views/FlexibleElecOpportunity/Dashboard1?:language=en-GB&publish=yes&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link)

[EV Chargers](https://alternative-fuels-observatory.ec.europa.eu/transport-mode/road/european-union-eu27/country-comparison): 2025 data

[Population Data](https://ec.europa.eu/eurostat/web/population-demography/demography-population-stock-balance/database): to calculate EV density

[Renewable Generation](https://ec.europa.eu/eurostat/databrowser/view/nrg_cb_pem__custom_20149696/default/table)

[Electricity Price Data](https://ember-energy.org/data/european-wholesale-electricity-price-data/?utm_source=chatgpt.com)
