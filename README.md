T (Liquid Token):

Current code in ....py

1. stress_factor = 0.99  # 99% sellable
2. sellable_supply = circulating_supply * 0.99  # 1% fixed resistance
3. floor_price = market_cap / sellable_supply

Stress Factor (0.99):

1. Function: Intrinsic resistance (holder conviction)
2. Constant: 1% of tokens are never sold, even under extreme stress
3. Applied to: All calculations (Bear, Bull, baseline)

----------------------------------------------

T (Staking Token):

Code for T with dynamic resistance
floating_supply = circulating_supply - bonded_tokens
resistance_factor = get_resistance_factor(staking_rate)  # 2% to 15%
stakeable_vendable = bonded_tokens * (1 - resistance_factor)
total_sellable = floating_supply + stakeable_sellable

