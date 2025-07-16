T (Liquid Token):

# Current code in ....py
stress_factor = 0.99  # 99% sellable
sellable_supply = circulating_supply * 0.99  # 1% fixed resistance
floor_price = market_cap / sellable_supply

Stress Factor (0.99):

Function: Intrinsic resistance (holder conviction)
Constant: 1% of tokens are never sold, even under extreme stress
Applied to: All calculations (Bear, Bull, baseline)

----------------------------------------------

T (Staking Token):

# Code for T with dynamic resistance
floating_supply = circulating_supply - bonded_tokens
resistance_factor = get_resistance_factor(staking_rate)  # 2% to 15%
stakeable_vendable = bonded_tokens * (1 - resistance_factor)
total_sellable = floating_supply + stakeable_sellable

