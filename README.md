# Pine-Script---Short-Term-Scanner-
Short-Term Scanner (Enhanced with 0.5% or More)


Code improvements:
Condition for movement of 0.5% or more:

Added conditions that verify that the movement is indeed above 0.5% of the current price or below 0.5%.
Added logic in the section:
pinescript
Copy code
exceeds_target_up = ta.highest(high, lookahead_bars) >= target_up and (ta.highest(high, lookahead_bars) - close) / close >= 0.005
exceeds_target_down = ta.lowest(low, lookahead_bars) <= target_down and (close - ta.lowest(low, lookahead_bars)) / close >= 0.005
Combining volume conditions:

The signals are displayed only if the condition of volume above the average (as defined in the code) is met.
Enhanced signals:

Blue signals are indicated for a movement of 0.5% or more:
Blue arrow pointing up for an upward movement.
Blue arrow pointing down for a downward movement.

Work nice on crypto 
