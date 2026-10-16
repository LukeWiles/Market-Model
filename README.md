# Market-Model
Researching a market simulation to get a better understanding of optimal ask-bid spread, and the effects of volatility, information, and other variables.

## Research Questions
- How does market volatility affect profit?
- What ask-bid spread is optimal for maximizing profitability?
- Does volatility change a spread's profitability?
- What are the impacts of a more informed customer-base?

## Model/Logic
My simulation mimicks the scenario of a market maker posting bid and ask prices around a fair price. It takes into account different buy/sell rational based on if customers are potentially informed on the direction of price change or not.
- Fair Price: Changes over time based on random price changes.
- Bid/Ask Prices: Determined by the given spread around the fair price.
- Customer Arrivals: Arrival probability decreases as given spread increases.
- Customer Behavior: Uninformed customers make decisions based on their estimated valuations, whilst informed customers choose based on their prediction of the price change.
- Transaction Costs: Each trade incurs a transaction cost.
- Inventory Limit: Market maker can not exceed a certain inventory.

## Experimental Design
The simulation varies the bid-ask spread, volatility, number of "trade steps" that are simulated, as well as the proportion of informed traders. For each of these, multiple simulations are ran, where key metrics are noted. These metrics were average profitability, standard deviation of profit, number of total trades, as well as what percent of simulations ended in a loss.

## Results

### Bid-Spread Vs. Profitability
! [Spread Profitability Graph](Plots/market_maker_profit_vs_spread_cubic_fit.png)