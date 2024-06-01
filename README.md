![Auction](https://github.com/sourceduty/Discount_Auctioning/assets/123030236/0b0a20cd-5c94-4c22-9b87-74c930e561ea)

> A unique auction format where bidders earn discounts from the total sale price for each bid they place.

#
### Overview:

Discount auctioning is a unique auction format where bidders earn discounts from the total sale price for each bid they place. This model incentivizes participation by rewarding bidders directly, while the seller controls the total discount amount and minimum selling price, ensuring a profitable outcome.

#
### Mechanics:

1. Discount Allocation:

- Dynamic Discount Distribution: Introduce a dynamic discounting mechanism where the discount amount per bid increases incrementally as more bids are placed. This encourages sustained participation throughout the auction.

- Example: Start with a $10 discount per bid for the first 10 bids, increase to $15 for the next 20 bids, and $20 for subsequent bids.

2. Bidding Rules:

- Sequential Bidding:
Bids cannot be placed consecutively by the same participant, ensuring diverse participation and preventing monopolization.
 - Unique Bids:
Each new bid must differ from the previous one, encouraging a variety of bid amounts.
 - Strategic Time Intervals:
Implement mandatory time intervals between bids to allow for strategic planning and to prevent rapid-fire bidding. For example, a 1-minute gap between bids.

3. Bid Calculation:

- Total Bids:
Determine the total number of bids based on the difference between the starting price and total price, divided by a chosen increment (pricing distance).
- Example: Total bids = (Total price - Starting price) / Pricing distance.
- Dynamic Pricing Distance:
Adjust the pricing distance based on auction activity. For instance, start with a $100 increment and reduce to $50 after reaching a certain number of bids.

4. Minimum Selling Price:

The seller sets a minimum selling price to ensure profitability. This price should be periodically reviewed and adjusted based on market conditions and past auction performance.

5. Fixed Discount:

Maintain a fixed total discount amount, but allow for dynamic per-bid discounts as described above. Ensure clarity and consistency in discount allocation.

#
### Simulation and Analysis:

Assumptions:

- Total Discount Amount: $1,000
- Starting Price: $10,000
- Total Price: $15,000
- Initial Pricing Distance: $100
- Minimum Selling Price: $8,000

#
### Simulation Parameters:

1. Total Bids:

- Calculation: (Total price - Starting price) / Initial pricing distance.
- Example: (15,000 - 10,000) / 100 = 50 bids.

2. Discount Per Bid:

- Dynamic Distribution:
First 10 bids: $10 discount each.
Next 20 bids: $15 discount each.
Remaining 20 bids: $20 discount each.
- Average Discount Calculation:
(10 * 10 + 20 * 15 + 20 * 20) / 50 = $17 per bid on average.

3. Bidding Dynamics:

- Early Phase: Initial bids earn lower discounts, encouraging early participation.
- Mid Phase: Increasing discounts sustain bidder interest and competition.
- Final Phase: Highest discounts encourage aggressive bidding towards the end.

#
### Outcome Scenarios:

1. Optimistic Scenario:

- High participation drives the final price close to the total price of $15,000.
- Dynamic discounts maximize bidder engagement and satisfaction.

2. Realistic Scenario:

- Moderate participation results in a final price between $12,000 and $14,000.
- Balanced discounting maintains bidder interest, ensuring satisfactory returns.

3. Pessimistic Scenario:

- Low participation results in fewer bids, potentially reaching the minimum selling price of $8,000.
- Dynamic discounts still provide value to participants, with the seller securing the minimum acceptable price.

#
### Summary:

The optimized discount auctioning model introduces dynamic discounting and strategic bidding rules to enhance bidder engagement and optimize revenue outcomes. By adjusting discount amounts and pricing distances based on auction activity, the model maintains competitiveness and fairness. Sellers can leverage these optimizations to maximize returns while ensuring participant satisfaction, making this model suitable for various high-value market segments.

```
-------------------------------------------------
                    RECEIPT
-------------------------------------------------

Item Description                          Amount
-------------------------------------------------
Starting Price                         $10,000.00
Total Discount Amount                  -$1,000.00
                                        ---------
Effective Price After Discount          $9,000.00

Minimum Selling Price Validation:

Effective Price is above the
Minimum Selling Price ($8,000.00)

Additional Costs/Fees                   $5,000.00
                                        ---------
Total Price                            $15,000.00
-------------------------------------------------
Initial Pricing Distance:               $100.00
-------------------------------------------------
Total Bids:                             50
-------------------------------------------------
Discount Per Bid:
First 10 bids:                        $10.00 each
Next 20 bids:                         $15.00 each
Remaining 20 bids:                    $20.00 each
-------------------------------------------------
Thank you for your purchase!
-------------------------------------------------
```

***
Copyright (C) 2024, Sourceduty - All Rights Reserved.
