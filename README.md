# U-C-Berkeley
U C Berkeley Assignments
Context
Imagine driving through town and a coupon is delivered to your cell phone for a restaurant near where you are driving. Would you accept that coupon and take a short detour to the restaurant? Would you accept the coupon but use it on a subsequent trip? Would you ignore the coupon entirely? What if the coupon was for a bar instead of a restaurant? What about a coffee house?

This project uses the UCI In-Vehicle Coupon Recommendation dataset to explore the factors that determine whether a driver accepts or rejects a coupon. Through visualizations, statistical summaries, and probability distributions, we aim to distinguish between customers who accepted a driving coupon versus those who did not.

Data Source
The data comes from the UCI Machine Learning Repository and was collected via a survey on Amazon Mechanical Turk. The survey describes different driving scenarios (destination, time, weather, passenger, etc.) and asks whether the person would accept the coupon.

Y = 1: Accepted the coupon ("right away" or "later before expiration")
Y = 0: Rejected the coupon ("no, I do not want the coupon")
Five coupon types: Restaurants under  20, Coffee Houses, Carry out & Take away, Bars, and Restaurants
 20–$50
 
**Key Findings — Overall Acceptance: from Data analysis **
56.8% of all coupons were accepted overall.
Carry out & Take away coupons have the highest acceptance rate (~73.5%), followed by cheap restaurants (<$20) at ~70.7%.
Bar coupons have the lowest acceptance rate (~41.0%), and Coffee House coupons are nearly a coin flip (~49.9%).
Expensive restaurant coupons ( 20 –  50) are also relatively low at ~44.1%.
This suggests that lower-cost, everyday dining coupons are far more likely to be accepted than discretionary ones like bars or fine dining.


