# U-C-Berkeley
U C Berkeley Assignments
**Context**
==========
Imagine driving through town and a coupon is delivered to your cell phone for a restaurant near where you are driving. Would you accept that coupon and take a short detour to the restaurant? Would you accept the coupon but use it on a subsequent trip? Would you ignore the coupon entirely? What if the coupon was for a bar instead of a restaurant? What about a coffee house?

This project uses the UCI In-Vehicle Coupon Recommendation dataset to explore the factors that determine whether a driver accepts or rejects a coupon. Through visualizations, statistical summaries, and probability distributions, we aim to distinguish between customers who accepted a driving coupon versus those who did not.

Data Source
============
The data comes from the UCI Machine Learning Repository and was collected via a survey on Amazon Mechanical Turk. The survey describes different driving scenarios (destination, time, weather, passenger, etc.) and asks whether the person would accept the coupon.

Y = 1: Accepted the coupon ("right away" or "later before expiration")
Y = 0: Rejected the coupon ("no, I do not want the coupon")
Five coupon types: Restaurants under  20, Coffee Houses, Carry out & Take away, Bars, and Restaurants
 20–$50
 
**Key Findings — Overall Acceptance: from Data analysis **
==========================================================
56.8% of all coupons were accepted overall.
Carry out & Take away coupons have the highest acceptance rate (~73.5%), followed by cheap restaurants (<$20) at ~70.7%.
Bar coupons have the lowest acceptance rate (~41.0%), and Coffee House coupons are nearly a coin flip (~49.9%).
Expensive restaurant coupons ( 20 –  50) are also relatively low at ~44.1%.
This suggests that lower-cost, everyday dining coupons are far more likely to be accepted than discretionary ones like bars or fine dining.

Bar Coupon Analysis (Deep Dive)
================================
Key Findings — Bar Coupons:
--------------------------
Frequency matters most: Drivers who visit bars more than 3 times/month accept at 76.9% vs. 37.1% for those who go ≤3 times. This is the single strongest predictor.

Age + Frequency: Drivers who go to bars more than once AND are over 25 accept at 69.5% — more than double the 33.5% of all others.

Social context: Drivers with friends as passengers have the highest bar coupon acceptance, while those with kids have the lowest.

Lifestyle segments:
--------------------

Young bar-goers (age <30, bar >1/month): ~72% acceptance
Regular bar-goers who aren't widowed and don't have kid passengers: ~71% acceptance
Budget diners with lower income: ~46% acceptance
Hypothesis: Bar coupon acceptance is primarily driven by existing bar-going behavior and social context rather than purely economic factors.

Independent Investigation: Coffee House Coupons
===============================================
Key Findings — Coffee House Coupons:
---------------------------------------
Visit frequency is again the strongest predictor: Those who visit coffee houses 4+ times/month accept at ~67%, while those who never visit accept at only ~34%.
Time of day matters: Morning (10AM) shows the highest acceptance (~56%), aligning with typical coffee consumption patterns. Evening (6PM, 10PM) shows notably lower acceptance.
Weather impact: Sunny weather drives slightly higher acceptance. Snowy/rainy conditions reduce willingness to detour for coffee.
Expiration: Coupons with 1-day expiration are accepted at much higher rates (~58%) than 2-hour coupons (~43%), giving drivers flexibility increases acceptance.
Temperature: Warmer weather (80°F) shows higher acceptance than cold weather (30°F), possibly because people are more willing to make a stop in pleasant conditions.
Gender: Females show slightly higher acceptance rate for coffee house coupons than males.

Conclusions & Recommendations
=================================
Summary of Findings
-------------------
Analyzing the given dataset objetive was to understand what factors distinguish coupon acceptors from rejectors. I analysed the data set using statistical methods , and my Key findings are as below:

Below are the strongest predictors of coupon acceptance (by Cramér's V):

Coupon type (V=0.26): This type of coupon is the single most important factor. Carry out and cheap restaurant coupons enjoy ~70%+ acceptance, while bar and expensive restaurant coupons hover around 41–44%.
Visit frequency (V=0.15 for CoffeeHouse): This is another powerful predictor that lets us know how frequest a visitor visits Coffee House. Bar-goers accept bar coupons at nearly twice the rate of non-bar-goers, and the same pattern holds for coffee houses.
Passenger/social context (V=0.13): It is observed that who is in the car matters — Presence of friends increase acceptance (especially for bars), while kids decrease it.
Destination urgency (V=0.13): Drivers heading to "No Urgent Place" are far more likely to accept coupons than those going to work or home.
Expiration time (V=0.13): Also it is observed that coupons with longer expiration (1 day) increases acceptance significantly compared to 2-hour coupons, giving drivers flexibility.
Time of day (V=0.12): Acceptance varies by time — coffee coupons peak in the morning, bar coupons in the evening, aligning with natural consumption patterns.
Weather & temperature (V=0.10, 0.06): Sunny, warm weather modestly increases acceptance.

Actionable Recommendations for Coupon Targeting:
================================================
Target frequent visitors: Someone who already goes to bars or coffee houses is 2× more likely to accept a coupon for that venue.
Match timing to behavior: Send coffee coupons in the morning, bar coupons in the evening.
Extend expiration: 1-day coupons dramatically outperform 2-hour coupons.
Consider social context: Target bar/restaurant coupons when drivers have friends (not kids) as passengers.
Avoid targeting urgent trips: Focus on leisure driving or "no urgent place" destinations.

Link to Python Code :
======================
[https://github.com/mrsarojnayak/U-C-Berkeley/blob/main/Coupon_Acceptance_Solution_Saroj_Nayak.ipynb](https://github.com/mrsarojnayak/U-C-Berkeley/blob/main/Will%20the%20Customer%20Accept%20the%20Coupon/Coupon_Acceptance_Solution_Saroj_Nayak.ipynb)

Link to output : To view the output from the above python code please download the below file 
=================
[https://github.com/mrsarojnayak/U-C-Berkeley/blob/main/Coupon_Acceptance_Solution_Saroj_Nayak.html
To View the output : Download this file ](https://github.com/mrsarojnayak/U-C-Berkeley/blob/main/Will%20the%20Customer%20Accept%20the%20Coupon/Coupon_Acceptance_Solution_Saroj_Nayak.html)

   


