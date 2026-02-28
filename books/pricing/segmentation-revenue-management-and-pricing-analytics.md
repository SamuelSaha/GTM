# Segmentation, Revenue Management and Pricing Analytics

**Author:** Tudor Bodea, Mark Ferguson  
**Format:** PDF  
**Category:** pricing

---

## Page 2

Segmentation, Revenue 
Management, and 
Pricing Analytics
The practices of revenue management and pricing analytics have transformed the trans-
portation and hospitality industries, and are increasingly important in industries as 
diverse as retail, telecommunications, banking, health care, and manufacturing. Segmen-
tation, Revenue Management, and Pricing Analytics guides students and professionals on 
how to identify and exploit revenue management and pricing opportunities in different 
business contexts.
Bodea and Ferguson introduce concepts and quantitative methods for improving 
profit through capacity allocation and pricing. Whereas most marketing textbooks cover 
more traditional, qualitative methods for determining customer segments and prices, 
this book uses historical sales data with mathematical optimization to make those deci-
sions. With hands-on practice and a fundamental understanding of some of the most 
common analytical models, readers will be able to make smarter business decisions and 
higher profits.
Tudor Bodea is a Revenue Optimization Manager in the Global Revenue Management 
and Systems Department at the InterContinental Hotels Group in Atlanta, USA. He 
earned his Ph.D. in Civil Engineering at the Georgia Institute of Technology, USA, with 
an emphasis on transportation systems, logistics, and statistics. He holds a B.S. in Trans-
portation Systems from the Technical University of Cluj-Napoca, Romania and an M.S. 
in Civil Engineering from the Georgia Institute of Technology.
Mark Ferguson is a Distinguished Business Foundation Fellow and Professor of 
Management Science at the University of South Carolina, USA. He received his Ph.D. in 
Business Administration, with a concentration in operations management, from Duke 
University, USA. He holds a B.S. in Mechanical Engineering from Virginia Tech, USA 
and an M.S. in Industrial Engineering from the Georgia Institute of Technology.

---

## Page 3

This page intentionally left blank

---

## Page 4

Segmentation, 
Revenue Management, 
and Pricing Analytics
Tudor Bodea and Mark Ferguson

---

## Page 5

First published 2014
by Routledge
711 Third Avenue, New York, NY 10017
and by Routledge
2 Park Square, Milton Park, Abingdon, Oxon OX14 4RN
Routledge is an imprint of the Taylor & Francis Group, an informa business
© 2014 Taylor & Francis
The right of Tudor Bodea and Mark Ferguson to be identified as authors of this 
work has been asserted by them in accordance with sections 77 and 78 of the 
Copyright, Designs and Patents Act 1988.
All rights reserved. No part of this book may be reprinted or reproduced 
or utilized in any form or by any electronic, mechanical, or other means, 
now known or hereafter invented, including photocopying and recording, 
or in any information storage or retrieval system, without permission in 
writing from the publishers.
Trademark notice: Product or corporate names may be trademarks or 
registered trademarks, and are used only for identification and 
explanation without intent to infringe.
Library of Congress Cataloging in Publication Data
Bodea, Tudor.
Segmentation, revenue management and pricing analytics / 
Tudor Bodea & Mark Ferguson.
pages cm
Includes bibliographical references and index.
1. Revenue management. 2. Pricing. 3. Market segmentation. 
I. Ferguson, Mark, 1969– II. Title. 
HD60.7.B63 2013
658.15'54—dc23
2013039078
ISBN: 978–0–415–89832–4 (hbk)
ISBN: 978–0–415–89833–1 (pbk)
ISBN: 978–0–203–80215–1 (ebk)
Typeset in Minion 
by Swales & Willis Ltd, Exeter, Devon

---

## Page 6

CONTENTS
List of figures vi
List of tables viii
Acknowledgments x
Chapter 1 The Ideas Behind Customer Segmentation 1
Chapter 2 Forecasting 8
Chapter 3 Promotion Forecasting 47
Chapter 4 Capacity-Based Revenue Management 77
Chapter 5 Unconstraining 98
Chapter 6 Pricing Analytics 136
Chapter 7 Dynamic and Markdown Pricing 167
Chapter 8 Pricing in Business-to-Business Environments 186
Chapter 9 Customer Behavior Aspects of Pricing 212
Appendix A Dichotomous Logistic Regression 220
Appendix B Advanced Analytics Using R 228
Index 251
v

---

## Page 7

LIST OF FIGURES
2.1 Measuring Forecast Accuracy 17
2.2 Illustration of the Role of Holdout Samples 19
2.3 Simple Moving Average 20
2.4 Weighted Moving Average 22
2.5 Simple Exponential Smoothing 28
2.6 Double Exponential Smoothing 31
2.7 Additive and Multiplicative Seasonality  34
2.8 Triple Exponential Smoothing 36
2.9 Triple Exponential Smoothing—Initialization of S
0 and T0 39
2.10 Sales of SPSS Manual (2nd Edition) 40
2.11 Sales of SPSS Manual (2nd Edition)—One-Step-Ahead Forecasts 42
2.12 Sales of SPSS Manual (2nd Edition)—1983 Forecasts 44
3.1 Illustration of the Deviations in the Linear Regression Analysis 50
3.2 Estimation of Regression Coefficients via the Least Squares Method 50
3.3 Daily Sales of Ice Cream and Daily Average Temperatures 52
3.4 Trendline Option in Excel 52
3.5 Ice Cream Sales with Trendline 53
3.6 Data Analysis Menu 54
3.7 Regression Pop-up Box 55
3.8 Output of the Linear Regression on the Ice Cream Sales 56
3.9 Illustration of the Maximum Likelihood Estimation Mechanism 57
3.10 Estimation of the Linear Regression Model via Maximum Likelihood 59
3.11 Ice Cream Sales with Promotional Flyer Variable Included 61
3.12 Regression Output with Promotional Flyer Variable Included 61
3.13 Promotion History for a Staple Fashion Item 69
3.14 Sales and Price Plots: Quick Quaker Oats at River Forest Store 71
4.1 Normal Distribution Curve 81
4.2 Protection Level and Booking Limit in a Hotel Context 86
4.3 Nested Fare Class Buckets 88
vi

---

## Page 8

Figures  vii
4.4 Flowchart of Bid Price Revenue Management Logic 93
4.5 Linear Programming Formulation of Revenue Management Problem in 
Excel 94
4.6 Solution Report to the Linear Programming Formulation  95
4.7 Solution Report After Total Capacity is Set to Ten Rooms 96
5.1 Royal Hotel Business Booking Curves  100
5.2 Product Availability Progression in an Online Environment 102
5.3 Out-of-Stock Rates for the Sampled Style/Color/Size Items 104
5.4 In-Store Item Availability Measures 105
5.5 Tocher’s Inverse and Inverse Gumbel Cumulative Distribution Functions 114
5.6 Illustration of Demand Unconstraining via Double Exponential Smoothing 120
5.7 Demand Unconstraining via Double Exponential Smoothing 122
5.8 PD E -like Step vs. EM E -Step 129
6.1 The Pricing Analytics Process 138
6.2 Linear Price-Response Function 140
6.3 Uniform WTP Distribution 141
6.4 Density of Demand at Price p from a Uniform WTP Distribution 142
6.5 Density of Demand at Price p from a Normal WTP Distribution 142
6.6 Linear Price-Response Function 143
6.7 Constant-Elasticity Price-Response Functions  144
6.8 Reverse S-Shaped Price-Response Function 144
6.9 Power Price-Response Function 145
6.10 Nonlinear Price-Response Function 147
6.11 Estimated Price Elasticities for Various Goods (Absolute Values) 149
6.12 Profit as a Function of Price 150
6.13 Developing Pricing Capabilities: Process Roadmap 154
6.14 Price-Response Functions and Elasticity Curves 159
7.1 Price-Dependent Demand Profiles 183
8.1 (A) Historical Demand Data for Customized Pricing, (B) Fitted Reverse 
S-Shaped Probability Function to Win/Loss Data 189
8.2 (A) Marginal Deal Contribution vs. Unit Price, (B) Win Probability vs. 
Unit Price, (C) Expected Profit vs. Unit Price 191
8.3 Online Auto Lender—CHAID Decision Tree 198
8.4 Online Auto Lender—CHAID Logit Bid-Response Functions 200
8.5 Online Auto Lender—Logistic Regression Tree 205
8.6 Auto Online Lender—Bid-Response Functions and Expected Profit 
Functions for a Holdout Sample Auto Loan Application 209
9.1 Changes in Consumer Utility as Explained by Prospect Theory 216
A.1 (A) Fitted Line for the Linear Regression Model (B) Fitted Curve for the 
Logistic Regression Model 222
A.2 (A) Fitted Line for the Linear Regression Model (B) Variance Plot 223
A.3 Residual Plot 223
B.1 Sales Forecasting at Company X 246
B.2 Price-Response Function, Profit Function and the Optimal Price 248

---

## Page 9

LIST OF TABLES
2.1 Summary of Forecasting Accuracy Measures 17
2.2 Simple Moving Average 21
2.3 Weighted Moving Average 23
2.4 In-Sample Forecasting Accuracy Measures—SMA(5) 24
2.5 Summary of Forecasting Accuracy Measures  25
2.6 In-Sample Forecasting Accuracy Measures—Simple Exponential Smoothing 29
2.7 In-Sample Forecasting Accuracy Measures—Double Exponential Smoothing 32
2.8 Triple Exponential Smoothing—Initialization of Seasonal Parameters 37
2.9 In-Sample Forecasting Accuracy Measures—Triple Exponential Smoothing 38
2.10 Sales of SPSS Manual (2nd Edition)—Smoothing Parameters and 
Forecasting Accuracy Measures 42
2.11 Sales of SPSS Manual (2nd Edition)—1983 Forecasts 43
3.1 Illustration of the Maximum Likelihood Estimation Mechanism 58
3.2 Promotion Planning and Optimization 64
3.3 Additive and Multiplicative Promotion Models 66
3.4 Promotion History for a Staple Fashion Item 68
3.5 Summary Statistics and Model Fit 69
3.6 Log-Transformed and Original Multiplicative Models (Full Model) 74
3.7 Log-Transformed and Original Multiplicative Models (Reduced Model) 74
4.1 Demand Distribution 78
4.2 Expected Profit Calculation for an Order Quantity of 200 bagels 79
4.3 Expected Profits for Each Order Quantity Option 80
4.4 Standard Normal Distribution Table 82
4.5 Fare Class Prices and Distribution Parameter Values 88
4.6 Nested Protection Levels Calculated Using EMSR-b 92
5.1 Daily Sales of Pain de Boulogne at an Albert Heijn Store 107
5.2 Product-Limit Method Applied to the Pain de Boulogne Data 108
5.3 Hourly Sales Rates (Units/Hour) of Pain de Boulogne 109
5.4 Hourly Sales Rates to Cumulative Sales Ratios 111
viii

---

## Page 10

5.5 Cumulative Hourly Sales and Unconstrained Demand 112
5.6 Cumulative Demand Distribution Function 113
5.7 Parameter Estimates for Tocher’s Inverse Cumulative Demand Distribution 
Function 114
5.8 Parameter Estimates for the Gumbel Cumulative Demand Distribution 
Function 115
5.9 Operationalization of Averaging Method for Demand Unconstraining 118
5.10 Demand Unconstraining via Averaging Method (AM) 119
5.11 Demand Unconstraining via Double Exponential Smoothing (DES) 121
5.12 Operationalization of the EM Algorithm for Demand Unconstraining 127
5.13 Demand Unconstraining via the EM Algorithm 128
5.14 Operationalization of the PD Method for Demand Unconstraining 132
5.15 Demand Unconstraining via the PD Method 133
6.1 Price-Response Functions 146
6.2 Estimated Price Elasticities at the Industry and Brand Level 148
6.3 Estimated Price Elasticities for Various Goods 148
6.4 Types of Data Used to Make Pricing Decisions 153
6.5 Online Price Experiment Results 158
6.6 Linear Price-Response Function 160
6.7 In-Store Price Experiment Results 160
6.8 Constant-Elasticity Price-Response Model 161
6.9 Customer Survey Results 162
6.10 Logit Price-Response Function 163
7.1 Critical Ratio 
σ (.)for Assessing the Economic Viability of Price Markdowns 178
7.2 Product Group Demand Analysis 181
7.3 Preseason Optimal Markdown Policies 184
8.1 Output From Logistic Regression on Alpha’s Historical Win/Loss Data 193
8.2 Output From Logistic Regression After Removing Quantity 193
8.3 Bid Characteristics 194
8.4 Online Auto Lender—Data Dictionary 197
8.5 Online Auto Lender—CHAID Logit Bid-Response Functions 199
8.6 Online Auto Lender—Logistic Regression Results 203
8.7 Online Auto Lender—Behavioral Interpretation of the Δ Rate Interaction 
Effects 204
8.8 Online Auto Lender—Logistic Regression Tree Bid-Response Functions 206
8.9 Online Auto Lender—Behavioral Interpretation of the APR Effects 207
8.10 Online Auto Lender—Characteristics of a Holdout Sample Auto Loan  208
8.11 Online Auto Lender—Bid-Response Functions and Expected Profit 
Functions for a Holdout Sample Auto Loan Application 209
A.1 Dichotomous Logistic Regression Model 225
B.1 Model Selection Using Forecast Accuracy Measures 245
B.2 Long-Term Forecasts and Prediction Intervals 247
B.3 Product-Level Optimal Prices and Expected Profits 248
Tables  ix

---

## Page 11

ACKNOWLEDGMENTS
I would like to thank the following people and organizations for their contributions to 
the making of this book: David Parker, founder and former publisher at Business Expert 
Press, and John Szilagyi, former publisher at Routledge Publishing—thank you for your 
patience and continued support; Loren Williams, executive director, Advisory Services 
at Ernst & Young—thank you for making sure that the book content remained relevant 
and anchored into reality; InterContinental Hotels Group, Predictix, LLC and Univer-
sity of Groningen, the Netherlands—thank you for allowing me to learn from and work 
with some of the most respected professionals in the revenue management field. Last but 
not least, special thanks go to my family—I have become who I am because of you. 
Tudor Bodea
Much of the credit for the thinking and material presented in this book goes to the excel-
lent colleagues and students that I have been very lucky to work with over the years. 
Special thanks goes to my wife Kathy and two daughters, Gracie and Tate, for their love 
and support. Any omissions or errors are my own.
Mark Ferguson
x

---

## Page 12

1
THE IDEAS BEHIND CUSTOMER SEGMENTATION
The practices of Revenue Management and Pricing Analytics use historical sales data to 
analytically estimate demand forecasts that are then used in optimization models to set 
and update capacity (or prices) offered through various channels to specific customer 
segments in order to maximize profit. A familiar example is the passenger airline indus-
try, where a carrier may sell the same type of seats (e.g., coach) on the same flight to 
different customer segments (typically business and leisure travelers) at different prices. 
These practices have transformed the transportation and hospitality industries and are 
increasingly important in industries as diverse as retail, telecommunications, banking, 
health care, and manufacturing. While capacity-constrained industries such as airlines 
and hotels typically optimize on the capacity to make available to each customer seg-
ment, price optimization is more frequently used for less capacity-constrained indus-
tries such as retailing and banking. The key denominator for successful implementations 
of either a revenue management or pricing analytics solution is a customer population 
that is diverse (at some level) in how different groups of customers value a company’s 
products. The process of identifying these different groups of customers is commonly 
referred to as customer segmentation.
To better understand the idea behind customer segmentation, consider your own 
buying behavior. If someone asked you what is the maximum price that you would be 
willing to pay for a bottle of your favorite brand of purified water, it is unlikely that you 
would give a price more than $1. We are unlikely to assign a higher value to the bottle 
of water because we know of many retail outlets where we can purchase this product in 
bulk, most likely at a per bottle price that is significantly less than $1. If someone could 
magically search our entire buying history, however, he or she would probably find 
instances where we have paid much more than $1 for a bottle of water (ball games, fancy 
restaurants, and hotel mini-bars to name just a few). We are still the same person with 
the same valuations, yet we purchase the same product at very different prices depending 
on the time and location when the purchase is made. Even though it is the same person 
who may not pay more than $0.20 for a bottle of water at a grocery store and then pays 
1

---

## Page 13

2  The Ideas Behind Customer Segmentation
$4 for the same brand bottle of water at a restaurant, he or she is considered to belong to 
two different segments of customers, depending on the time and location where the pur-
chase is made. The customer at the grocery store is typically buying in bulk and primarily 
concerned with meeting their basic needs, while the customer at the fancy restaurant is 
buying a luxury experience and no alternatives are easily available. Thus, it would be 
a very costly mistake to use the same customer pricing policy in all of the distribution 
channels as a $4 price per bottle will not sell in a grocery store while a $0.20 per bottle 
price will leave unrealized revenue at a fancy restaurant.
In the example above, the products were sold at two completely different locations 
so an argument can be made that the price difference is purely due to cost; the cost of 
supplying the product to the grocery store is much less expensive than the cost of supply-
ing the product to the fancy restaurant. This argument has some truth as there is some 
difference in distribution costs to the two locations, although it is very unlikely that the 
difference is large enough to justify such an extreme price difference. A follow-up ques-
tion is then: Are there cases where customers pay very different prices for the same exact 
product at the same exact location? In fact, there are many examples where this is the 
case. It is a high probability that two people sitting beside each other on an airplane paid 
significantly different prices for their fares (business/leisure-based segmentation). It is 
also common practice for two different customers purchasing the exact same make and 
model car from the same dealership to have paid different prices (informed consumer-
based segmentation) or for men and women to pay different cover charges to enter the 
same popular night club at the same time (gender-based segmentation). Student dis-
count rates at some tourist attractions and senior discounts at some retailers and restau-
rants (membership- or age-based segmentation) are other examples.
Once you start looking for it, you will notice that segmentation-based pricing is prac-
tically everywhere, as it has been since the very beginning of human commerce. While 
there may be debates on which of these practices is ethical, or even legal in some cases, 
most consumers have come to accept a certain degree of segmentation-based pricing as 
a fact of life. We will cover the aspect of segmentation-based pricing that is more or less 
acceptable to customers in a latter chapter. For now, our focus is on identifying these 
different segments and designing products that are targeted for each one.
CUSTOMER SEGMENTATION VERSUS PRODUCT SEGMENTATION
The two major (but nonexclusive) segmentation strategies are customer based and prod-
uct based. Customer-based segmentation is when a firm offers exactly the same product to 
two or more different customers at different prices, based on certain customer attributes 
such as age, gender, or nationality. Ladies’ night at a club and senior discounts for a meal 
are examples of customer-based segmentation. While there does not appear to be any 
legal issues with these types of segmentation schemes, legal issues may arise if there is 
any perception that customers are segmented based on more sensitive attributes such as 
race or physical disabilities (imagine the public reaction to a surcharge for blind people, 
for example). While race-based segmentation is illegal in many countries, nationality is 
sometimes used. One of the authors experienced this first hand when attempting to rent 
a car in Spain. When the author’s U.S. address was entered on the car rental company’s 
website, a much higher price was quoted than when the address of the local hotel was 
entered. While customer-based segmentation is common, it typically places major limi-

---

## Page 14

The Ideas Behind Customer Segmentation  3
tations on how refined you can make your segments. A senior discount, for example, 
does not differentiate between a very affluent (and less price sensitive) older tourist and 
a less affluent (and very price sensitive) retiree who is barely getting by. To achieve this 
level of segmentation, firms typically have to move to product-based segmentation.
Product-based segmentation involves creating either superior or inferior versions 
of a product so that each version can be priced differently but that cannibalization of 
sales from the higher priced versions to the lower priced versions is minimized. The 
latter is the most critical part for successful product-based segmentation, as there needs 
to be some incentives or restrictions to keep the higher willingness-to-pay customers 
from purchasing the lower priced versions of the product. Customer acceptance of these 
restrictions is typically higher when the version choice is a conscious decision of the cus-
tomer rather than a true restriction on a particular class of customer from purchasing a 
particular version of the product.
It should be noted that different versions of a product do not necessarily mean actual 
physical differences in the product. For segmentation purposes, the exact same seat on 
an airline flight can be sold as different products; either a fully refundable or a nonre-
fundable ticket for example. Here, airlines create inferior versions of their base product 
(a fully refundable no advance purchase airline seat), placing various levels of restric-
tions on it. This allows the airlines to charge lower prices to their more price-sensitive 
customer segments while still having a “fence” in place to keep their less price-sensitive 
customers from paying the lower prices. In the case of airline tickets, business travel-
ers are typically less price sensitive than leisure travelers (as business travelers are typi-
cally reimbursed for their travel expenses through their employer). The restriction here 
for the lower priced version of the product is that it is nonrefundable and/or has an 
advance purchase requirement. Since business travelers often have to make last-minute 
travel decisions (or, changes in their current travel plans), they often self-select the more 
expensive airline tickets. This versioning practice is typically accepted by the business 
travelers because they are not excluded from purchasing the lower-priced (and more 
restricted) versions of the airline tickets. The science behind the allocation of these dif-
ferent product versions to their respective customer segments is discussed in Chapter 4.
Compare the product versioning practice of the airlines to those of the previously 
mentioned rental car company in Spain that charges native Spanish residents lower 
prices than customers from other countries. Most foreign visitors would be upset if they 
knew that they were paying a significantly higher price, for exactly the same service, than 
native residents. To try to diminish this customer dissatisfaction, the rental car company 
only provides the final price once a customer puts in their credit card address informa-
tion, thus minimizing the likelihood that the customers will observe the differential pric-
ing. This practice of trying to hide or disguise the final prices is also a common practice 
of auto dealerships and repair shops, which frequently rank very low in cross-industry 
customer satisfaction surveys.
We are not claiming by any means that all customers are happy with the airlines’ 
current pricing practices. As a general rule, customers commonly feel dissatisfied when 
they learn that they are paying more for what they perceive to be the same product than 
another customer. Businesses (the ones actually paying the travel bills) often revolt when 
they feel that the airline price differentials become excessive, slashing travel budgets and 
encouraging their employees to meet via tele-presence. This dissatisfaction has been 
successfully exploited by the “low-cost” airlines that have entered the industry over the

---

## Page 15

4  The Ideas Behind Customer Segmentation
last 30 years. Many of the low-cost airlines advertise their “simpler” fare structures and 
lighter restrictions on purchasing the lower fare classes. Thus, as in any market, there 
are constant price adjustments taking place as the airlines try to find the prices that best 
match supply with demand. Despite the frequent complaints, however, most leisure 
travelers are happy to give up some travel flexibility for an (often) lower total cost ticket 
price while most business travelers appreciate the ability to find seats still available for 
last-minute flight changes. Examples of product-based segmentation methods outside of 
the airline industry are provided in the next section.
EXAMPLES OF PRODUCT-BASED SEGMENTATION
Recall that the most successful product-based segmentation schemes often involve 
restrictions placed on a product to create inferior versions of the product where the cus-
tomers self-select which version (and thus price) they want. You may already be familiar 
with how this practice works in an industry that has an expiring capacity such as airlines 
(once a plane leaves with an empty seat, the opportunity to sell that seat on that flight 
is lost forever), but how is it practiced in industries without expiring capacity? Exam-
ples abound, especially in the retail sector. At first glance, retail products appear to have 
opposite characteristics than do products in the travel industry: a retail product tends 
to depreciate in value as it sits on a shelf while a travel product tends to appreciate in 
value as the time of consumption approaches. Thus, the common revenue management 
practices of reserving capacity for higher paying (and later arriving) customers cannot be 
directly applied in the retail sector. In its place is a myriad of methods designed to offer 
customer segment specific prices for what is, essentially, the same product. Some of the 
more common methods are listed below.
1. Seasonal time-based pricing.
2. Package-based pricing.
3. Channel-based pricing.
4. Coupons, mail-in rebates, and promotion codes. 
Seasonal time-based pricing refers to when a retailer sells a seasonal product at a list price 
at the beginning of the season and then discounts or “marks-down” the product’s price 
as the season progresses. This practice is very common in the apparel retail sector, where 
a winter coat that was priced at $200 in September may be marked down to $80 the fol-
lowing March. While this practice is sometimes simply an act by the retailer to make up 
for an ordering mistake (perhaps the coat was assorted in a very unpopular color), it is 
often a conscious decision by the retailer to exploit two different customer segments. 
The customer segmentation that occurs here is between the highly fashion-conscious 
customers who gain a lot of satisfaction from wearing the latest fashions in the season 
that the fashions are first introduced and the less fashion-conscious customers who are 
willing to trade-off a slightly out-of-fashion garment (a coat bought at the end of the 
current season will mostly be worn the following winter) for a lower price. The practice 
of markdown pricing is described in Chapter 7.
Package-based pricing is a broad term that refers to several segmentation strategies in 
the consumer goods industry. One strategy is to simply package the product in differ-
ent sizes, with the smaller package typically commanding the higher per-unit price. In

---

## Page 16

The Ideas Behind Customer Segmentation  5
the bottled water example at the beginning of this chapter, a gallon-sized bottle of water 
typically sells for a lower price per ounce than does a 20 ounce bottle of the same brand. 
While there are typically economies of scale and a reduction in per-unit packaging cost 
for larger quantity package sizes, these cost savings rarely explain the full price differ-
ential between the two package sizes. Thus, this pricing strategy is intended to segment 
customers who are looking for an immediate and convenient package size from the cus-
tomers who are looking to meet the needs of themselves (and perhaps others) over a 
longer span of time. This same reasoning applies when the packaging involves the aggre-
gation of multiple units of the same size (i.e. bulk purchases). A 25-pack of 20 ounce bot-
tles, for example, is priced at a lower per-bottle price than an individual 20 ounce bottle 
(see Chapter 8 for an example where customers are segmented based on the quantity size 
they purchase in a B2B environment).
Channel-based pricing refers to the differential pricing of the same product depend-
ing on which channel the product is sold through. Referring back to the bottled water 
example, a bottle of water sold by a vendor in the stands at a sporting event is a different 
product (by our definition) than the same brand bottle of water sold at a grocery store. 
The segmentation in this case is mainly driven by the amount of alternative options 
available to the buyer at the time of purchase. A buyer considering a purchase in a gro-
cery store may have many alternative beverages easily available to them, as well as a 
number of alternative grocery stores to shop from. Thus, a large price increase of a par-
ticular brand of bottled water will result in many consumers switching to another brand 
of bottled water, to some other type of beverage, or even to deferring their purchase until 
they can purchase their preferred brand of water at another retail location. Compare this 
scenario to the pricing of bottled water at a stadium during a sporting event. The owner 
of the stadium typically operates as a local monopoly of all concessions, controlling the 
pricing of all beverages that are sold there. Thus, the availability to the consumer of 
significantly lower priced options is very limited in this situation. This is the reason we 
typically see much higher per-unit prices for products sold in restaurants, theatres, and 
theme parks; or basically anywhere a localized monopoly can control the availability of 
outside alternatives.
While it is typically easy to identify the channel-based pricing opportunities described 
in the examples above, there are many other channel-based pricing opportunities that are 
less understood. Internet retail sales is an example of an area where companies are still 
struggling to understand exactly what customer segment this buying sub-population rep-
resents. On the one hand, the internet makes it extremely easy to price comparison shop 
compared to when consumers had to physically travel to different retail locations to com-
pare prices. On the other hand, active users of the internet typically have higher discre-
tionary income than do consumers who do not have home access to high-speed internet 
service. Thus, an argument can be made that internet shoppers are less price sensitive than 
noninternet shoppers. When internet retail sales was still in its infancy, there were several 
notable pronouncements that the increased price transparency of the internet would lead, 
within a few years, to only a few dominant internet retailers who would basically charge 
the same price as the other major retailers for all of the products they sold. A quick search 
on almost any product today, however, shows that there still exists a wide variety of inter-
net retailers selling a product along with a wide variety of selling prices between them. 
Thus, it is now becoming clear that attempts to group all internet buyers into a single 
purchasing behavior segment is misguided and a more nuanced approach is needed.

---

## Page 17

6  The Ideas Behind Customer Segmentation
Some firms who primarily advertise their prices on the internet (where the search cost 
is low) have found that using a portfolio of pricing strategies can significantly increase 
profits. Rental car companies are a good example of this group, as they typically price 
their base daily rental rates very competitively and, subsequently, command very low 
margins on actually renting their cars. One reason could be that the search cost is very 
low for this industry, as most customers use a third-party search engine such as Expedia 
or Travelocity to compare the daily prices of all the available rental companies for a par-
ticular location. After a customer has reserved a car and is picking it up at the rental car 
counter, however, he or she is often encouraged to buy extras such as insurance, pre-paid 
gas or GPS units. Since the search cost for these products is much higher (the customer 
is already at the counter), the corresponding margins on the products are much higher 
as well.
The last of the common segmentation-based pricing strategies involves the use of 
effort-based discounts such as coupons, mail-in rebates or promotion codes. The con-
sumers segmented through this strategy are the group who are willing to take the time 
and effort (and have the organizational skills) required to claim the discount versus 
those who do not. The use of coupons seems to be more popular for lower-priced prod-
ucts sold in grocery and convenience stores while mail-in rebates are more popular for 
higher-priced items such as consumer electronics. In internet retailing, promotion codes 
appear to be the most popular way to employ this strategy, as a way to offer lower prices 
to customers who are more price-sensitive and willing to search for these codes. We dis-
cuss aspects of this type of pricing in Chapter 3.
MAJOR CHALLENGES OF PRODUCT-BASED SEGMENTATION
An advantage of customer-based segmentation versus product-based segmentation is 
that it is typically easier to identify which consumers belong to each segment. Simply 
checking the birthdate on a person’s driver’s license, for example, can confirm whether 
or not the person is eligible for a senior discount. As previously discussed, however, 
product-based segmentation has a lot of advantages over customer-based segmentation, 
and is typically worth the additional effort required to identify the micro-segments and 
build versions of the product specifically designed for each segment.
THE DAWN OF BIG DATA AND BUSINESS ANALYTICS
The majority of the segmentation categories and methods discussed so far have been 
around for at least the last 20 years. The science in this area has been re-energized recently, 
however, with the emergence of Big Data and Business Analytics. Big Data describes the 
vast amount of unstructured data depicting customer preferences that has just recently 
become available from social network sources such as Facebook, Twitter, and, from 
customer web search history. The availability of this type of data combined with an expo-
nential increase in computing power provides new opportunities for categorizing cus-
tomers into more refined segments. In addition, the econometric and data mining tools 
have also had significant advances in recent years. The science of applying these tools to 
the new opportunities provided by Big Data is commonly termed Business Analytics. 
Business Analytics can be characterized into three different categories:

---

## Page 18

The Ideas Behind Customer Segmentation  7
1. Descriptive Analytics.
2. Predictive Analytics.
3. Prescriptive Analytics.
Descriptive analytics involves the science of identifying different customer segments such 
as the ones described in this chapter. While this practice remains challenging, it is the 
area where the most advances have already been made and represents the most prevalent 
uses of business analytics in practice. A simple way of thinking about descriptive analyt-
ics is as a way of better understanding who your customers are. It allows firms to think of 
their customer base as a combination of many micro-segments, so as to design targeted 
products and advertising programs for each segment.
Predictive analytics is closely related to descriptive analytics except for the main objec-
tive, which is to predict customer demand or their reactions to a set of marketing expo-
sures. Time series forecasting, where past demand data are extrapolated into the future 
using statistical techniques, is a subset of predictive analytics. Time series forecasting is 
discussed in Chapter 2. Prescriptive analytics goes beyond time series forecasting, how-
ever, to include causal variables such as price, promotions, weather, economic condi-
tions, and other possible predictive variables. Both predictive and prescriptive analytics 
often rely on econometric techniques such as regression analysis, so it is sometimes con-
fusing to distinguish the two. A simple way to differentiate between the two is the follow-
ing. If your end goal is simply to make better predictions without a need to understand 
the causal reasons for the outcomes, then you are employing prescriptive analytics. On 
the other hand, if you are more concerned with understanding the underlying causes 
of some outcome (such as sales), then you are employing prescriptive analytics. From a 
slightly more technical standpoint, predictive analytics involves studying the significance 
of the possible explanatory variables in a regression model while predictive analytics is 
only concerned about the predictive accuracy of the model. Both predictive and pre-
scriptive analytics methods, as they relate to pricing and promotion, are discussed are 
discussed in Chapters 3, 7 and 8.
Prescriptive analytics describes the science of using the forecast provided by predic-
tive analytics in an optimization model to guide firms on how to set prices or allocate 
capacity so as to achieve some objective such as maximizing profits or market share. In 
capacity-based revenue management (described in Chapter 4), the objective is to save 
expiring capacity such as an airline seat for latter arriving segments who are willing to 
pay more for the product. In pricing analytics (described in Chapters 6, 7 and 8), the 
objective is to set prices or target promotions so as to maximize the firm’s overall profits. 
Prescriptive analytics, as with most business tools, starts with a forecast—the topic of the 
next chapter.

---

## Page 19

2
FORECASTING
INTRODUCTION
Many organizations operate in uncertain business environments. Without proper 
insights into what their short- and long-term outlook may look like, these organizations 
could make unfit decisions and become liabilities. Thus, acquiring and employing intel-
ligence on likely future business developments should be of concern to all those who 
proactively pursue profitability and competitiveness. In this context, when employing 
the science of forecasting, firms attempt to answer questions such as: How much revenue 
is the company expected to generate by the end of the quarter/year? How much demand 
should my hotel expect to see on New Year’s Eve? How many winter jackets should I 
order in anticipation of the demand expected to materialize during the cold season? 
What is the likely performance of our new fashion line three months after the launch? 
Or, will investments in a major convention center in Alpharetta, GA repay in 15 years? 
Whether by using historical transaction data or eliciting experts’ opinion, forecasting is 
used to assist professionals at all decision levels make the most informed decisions in the 
particular environment in which they compete.
Since its inception as a discipline in the early 1950s, forecasting has often been cited 
by organizations as a critical business enabler. In the airline industry, for example, Con-
tinental Airlines Cargo, a division of Continental Airlines, reported that its efforts to 
increase its demand forecast accuracy by 10% led to a 2.5% improvement in the bottom-
line revenue, or, equivalently, more than $1 million incremental annual revenues (JDA 
Software Group, 2007). In the same industry, America West Airlines, which merged with 
US Airways Group in 2005, credited its completely redesigned forecast of the demand for 
reserve crews with savings for the company totaling several million dollars (SAS Institute 
Inc., 2009). In the hospitality industry, Carlson Hotels made significant investments in 
advanced forecasting capabilities to help its hotels make better revenue decisions and 
be more profitable (Rozell, 2007). In manufacturing, Procter & Gamble’s decision to 
revamp its short-term demand forecasting led to a 30% increase in the forecast accuracy 
8

---

## Page 20

Forecasting  9
and a 10% decrease of its safety stock inventories (Moad, 2008). Similarly, in an effort to 
improve their performance through collaboration and alignment, Sara Lee Corporation 
and Wal-Mart formalized and developed integrated sales forecasting processes (Seifert, 
2003). In the same vein, to help its first-tier suppliers make sound inventory decisions, 
Dell provides them with demand forecasts every month (Kapuscinski, Zhang, Carbon-
neau, Moore, & Reeves, 2004).
These success stories illustrate the impact forecasting has had on the operations of 
established organizations. By no means, however, does this mean that small businesses 
that operate in the same or other industries could not benefit from the use of the fore-
casting concepts. It is our belief that the outcome of any process that is to a certain extent 
time dependent and surrounded by uncertainty can be improved by better forecasting 
practices. To this end, however, a question often asked by business owners and adminis-
trators alike relates to what an initiative that involves forecasting should employ in order 
for it to be successful. In this context, while the choice of a particular forecasting method 
is critical (e.g., judgmental forecasts vs. extrapolation methods vs. econometric models), 
the design and the execution of the initiative’s auxiliary components are important to the 
point that they cannot be overlooked. In particular, the objectives of the initiative need 
to be transparent and have the support of the leadership team. For style and seasonal 
goods retailers, for example, forecasting sales at the chain/product-category level typi-
cally requires less of an effort than forecasting sales for a staple/fashion item at the store/
style/color level. Hence, the two situations would command different sets of objectives 
and require differentiated levels of upper management support. Furthermore, the data 
to support these objectives are needed. Whether collected internally (e.g., own sales data, 
internal expert opinions) or gathered through third-party intermediaries (e.g., aggre-
gate hotel sales data for direct competitors shopped through, e.g., Rubicon, a Travelclick 
company), these data should be centrally stored and made available to a wide audience 
of users from within the organization. Finally, since it is rare that forecasting happens in 
isolation, the links that support the deployment of the forecasts to downstream systems 
and/or processes need to be designed flexibly enough to allow for future developments. 
In a closed-loop pricing system, for example, provisions for manual intervention must 
exist to facilitate super users’ access to forecasting override capabilities.
Almost all initiatives that target specific business goals require some type of forecast-
ing. Often, if not always, the performance of these initiatives depends on the accuracy 
of the corresponding forecasts. Although it is often difficult to quantify the financial 
returns associated with the use of improved forecasts, a general consensus exists that 
better forecasts lead to better outcomes (Cooper, Homem-de-Mello, & Kleywegt, 2006; 
Weatherford, 1997; Weatherford & Belobaba, 2002). To this end, in what follows, we 
focus our discussion on how forecasts are produced and how their accuracy is assessed. 
We provide insights into the latter of these points because companies typically down-
play the importance of measuring the uncertainty in their forecasts and consistently fail 
to account for it (see, e.g. Fisher, Hammond, Obermeyer, & Raman, 1994). This being 
said, it is not our intention to exhaustively review these topics. We also do not discuss at 
length the critical steps that precede or follow the forecasting activities (e.g., data sources, 
data quality, level of aggregation, forecast usage). For these and other similar issues, the 
reader is referred to standard textbooks such as Makridakis, Wheelwright, & Hynd-
man (1998), Bowerman, O’Connell, & Koehler (2004) and Hyndman, Koehler, Ord, & 
Snyder (2008).

---

## Page 21

10  Forecasting
THEORY OF FORECASTING
Typically, forecasts are the end result of qualitative, quantitative or a combination of 
qualitative and quantitative work. Often, when historical data do not exist (e.g., at the 
time Toyota introduced Prius, the first mass-produced hybrid electric vehicle, little 
was known about its future demand) or are considered irrelevant for future develop-
ments (e.g., the 9/11 tragic events in 2001 completely changed established travel pat-
terns in the United States), qualitative forecasts are employed. These are a reflection of 
a sound process of expert opinion engagement. Whenever the need arises, experts in 
relevant fields are asked in centralized or decentralized settings to provide their advice 
on where things may go in the future given their present state. At first, likely future 
developments are outlined by experts. These are subsequently reviewed by the group 
who then recommends a forecast based on the agreement reached by its members. In 
many business settings, however, the consensus forecasts have proven to be unrea-
sonably influenced by the dominant members of the group. In fashion retailing, for 
example, members of the leadership team involved in merchandise buying may inad-
vertently impact the individual decisions of the buying committee associates such that 
too much or too little product gets purchased (for relevant examples, see Fisher et al., 
1994; Fisher & Raman, 2010). Some of the methods on which the qualitative forecasts 
are based are discussed in Linstone & Turoff (2002) and Kahn (2006). Further details 
about judgmental biases and ways to address them are discussed in Makridakis et al. 
(1998).
In contrast to the intuition and experience-based approach promoted by qualitative 
forecasts, quantitative forecasts are data driven. Usually, explanatory and/or extrapola-
tive techniques are employed to compute these forecasts. Explanatory models assume 
that a relationship exists between the forecast entity and some other observed variables. 
Since the relationship is known explicitly, changes in forecasts due to changes in explan-
atory variables are predictable and accurate for as long as the underlying explanatory 
mechanism stays unchanged. Representative members of this class of models are linear 
and generalized linear regression models (for extensive reviews see, e.g., McCullagh & 
Nelder, 1989; and, Neter, Kutner, Nachtsheim, & Wasserman, 1999). To illustrate the 
use of such models, consider the problem of predicting the daily sales of frozen custard 
at one of Rita’s Ice Cream stores (www.ritasice.com). The relation between sales and 
(some) other explanatory variables can be formalized as:
 Sales
t = β0 + β1 . DATt + β2 . OOSt + β3 . St + β4 . DOWt + εt (2.1)
where t identifies the t th time dependent observation in the data set, DATt is the daily 
average temperature, OOSt indicates whether or not flavor or product out-of-stocks hap-
pened that day (Yes=0, No=1), St indicates the season (cold=0, hot=1), DOWt identifies 
the day of the week and εt is a random error term that incorporates the influence of all 
other variables that impact the sales but were omitted from the model. βk, 0 ≤ k ≤ 4, is a 
set of weights that measure the importance of the explanatory variables in describing the 
sales outcome. The estimation of the βk parameters through the means of linear regres-
sion models makes the relationship among the variables explicit. Hence, once the model 
has been estimated using historical data, the expected sales can be predicted for any pair 
of inputs (DAT
t, OOSt, St, DOWt). Explanatory modeling techniques are described fur-
ther in Chapter 3.

---

## Page 22

Forecasting  11
Extrapolative models, or, time series models, do not link the entity that needs to be 
forecast to any other explanatory variables. Instead, they predict the future state of a 
system using its past realizations and/or forecast errors. Thus, in such an environment, 
the what will happen takes precedence over the why it happens. While such an approach 
is always debatable, in certain contexts, it may be the only solution available. Oftentimes, 
for example, complex systems cannot be timely understood and explained through for-
mal relations. Similarly, at times, the explanatory variables themselves need to be pre-
dicted which may turn out to be as complex a task as forecasting the dependent variable 
itself. Thus, extrapolative models are an important component of the arsenal of forecast-
ing methods. These models include, but are not limited to, moving average and expo-
nential smoothing methods (Brown, 1963; Holt, 2004; Hooker, 1901; Winters, 1960; 
Yule, 1909) (discussed further in the next sections), autoregressive integrated moving-
average models (ARIMA) (Box & Jenkins, 1970; Box, Jenkins, & Reinsel, 2008), (innova-
tions) state space models (Hyndman, Koehler, Snyder, & Grose, 2002; Hyndman et al., 
2008), structural models (Harvey, 1989) and certain types of neural networks (Azoff, 
1994; McNelis, 2005). Returning to Rita’s ice cream store, if sales in the current period 
are hypothesized to strictly depend on sales from the previous period, the corresponding 
model, an ARIMA(1,0,0), could be formalized as:
 Sales
t = µ + ϕ . Salest-1 + εt (2.2)
where µ is a constant, ϕ is the parameter of the model (|ϕ| ≤ 1) and εt is a random error 
term that represents the unexplained portion of the variability in sales.
In isolation, explanatory and extrapolative models have been shown to perform con-
sistently well. To achieve better outcomes, however, the two methods can be unified in a 
single methodological framework intended to make the forecasts even more responsive. 
Called dynamic regression models in the social sciences (Pankratz, 1991), these methods 
build on the strengths of the underlying models to provide for superior returns. Certain 
types of neural networks have similar properties (Zhang, 2004). In Rita’s example, for 
instance, the sales forecasts could be expressed as:
 Sales
t = β0 + ϕ . Salest-1+ β1 . DATt + β2 . OOSt + β3 . St + β4 . DOWt + εt (2.3)
where the βk, 0 ≤ k ≤ 4, and ϕ parameters have the meaning discussed in equations (2.1) 
and (2.2). If the explanatory variables are treated as system disturbances, ϕ can be viewed 
then as a measure of how well the dependent variable Sales copes with the corresponding 
shocks. Small values for ϕ suggest that sales are fast to respond to environmental shocks 
such as the changes in the weather. The reverse is true if ϕ is large.
In the world of extrapolative models, researchers and industry practitioners alike tend 
to make a clear distinction between forecasting methods and models. Although through-
out the chapter these terms are used interchangeably, we detail the corresponding dif-
ferences next. Whenever opportune, we complement the exposition with other relevant 
insights. Simpler techniques such as moving average and exponential smoothing which 
primarily smooth the appearance of the original time series produce point forecasts. 
These estimates are intended to represent the true future values of the forecast measure 
but, in doing so, they fail to provide any insights into the uncertainty that surrounds

---

## Page 23

12  Forecasting
the forecasting process. Hence, they do not support the direct computation of predic-
tion intervals. Such techniques are often referred to as forecasting methods. In contrast, 
forecasting models provide, in addition to point forecasts, information on how accurate 
the forecasts are expected to be, that is, they allow for the computation of prediction 
intervals. In problems such as inventory planning this information is invaluable. For 
example, an expected demand of 25 units with standard deviations of 2 and 15 units, 
respectively, should lead to significantly different recommendations, at least, in terms 
of safety stocks. Classic forecasting models are ARIMA and (innovations) state space 
models. Since essentially all exponential smoothing methods have equivalent ARIMA 
or (innovations) state space models, the latter have been traditionally used to indirectly 
compute prediction intervals for the former (see, e.g., Chatfield & Yar, 1991; Gardner, 
2006; Hyndman, Koehler, Ord, & Snyder, 2005; Yar & Chatfield, 1990).
In practice, the selection of a forecasting technique or model appropriate for a specific 
application is approached through the use of forecasting accuracy measures. We discuss 
the most common of these measures in the next section.
FORECASTING ACCURACY MEASURES
Quantitative forecasts are intended to discover and predict data elements that are unlikely 
to change during a predefined time window. For example, demand levels, trends and 
seasonal patterns together with the corresponding correlations or autocorrelations are 
all data elements that, in certain contexts and at certain times, can be assumed constant. 
In addition, quantitative forecasts are used to characterize the inherent randomness that 
exists in the data and is not accounted for through the use of the systematic components 
such as the levels or the trends. Forecasting accuracy measures reflecting how well a 
forecasting method captures the systematic component (vs. the random component) of 
a data set can be employed to achieve two goals. First, during the model selection phase, 
they can be used to screen out forecasting methods that are not appropriate for particu-
lar sets of data. Second, once a given method is routinely used to produce forecasts, these 
measures can signal when a structural change occurs and the underlying model needs 
to be either refined or replaced. Thus, the specific objective calls for how the accuracy 
measures are computed and reported. On the one hand, if model selection is of impor-
tance, then accuracy measures are computed on an estimation sample and subsequently 
validated against those calculated on a holdout sample. Often, to avoid over fitting on 
both sides, the model with good and consistent performance on both samples is recom-
mended as the preferred one. On the other hand, if the interest lies in assessing the per-
formance of an existing forecasting method, then these measures are computed on the 
full sample and compared with similar historical estimates. Substantial departure from 
historical performance may indicate that the forecasting method is no longer appropri-
ate for the circumstances at hand. In the remainder of this section, we discuss how the 
forecasting accuracy measures are computed in the context of extrapolative models that 
use time series data to produce the forecasts. The approach, however, is easily transfer-
able to the case when the forecasts are produced by explanatory models or qualitative 
forecasting techniques.
Irrespective of the reasons why the forecasting accuracy measures are computed, their 
calculation makes use of the generic forecast error defined as e
t = Yt – Yˆ
t where Yt and Yˆ
t 
are the observed value and the forecast of the time series at time t. As before, the com-

---

## Page 24

Forecasting  13
putational context imposes the technique to use to estimate the forecasts  Yˆ
t. One could 
rely, for example, on forecasts for which the time origin changes but which maintain a 
similar forecast horizon. The one-step-ahead forecasts are representative of this class of 
forecasts and are employed when models are fitted on estimation samples or validated 
on holdout samples. In addition, one could compute the forecasts by fixing the time ori-
gin, say at period n, and, subsequently, producing the estimates for a series of consecu-
tive time instances n + h (h ≥ 1, h integer). This class of forecasts is often used on holdout 
samples. The standard process implemented to generate forecasts for future time periods 
also follows this latter approach. As an aside, when these forecasts are produced, they are 
based on the full data set, that is, the set that combines the estimation and the holdout 
samples.
The calculation of the forecasting accuracy measures is independent of the underlying 
process used to generate the forecasts. Thus, computing the forecasting accuracy simply 
requires one to assess the relatedness of two streams of univariate data. In such a con-
text, the observed realizations Y
t of the time series are compared against the forecasts Yˆ
t 
which are considered known at the time of the procedural execution. At an abstract level, 
accuracy measures can be grouped into two distinct classes based on how they relate to 
the scale of the corresponding time series. Scale-dependent measures are often employed 
to compare the forecast performance of several forecasting techniques on a single time 
series. These metrics fail to serve their purpose when the performance over multiple time 
series is sought as the scale of the series may inadvertently impact the recommendations. 
In contrast, the scale-independent measures do not suffer from this bias. Depending on 
how they are computed, however, some scale-free metrics may at times be infinite, not 
defined, extremely skewed or perceived as favoring some errors over others. Irrespective 
of their scale association, several of the accuracy measures proposed in the forecasting 
literature are discussed in the next paragraphs.
Scale-Dependent Forecasting Accuracy Measures
The scale-dependent metrics are calculated using various transformations of the fore-
cast errors e
t. Since no standardization is involved, the scale-dependent measures have 
measurement units dependent on the units of the original time series data. Hence, these 
measures should only be used to assess the relative performance of competing forecast-
ing methods on a single time series. Extending the evaluation to multiple time series is 
controversial and, thus, not recommended (Chatfield, 1988). The most frequently cited 
scale-dependent metrics typically require the transformation of the forecast error using 
absolute value and squaring and are formally expressed as:
 
Mean Error 
Mean Absolute Error
ME n e
MAE n A
t
t
n
t
t
() =⋅
() =⋅
=
=
∑
1
1
1
111
2
1
1
1
n
t
t
n
t
t
n
n e
MSE n e
∑∑
∑
=⋅
() =⋅
=
=
Mean Squared Error
Root Meann Squared Error RMSE MSE() = ,
 (2.4)

---

## Page 25

14  Forecasting
where et = Yt – Yˆ
t is the forecast error, At = /H20895et /H20895 is the absolute error, et
2 is the squared error 
and n provides the number of observations for which forecasts have been computed.
Scale-Independent Forecasting Accuracy Measures
The scale-free measures intend to remove the dependency of the forecast accuracy on the 
measurement units of the time series data. While multiple such metrics have been rec-
ommended, they can all be grouped in four distinct subclasses. Of the measures encom-
passed by the percentage error subclass, the mean absolute percentage error (MAPE) is 
probably the one used the most. To compute the MAPE, the forecast errors e
t are scaled 
by the observed values of the time series, transformed using the absolute value, expressed 
in percentages and then averaged to lead to:
 Mean Absolute Percentage Error MAPE n
e
Y
t
tt
() =⋅ ⋅
⎛
⎝
⎜⎜
⎞
⎠
⎟⎟
=
1 100
1 1
n
∑  . (2.5)
One of the criticisms that MAPE has often received lies in the percentage error being 
undefined and/or infinite when Y t is zero (as in the case of intermittent time series) or 
numerically unstable when observations Yt approach zero. For more on this and other 
similar issues, we refer the savvy reader to the work of Makridakis (1993) and Hyndman 
& Koehler (2006).
The deficiencies of the percentage errors prompted researchers to start looking for 
alternative approaches for assessing forecasting accuracy. In this context, the relative 
error subclass of measures follows the spirit of percentage errors but scales the fore-
cast errors differently. In particular, a second set of forecast errors e˜
t, computed using a 
benchmark forecasting method such as the random walk without drift (where Yˆ
t is sim-
ply computed as Yt-1), is employed to scale the corresponding errors  et. Thus, the mean 
relative absolute error, for example, can be defined as:
 Mean Relative Absolute Error MRAE n
e
e
t
tt
n
() =⋅
=
∑
1
1 % .  (2.6)
The possibility that e˜t could be either small or, sometimes, zero has led to this subclass 
of accuracy measures to also be regarded with skepticism. As an extreme reaction, some 
authors have gone so far as to advise against the use of these relative error measures (see, 
e.g., Hyndman, 2008).
An alternative formulation of the relative error subclass requires the use of relative 
measures rather than relative errors. For example, if the mean absolute error MAEb and 
the mean squared error MSEb are computed for the benchmark forecasting method, then 
the relative mean absolute error and the relative mean squared error could be expressed 
as:
 
Relative Mean Absolute Error , and, 
Relati
RelMAE MAE
MAEb
() =
vve Mean Squared Error ,RelMSE MSE
MSEb
() =
 (2.7)

---

## Page 26

Forecasting  15
respectively. The advantage of accuracy measures in this subclass over other competing 
metrics lies in the intuitive interpretation of the results. A relative measure smaller than 
one suggests that the method considered performs better than the benchmark method. 
Conversely, a relative measure above one implies that the method considered is inferior 
in performance to the reference method. Among the disadvantages of the relative accu-
racy measures, two frequently quoted ones refer to the inappropriateness of their use 
when working with multiple time series and the need to forecast multiple times (Hynd-
man, 2008).
The last subclass of the scale-free measures makes use of scaled errors to assess the 
forecasting accuracy (Hyndman & Koehler, 2006). The forecast errors e
t are scaled in this 
case, for example, by the mean absolute error associated with the use of the random walk 
without drift forecasting method. Thus, the mean absolute scaled error can be written 
as:
 
Mean Absolute Scaled Error MASE n
e
MAE
t
bt
n
() =⋅ ⎛
⎝
⎜⎜
⎞
⎠
⎟⎟
=
=
∑
1
1
1
n n
e
n YY
n
e
n Y
t
ii
i
n
t
n
t
t
n
⋅
− ⋅−
⎡
⎣
⎢
⎢
⎢
⎢
⎢
⎤
⎦
⎥
⎥
⎥
⎥
⎥
=⋅
− ⋅
−
=
=
=
∑
∑
∑
1
1
1
1
1
1
2
1
1
iii
i
n
Y− −
=
∑ 1
2
 
 (2.8)
MASE has the same intuitive interpretation of the relative error measures. A MASE value 
below one suggests that the forecasts are more precise than those recommended by the 
random walk without drift forecasting method. The robustness of this measure has led 
several authors to recommend MASE as the standard metric for assessing the forecasting 
accuracy across multiple time series (Hyndman & Koehler, 2006; Hyndman, 2008).
The Bias and the Tracking Signal
The forecasting accuracy measures introduced in equations (2.4) – (2.8) help determine 
the recommended forecasting method to be used in a given context. These, however, 
do not provide timely intelligence on whether or not the forecasting method remains 
relevant once it is repeatedly applied on new streams of data. To assess the potential bias 
that the use of a specific forecasting method introduces, the sum of forecast errors can be 
employed. For all n time instances, the bias then can be iteratively expressed as:
 Bias e
t
t
n
=
=
∑
1
.  (2.9)
.

---

## Page 27

16  Forecasting
Ideally, the bias should not depart from but fluctuate around zero for the forecasts to 
be unbiased. The same holds if the forecast errors, plotted against time, are randomly 
distributed around zero and characterized by a regression fitted line that closely parallels 
the zero horizontal line.
While illustrative of the overall performance of the forecasting method, the bias 
alone cannot always lead to actionable decisions. Often, a reference point is provided by 
employing the tracking signal which scales the bias by the corresponding mean absolute 
error as shown below:
 
Tracking Signal .TS Bias
MAE() =  (2.10)
The time periods with a tracking signal outside the range[–4.0, +4.0] (depending on the 
application, the range may be tighter or wider) are either over-forecasted (i.e., TS ≤ –4.0) 
or under-forecasted (i.e., TS ≥ 4.0). Failure to keep the tracking signal within the accept-
able bounds may warrant the selection of a new forecasting method. As with the other 
forecasting accuracy measures, the bias and the tracking signal can be compiled on both 
estimation and holdout samples and are independent of how the forecasts are produced.
Illustration of the Use of Forecasting Accuracy Measures
At a very high level, we discuss the use of the forecasting accuracy measures for the time 
series depicted in Figure 2.1. The details of how these measures are adaptively computed 
are irrelevant at this point and therefore are left out of the discussion. They are, however, 
examined thoroughly throughout the later sections of this chapter. In this hypothetical 
example, a service company intends to estimate a model which would allow it to forecast 
its future monthly dollar sales. The first 36 monthly figures at this service company are 
used to estimate the parameters of an underlying forecasting model (i.e., triple exponen-
tial smoothing with an additive damped trend component and an additive error term). 
The last 18 monthly observations are held out for validation. The one-step-ahead fore-
casts computed on the estimation sample (dashed gray line on the left of the dotted verti-
cal line) appear to represent the original time series quite well. A similar performance is 
suggested by the one-step-ahead forecasts calculated on the holdout sample (dot-dashed 
black line on the right of the dotted vertical line). If the firm makes tactical decisions on a 
monthly basis and updates the forecasts accordingly, this is an indication of the expected 
accuracy when forecasting future sales. In contrast, if the firm needs to make strategic 
decisions that are further out in the future, then the expected accuracy should be assessed 
by extrapolating solely from the estimation data when computing the forecasts. These 
forecasts (continuous black line on the right of the dotted vertical line) suggest a much 
worse accuracy. If it exceeds the acceptable threshold imposed by the firm, the selection 
of a different forecasting method could be considered at this time. For completeness, we 
report some of the relevant forecasting accuracy measures in Table 2.1.
Throughout this section, the selection of the recommended forecasting method has 
been consistently linked to its forecasting performance on a holdout sample. There are 
exceptional circumstances, however, that may impede one to always follow this rule. 
Small samples usually warrant such a special treatment. In such cases, the use of penal-
ized criteria such as the Akaike’s Information Criterion (AIC) (Akaike, 1974) and/or 
the Bayesian Information Criterion (BIC) (Schwarz, 1978), computed on the full

---

## Page 28

Forecasting  17
sample, is generally recommended. For more details, the interested reader is referred to, 
for instance, the work of Hyndman et al. (2008) and Hyndman & Khandakar (2008).
The Importance of the Holdout Sample
The poor performance of the standard forecasts depicted in Figure 2.1 over the holdout 
period shows just how important is the decision to split the data set into the estimation 
and holdout samples. In particular, through our choice of positioning the start of the 
holdout period at the beginning of 2008, we effectively built a model on data that reflected 
prosperous years which we then attempted to validate on performance figures collected 
during an economic recession. In this case, an inadequate split decision could have done 
the proposed model an injustice. Specifically, based on the forecasting accuracy measures 
alone, we could have concluded that this model was a misfit and started to look for alter-
native ones. It turns out, however, that if no splitting is put in place—to account for the 
relevance of the most recent observations—the proposed model is still the preferred one 
at least in terms of the alternative AIC- and BIC-related selection criteria. If the idea of 
using a single estimation sample consisting of 54 monthly observations is deemed inap-
propriate, one could attempt to use the data from 2008 and parts of 2009 to both select 
the model of choice and compute the required forecasts. This task, however, could be 
difficult and error-prone due to the limited amount of historical data available.
2005
200
0
400
600
2006
Estimation Sample (2005–2007) Holdout Sample (2008+)
2007 2008 2009
Time (months)
Monthly $ Sales (thousands)
One-Step-Ahead Forecast (Estimation) One-Step-Ahead Forecast (Holdout)
Actual Monthly $ Sales Standard Forecast (Holdout)
Figure 2.1 Measuring Forecast Accuracy.
Table 2.1 Summary of Forecasting Accuracy Measures
Forecast Type Forecasting Accuracy Measures
ME MAE RMSE MAPE MASE
One-Step-Ahead Forecast (Estimation) –1.31 11.00 15.02 5.42 0.27
One-Step-Ahead Forecast (Holdout) 1.35 14.49 16.65 3.17 0.33
Standard Forecast (Holdout) –40.29 52.67 70.36 12.23 1.27

---

## Page 29

18  Forecasting
We conclude our discussion of the critical role the holdout samples play in forecast-
ing applications with a few thoughts that build on an arguably extreme example. Con-
sider, for instance, the time series depicted in the upper panel of Figure 2.2. This time 
series shows an upward trend and seasonal patterns that repeat each year. Relative to 
the annual average, the first six months of the year tend to underperform while the last 
six months usually over perform. Each year, the peak performance is reached during 
the months of November or December. Now, consider that a decision maker needs to 
make a one-time costly investment decision based on the demand likely to materialize 
in 2012. Hence, the decision maker tries to get an understanding of what she can expect 
to happen in the coming year and employs two competing forecasting methods A and B 
to compute the required demand figures. In terms of the in-sample forecasting accuracy 
measures computed on the entire data set, the two techniques do not differ that much. 
This behavior is apparent in the lower panel of Figure 2.2 where the in-sample one-
step-ahead forecasts for both methods follow the actual time series quite well. This said, 
method B, which accounts for both the trend and the seasonal patterns present in the 
data, performs slightly better than method A, which only deals with the observed upward 
trend (i. e. MSE
A
Dec 2011 = 178.4 vs. MSE
B
Dec 2011 = 40.6). In spite of this marginal improved 
performance, the decision maker may still choose to produce forecasts with method A, 
in particular, because this technique is a lot easier to operationalize and execute than 
method B. In doing so, however, the decision maker would make an unfortunate deci-
sion as her long-term forecasts would be rather unrepresentative of the actual time series’ 
behavior. These forecasts, as shown in the lower panel of Figure 2.2, will likely over fore-
cast what is reasonably expected to materialize in 2012 and could possibly lead to a poor 
investment decision. Such an outcome could be avoided, however, if the decision maker 
would test the one-time forecasting performance of both methods on a holdout sam-
ple. There, the abnormal behavior of method A would be easily spotted and the method 
would be removed from the set of the to-be-considered forecasting techniques. We illus-
trate this point by providing the forecasting accuracy measures computed on estimation 
and holdout samples, where the latter covers the full year of 2011. Based on the in-sample 
one-step-ahead forecasts, the mean squared errors corresponding to December of 2010 
(i.e., the last month of the estimation sample) are 166.0 and 45.0 for methods A and B, 
respectively. This similar performance is in sharp contrast with the relative performance 
of the out-of-sample mean squared errors computed on the holdout sample using the 
one-time forecasts produced based on the models calibrated on the estimation sample. 
Here, the mean square errors for methods A and B are 1,212.0 and 33.0, respectively. 
Faced with such forecasting accuracy figures, the decision maker can confidently remove 
method A from the techniques she is considering using to compute the long-term fore-
casts for 2012.
In the next sections, we detail some of the most commonly used forecasting tech-
niques, including those that we labeled as methods A and B in the example above. These 
techniques typically require the smoothing of the original time series through averaging 
or exponential smoothing.
SIMPLE AND WEIGHTED MOVING AVERAGE
The simple moving average method is used when no noticeable trends or seasonal pat-
terns are present in the time series data. Since it builds on the assumption of a constant

---

## Page 30

Forecasting  19
mean model, the simple moving average uses the mean of the most recent N observa-
tions as the forecast for any of the future time periods. This process is adaptive in the 
sense that the forecasts as well as the rolling means are updated dynamically as new data 
become available. In this setup, the oldest observation of the N data point rolling win-
dow is dropped to make room for the newly observed one. In formal terms, the dynamics 
of the forecasting process can be described as:
 
ˆYS
S YY Y Y
N
Y
N S Y
N
th t
t
t t tN tN t
t
tN
+
+
+− + − + + − +
=
= +++ + =+ −1
13 2 1 1K  (2.11)
2008
100
50
0
150
200
2009
Long-Term ForecastsIn-Sample Forecasts
(A) Actual Time Series
2010 2011 20132012
Time (months)
Monthly Demand
2008
100
50
0
150
200
2009
(B) In-Sample and Long-Term Forecasts: Method A vs. Method B
2010 2011 20132012
Time (months)
Monthly Demand
Actual Time Series Method A Method B
Actual Time Series
Figure 2.2 Illustration of the Role of Holdout Samples.

---

## Page 31

20  Forecasting
where t, N ≤ t ≤ T, is the current time period, N, N ≤ T, is the width or the order of the 
moving average, Yjs are the observed values of the time series at times j, j ∈ [t–N + 1, 
t + 1], j integer, St and St+1 are the rolling means computed at times t and t + 1, respec-
tively, and Yˆ
t+h is the forecast for time instances t + h, h ≥ 1, computed at time  t. If T 
provides the length of the time series, the forecasts Yˆ
t+h computed for periods t < T are 
all in-sample forecasts. Further, if  h=1, the forecasts are the one-step-ahead in-sample 
forecasts. These are the forecasts that are typically used to compute the in-sample fore-
casting accuracy measures. For t = T and h ≥ 1, ST provides an estimate for the forecasts 
for any number of time periods in the future. We call these forecasts long-term forecasts 
to differentiate them from the out-of-sample forecasts that one could compute on a 
holdout sample. Note that in this setup, the forecast for 1,000 periods in the future (i.e., 
h = 1,000) is the same as the forecast for one period in the future (i.e., h = 1), that is, we 
are assuming a constant mean.
Across all time series forecasting techniques, the basic goal when choosing param-
eter values for time series forecast is to distinguish the signal (e.g., the true changes in 
the demand patterns) from the noise (e.g., the random and inherent demand fluctua-
tions). For a simple moving average, the value chosen for N in equation (2.11) impacts 
greatly the one-step-ahead in-sample forecasts Yˆ
t+1. A small N leads to forecasts that 
follow the original time series quite closely. These forecasts, while extremely respon-
sive, incorporate a lot of the noise that surrounds the mean of the series. To balance the 
forecasts’ responsiveness and accuracy, higher values for N are also used in practice. 
These values smooth the appearance of the one-step-ahead in-sample forecasts and 
provide a clearer picture of how the series will behave in the long run. A relevant exam-
ple that looks into the impact on forecasts of multiple N values is depicted in Figure 2.3. 
At one end of the spectrum, an N value of 3 recommends one-step-ahead in-sample 
forecasts that describe the original series fairly well. At the other, an N value of 20 levels 
the forecasts so that they vaguely resemble the time series they are derived from. In 
0
65
60
55
75
70
80
10 20 30 40
Time
Y
Forecast SMA(10)
Forecast SMA(20)
Actual Observations
Forecast SMA(3)
Figure 2.3 Simple Moving Average—In-Sample and Long-Term Forecasts

---

## Page 32

Forecasting  21
between these extremes, an N value of 10 leads to forecasts that follow the time series 
but lag behind the turning points by about 5 (or, N/2) time periods. In practical appli-
cations, N is typically chosen such that the corresponding moving average results in 
the best in-sample data fit.
The construction of the forecast lines depicted in Figure 2.3 is detailed in Table 2.2. 
For the simple moving average of order 3, the one-step-ahead forecast Yˆ
4 is computed 
using Y3, Y2 and Y1 as, Yˆ
4 =(Y3 + Y2 + Y1)/ N, or, equivalently, as Yˆ
4 = (79 + 61 + 69)/3 = 
69.7. Since their time series indices are smaller than or equal to the width of the moving 
average, the first three data periods do not show in-sample forecasts. Similar judgment 
applies to the higher order moving averages SMA (10) and SMA (20) which do not show 
forecasts up to the 11th and the 21st observation, respectively. All other forecasts, how-
ever, are computed following the simple approach discussed above but employing roll-
ing windows of size 3, 10 or 20. Although labeled as Yˆ
t+1 and possibly implying an associa-
tion with the in-sample one-step-ahead forecasts, the forecast values reported in the last 
row of Table 2.2 for period 40 are long-term forecasts that characterize all future time 
periods. The horizontal lines in Figure 2.3 correspond to these long-term forecasts.
The formulae provided in equation (2.11) assign an equal weight to all N observations 
in the rolling horizon. While easy to implement in practice, this approach is at times 
counterintuitive since the same amount of weight is put on a demand observation that 
occurred N periods in the past as is put on the observation that occurred in the previous 
period. A modification to the moving average technique that allows for more weight to 
be put on the most recent observations is the weighted moving average method. The 
recursive formula for the forecasts can then be restated as:
Table 2.2 Simple Moving Average – In-Sample and Long-Term Forecasts
Period Yt S t = Yˆt + 1 St=Yˆt +1 St = Yˆt +1 Period Y t St= Yˆt + 1 St=Yˆt +1 St = Yˆt +1
t SMA (3) SMA (10) SMA (20) t SMA (3) SMA (10) SMA (20)
1 69 — — — 21 62 63.0 70.9 69.3
2 61 — — — 22 61 61.7 70.1 69.3
3 79 69.7 — — 23 63 62.0 68.7 68.5
4 71 70.3 — — 24 65 63.0 67.9 68.2
5 60 70.0 — — 25 70 66.0 67.5 68.7
6 74 68.3 — — 26 62 65.7 65.9 68.1
7 72 68.7 — — 27 65 65.7 65.2 67.8
8 66 70.7 — — 28 63 63.3 63.8 67.6
9 61 66.3 — — 29 64 64.0 63.7 67.8
10 66 64.3 67.9 — 30 76 67.7 65.1 68.2
11 67 64.7 67.7 — 31 70 70.0 65.9 68.4
12 69 67.3 68.5 — 32 69 71.7 66.7 68.4
13 77 71.0 68.3 — 33 72 70.3 67.6 68.2
14 73 73.0 68.5 — 34 68 69.7 67.9 67.9
15 74 74.7 69.9 — 35 70 70.0 67.9 67.7
16 78 75.0 70.3 — 36 69 69.0 68.6 67.2
17 72 74.7 70.3 — 37 78 72.3 69.9 67.5
18 77 75.7 71.4 — 38 61 69.3 69.7 66.8
19 65 71.3 71.8 — 39 67 68.7 70.0 66.8
20 62 68.0 71.4 69.7 40 67 65.0 69.1 67.1

---

## Page 33

22  Forecasting
 ˆYS w Y w Y w Y w Yth t t t t t tN tN tN tN+− − − + − + − + − +==⋅ + ⋅ ++ ⋅ + ⋅ 11 2 2 1 1 K ,  (2.12)
where t, N, St, Yj and Yˆ
t+h have the meaning discussed before and wjs, 0≤ wj ≤1,  ∑
t
 wj = 1 
 j=t–N+1
are constants that represent the different weights assigned to the observations in the rolling 
horizon. Often, the weights are proportional with the observations’ position in the horizon 
and decrease linearly or exponentially with the observations’ age. For a linearly weighted 
moving average, the adaptive formulation provided in equation (2.12) becomes:
 ˆYS NY N Y Y Y
NNth t
t t tN tN
+
−− + − +== ⋅+ − () ⋅+ + ⋅ + ⋅
+−() ++ +
12 1
12 1
12 1K
K . (2.13)
The special case of an exponentially weighted moving average is discussed in the next few 
sections of this chapter.
The expressions in equations (2.12) and (2.13) are graphically operationalized in Fig-
ure 2.4. The forecast lines are all built using weighted moving averages of order 5, or, 
equivalently, N = 5. As expected, the smoothness of the lines depends on the weights 
assigned to the most recent observations. Higher values as for WMA(5)a and WMA(5) 
b lead to very responsive in-sample forecasts that follow the original series more aggres-
sively than those recommended by the equivalent simple moving average (i.e., SMA (5)). 
This responsiveness, while critical in certain fields, may be detrimental in others. Thus, 
when selecting the weights w
j, one needs to carefully balance the desired precision and 
the intended forecast responsiveness.
The calculation of the forecast lines shown in Figure 2.4 is detailed in Table 2.3. For exam-
ple, the forecasts Yˆ
6 for the three distinct weighted moving averages can be computed as:
0
65
60
55
75
70
80
10 20 30 40
Time
Y
Forecast WMA(5)a
Forecast WMA(5)b
Actual Observations
Forecast SMA(5)
Figure 2.4 Weighted Moving Average—In-Sample and Long-Term Forecasts.
Note: To compute the in-sample forecast for a time period (t+1), we adjust the observations Yt, Yt-1, Yt-2, Yt-3 and Yt-4 in the rolling horizon by the fol-
lowing sets of weights: SMA(5) — (0.20, 0.20, 0.20, 0.20, 0.20); WMA(5)a — (5/15, 4/15, 3/15, 2/15, 1/15); and, WMA(5)b — (0.80, 0.05, 0.05, 
0.05, 0.05) The long-term forecasts coincide with the forecast computed using the observations in the last rolling window of size 5 (i.e., t = 40).

---

## Page 34

Forecasting  23
 S M A Y YYYYY51 1 1 1 1 565 4 3 2 1() = ⋅ +⋅ +⋅ +⋅ +⋅()          
           
ˆ
                 
             
= ⋅ +⋅ +⋅ +⋅ +⋅()1 6 01 7 11 7 91 6 11 6 95
               
     
=
() =⋅+ ⋅+ ⋅+ ⋅+ ⋅
68
55 4 3 2 165 4 3 2WMA a Y Y Y Y Y Y ˆ 1 1 54321
56 0 47 1 37 9
() ++++()
=⋅+ ⋅+ ⋅+                           22 61 1 69 15
67 5
5
⋅+ ⋅()
=
()
                           
   
.
ˆWMA b  YYY Y Y Y Y65 4 3 2 108 0 00 5 00 5 00 5 00 5  
             
=⋅ +⋅ +⋅ +⋅ +⋅.....
               
   
=⋅ +⋅ +⋅ +⋅ +⋅0 80 60 0 05 71 0 05 79 0 05 61 0 05 69.....
                         =62.
 
(2.14)
A similar approach can be employed to compute all other forecasts, including the long-
term ones (i.e., Yˆ
T+h = Yˆ
40+h, h ≥ 1, h integer).
Up to this point, we have discussed extensively how the moving average can help com-
pute forecasts but said little about how finding the order of the moving average and 
selecting the right set of weights are to be approached. In practice, both tasks typically 
rely on forecasting accuracy measures to compare and select among feasible solutions. 
In particular, of all candidate solutions, it is customary to select the one that minimizes 
either the in-sample mean absolute error ( MAE) or the in-sample mean squared error 
(MSE). We illustrate how some of the most common forecasting accuracy measures are 
Table 2.3 Weighted Moving Average—In-Sample and Long-Term Forecasts
Period
t Yt St = Yˆt + 1
SMA (5)
St=Yˆt +1
WMA (5)a
St = Yˆt +1
WMA (5)b
Period
t Yt St= Yˆt + 1
SMA (5)
St=Yˆt +1
WMA (5)a
St = Yˆt +1
WMA (5)b
1 69 — — — 21 62 67.6 65.3 63.4
2 61 — — — 22 61 65.4 63.1 62.1
3 79 — — — 23 63 62.6 62.3 62.9
4 71 — — — 24 65 62.6 63.1 64.4
5 60 68.0 67.5 62.0 25 70 64.2 65.5 68.5
6 74 69.0 69.5 72.8 26 62 64.2 64.8 62.6
7 72 71.2 70.5 71.8 27 65 65.0 65.1 65.0
8 66 68.6 68.7 66.7 28 63 65.0 64.4 63.5
9 61 66.6 66.2 62.4 29 64 64.8 64.1 64.2
10 66 67.8 66.0 66.5 30 76 66.0 67.8 73.5
11 67 66.4 65.7 66.9 31 70 67.6 69.1 69.4
12 69 65.8 66.6 68.2 32 69 68.4 69.6 68.9
13 77 68.0 70.3 74.8 33 72 70.2 70.8 71.5
14 73 70.4 72.0 72.4 34 68 71.0 70.1 68.8
15 74 72.0 73.2 73.5 35 70 69.8 69.7 70.0
16 78 74.2 75.2 77.1 36 69 69.6 69.5 69.2
17 72 74.8 74.5 72.7 37 78 71.4 72.3 76.4
18 77 74.8 75.2 76.5 38 61 69.2 68.8 63.1
19 65 73.2 71.9 67.0 39 67 69.0 68.1 67.5
20 62 70.8 68.2 64.2 40 67 68.4 67.4 67.3

---

## Page 35

24  Forecasting
computed in Table 2.4, which focuses on the simple moving average of order 5. For 
illustration purposes only, we provide a summary of the accuracy measures for all other 
moving averages introduced in this section in Table 2.5.
In Table 2.4, we compute ME, MAE, MSE, RMSE, MAPE, MASE and TS using equa-
tions (2.4)–(2.6) and (2.10). We estimate these accuracy measures adaptively so that for 
Table 2.4 In-Sample Forecasting Accuracy Measures—SMA(5)
Period 
t Yt S t Y ˆt et ME t A t MAE t MSE t RMSE t % |et| MAPEt MASE t TS t 
16 9
26 1
37 9
47 1
5 60 68.0
6 74 69.0 68.0 6.0 6.0 6.0 6.0 36.0 6.0 8.1 8.1 — 1.00
7 72 71.2 69.0 3.0 4.5 3.0 4.5 22.5 4.7 4.2 6.1 2.25 2.00
8 66 68.6 71.2 –5.2 1.3 5.2 4.7 24.0 4.9 7.9 6.7 1.18 0.80
9 61 66.6 68.6 –7.6 –0.9 7.6 5.5 32.5 5.7 12.5 8.2 1.26 –0.70
10 66 67.8 66.6 –0.6 –0.9 0.6 4.5 26.0 5.1 0.9 6.7 1.00 –0.98
11 67 66.4 67.8 –0.8 –0.9 0.8 3.9 21.8 4.7 1.2 5.8 1.02 –1.34
12 69 65.8 66.4 2.6 –0.4 2.6 3.7 19.7 4.4 3.8 5.5 1.05 –0.71
13 77 68.0 65.8 11.2 1.1 11.2 4.6 32.9 5.7 14.5 6.6 1.12 1.86
14 73 70.4 68.0 5.0 1.5 5.0 4.7 32.0 5.7 6.8 6.7 1.13 2.91
15 74 72.0 70.4 3.6 1.7 3.6 4.6 30.1 5.5 4.9 6.5 1.21 3.77
16 78 74.2 72.0 6.0 2.1 6.0 4.7 30.6 5.5 7.7 6.6 1.23 4.95
17 72 74.8 74.2 –2.2 1.8 2.2 4.5 28.5 5.3 3.1 6.3 1.12 4.68
18 77 74.8 74.8 2.2 1.8 2.2 4.3 26.7 5.2 2.9 6.0 1.05 5.39
19 65 73.2 74.8 –9.8 1.0 9.8 4.7 31.6 5.6 15.1 6.7 1.00 2.85
20 62 70.8 73.2 –11.2 0.1 11.2 5.1 37.9 6.2 18.1 7.4 1.12 0.43
21 62 67.6 70.8 –8.8 –0.4 8.8 5.4 40.3 6.4 14.2 7.9 1.26 –1.23
22 61 65.4 67.6 –6.6 –0.8 6.6 5.4 40.5 6.4 10.8 8.0 1.34 –2.43
23 63 62.6 65.4 –2.4 –0.9 2.4 5.3 38.6 6.2 3.8 7.8 1.34 –2.96
24 65 62.6 62.6 2.4 –0.7 2.4 5.1 36.9 6.1 3.7 7.6 1.33 –2.58
25 70 64.2 62.6 7.4 –0.3 7.4 5.2 37.8 6.1 10.6 7.7 1.34 –1.11
26 62 64.2 64.2 –2.2 –0.4 2.2 5.1 36.2 6.0 3.5 7.5 1.24 –1.57
27 65 65.0 64.2 0.8 –0.3 0.8 4.9 34.6 5.9 1.2 7.2 1.21 –1.47
28 63 65.0 65.0 –2.0 –0.4 2.0 4.8 33.3 5.8 3.2 7.1 1.20 –1.93
29 64 64.8 65.0 –1.0 –0.4 1.0 4.6 31.9 5.6 1.6 6.8 1.20 –2.21
30 76 66.0 64.8 11.2 0.0 11.2 4.9 35.7 6.0 14.7 7.2 1.17 0.21
31 70 67.6 66.0 4.0 0.2 4.0 4.8 34.9 5.9 5.7 7.1 1.14 1.03
32 69 68.4 67.6 1.4 0.2 1.4 4.7 33.7 5.8 2.0 6.9 1.14 1.36
33 72 70.2 68.4 3.6 0.4 3.6 4.7 32.9 5.7 5.0 6.8 1.15 2.14
34 68 71.0 70.2 –2.2 0.3 2.2 4.6 32.0 5.7 3.2 6.7 1.13 1.70
35 70 69.8 71.0 –1.0 0.2 1.0 4.5 30.9 5.6 1.4 6.5 1.12 1.52
36 69 69.6 69.8 –0.8 0.2 0.8 4.3 30.0 5.5 1.2 6.4 1.11 1.38
37 78 71.4 69.6 8.4 0.5 8.4 4.5 31.2 5.6 10.8 6.5 1.10 3.22
38 61 69.2 71.4 –10.4 0.1 10.4 4.7 33.6 5.8 17.0 6.8 1.04 0.86
39 67 69.0 69.2 –2.2 0.1 2.2 4.6 32.7 5.7 3.3 6.7 1.01 0.39
40 67 68.4 69.0 –2.0 0.0 2.0 4.5 31.9 5.6 3.0 6.6 1.03 –0.04

---

## Page 36

Forecasting  25
any time period t their values characterize the up-to-date forecasting accuracy associated 
with all observations for which relevant data exist. This necessarily means that we evalu-
ate all equations several times to mimic how the accuracy metrics evolve in time as more 
and more information becomes available. As shown in the last column of the table, at 
times, the tracking signal TS exceeds or follows closely the ±4 range, which indicates that 
the forecast using the five-period moving average may contain some significant bias. In 
our example, we seem to consistently under-forecast the time periods clustered around 
observation 15 and over-forecast those around observation 20; thus, the five-period 
moving average appears to respond a little too slowly to the changes in the mean of the 
time series. Besides showing a possible bias, the forecast has a reasonable MAE of 4.5 and 
MAPE of 6.6%. While this is encouraging, the MASE value of 1.03 suggests that the sim-
ple five-period moving average does not perform better than the competing but simpler 
random walk without drift forecasting technique which simply assigns the last observed 
time series entry to the forecast.
To echo some of the views we expressed already in the previous section of this chap-
ter, we reiterate that the standard process of finding the order of the moving aver-
age and selecting the right set of weights is not always error-free. In particular, since 
the forecasting accuracy measures that help select N and w
j s are representative of the 
entire time series data (see, for example, Table 2.4 and Table 2.5), they may be of little 
relevance to how the preferred moving average would perform on new streams of data. 
Oftentimes, these forecasting accuracy measures understate the magnitude of the true 
forecasting errors as the search for N and w
j s may induce the overfitting of the data. 
As hinted at previously, and generally applicable to all forecasting initiatives, a more 
sensible approach requires splitting the data into an estimation and a holdout sample, 
estimating the parameters of competing models on the estimation sample and validat-
ing/refining the model choice on data withheld from the parameter estimation and avail-
able in the holdout sample. Typically, models with a similar performance in regards to 
the forecasting accuracy measures on both estimation and holdout samples are preferred 
and, subsequently, reestimated on the entire time series to compute the forecasts beyond 
the horizon covered by the available data. We provide a fully worked-out example of this 
approach in the case study on p. 39.
SIMPLE EXPONENTIAL SMOOTHING
The simple exponential smoothing method performs well for time series with no notice-
able trends or seasonal patterns. Unlike the moving average technique which uses 
the mean of the most recent N observations as an estimate for the forecasts, simple 
Table 2.5 Summary of Forecasting Accuracy Measures
 Series ME MAE MSE RMSE MAPE MASE TS 
SMA(3) –0.3 4.1 29.4 5.4 6.1 0.85 –2.61
SMA(10) 0.2 4.9 35.7 6.0 7.2 1.10 1.42
SMA(20) –1.0 4.1 26.1 5.1 6.1 0.91 –4.94
SMA(5) 0.0 4.5 31.9 5.6 6.6 1.03 –0.04
WMA(5)a 0.0 4.0 28.4 5.3 5.9 0.92 0.07
WMA(5)b 0.1 4.3 32.5 5.7 6.3 0.98 1.07

---

## Page 37

26  Forecasting
exponential smoothing relies on all data available at time t to compute a smoothed mean 
and, implicitly, the forecasts. In particular, as new information becomes available, sim-
ple exponential smoothing makes use of the following recursive formulae to compute 
the forecasts and update the smoothed mean of the series:
 
ˆYS
SY S
th t
tt t
+
++
=
=⋅ +− () ⋅11 1αα
 (2.15)
where t, 0 ≤ t ≤ T, is the current time period, Yt+1 is the newly observed value of the time 
series at time t + 1, St and St+1 are the smoothed means of the time series at times t and t + 
1, respectively, Yˆ
t+h is the forecast for time instances t + h, h ≥ 1, computed at time t and 
α is a smoothing parameter with values between 0 and 1. The value assigned to or com-
puted for α dictates the importance the current observation Yt plays in determining the 
forecasts Yˆ
t+h for the next time periods. An α value close to 0 indicates that the forecasts 
follow closely the smoothed mean of all previous observations, or, equivalently, a value 
that does not change much in time (e.g., the overall mean of the time series). Con-
versely, an α value close to 1 suggests that the forecasts rely heavily on the last observa-
tion, or, equivalently, that they are extremely responsive to the observed changes in the 
time series. As for the moving average technique, if T provides the length of the time 
series, the forecasts Yˆ
t+h computed for periods t < T are all in-sample forecasts. Further, 
if h = 1, the forecasts are the one-step-ahead in-sample forecasts. These are the fore-
casts that are typically used to compute the in-sample forecasting accuracy measures 
which are part of the process that leads to the estimation of the α parameter. For t = 
T and h ≥ 1, ST provides an estimate for the long-term forecast for all time periods in 
the future.
To provide an understanding for why the method’s name makes references to expo-
nential smoothing (or, exponential weighting), we re-write Yˆ
t+h in equation (2.15) as:
ˆYS
YS
YY S
th t
tt
tt t
+
−
−−
=
=⋅ +− () ⋅
=⋅ +− () ⋅⋅ + − () ⋅()
=⋅
αα
αα α α
α
1
11
1
12
YYY S
YY
ttt
tt
+⋅− () ⋅+ − () ⋅
=⋅ +⋅− () ⋅+ ⋅ − ()
−−
−
αα α
αα α α α
11
11
1
2
2
1
2
...
⋅⋅ + + − () ⋅
=⋅ +− () ⋅+ − () ⋅+ + − ()
−
−
−−
−
YS
YY Y
t
t
tt t
t
2
1
1
1
2
2
1
11 1
K
K
α
αα α α 1 1
1
0
01
1
2
2
1
11 1 1
⋅( ) +
+−() ⋅
=⋅ − () +−() ⋅+ − () ⋅+ + −−−
Y
S
YY Y
t
tt t
α
αα α α K α α
α
() ⋅( ) +
+−() ⋅
−t
t
Y
S
1
1
01 (2.16)

---

## Page 38

Forecasting  27
where S0 is the value of the smoothed mean at time t = 0. For a sufficiently large t and 
|1 – α| < 1, we can write (1 – α)0 + (1 – α)1 + … + (1 – α)t–1 = 1/ α in which case equation 
(2.16) becomes:
 ˆY YY Y Y
th
tt t
t
+
−−
−
= ⋅+− () ⋅+ − () ⋅+ + − () ⋅
+−() +−
11 1 1
11 1
1
2
2
1
1αα α
αα
K
(() ++ − ()
+
+−() ⋅
−21
0
1
1
K α
α
t
t S     .
 (2.17)
As it is readily apparent from equation (2.17), the computation of forecasts Yˆ
t+h involves 
the exponential smoothing (or, exponential weighting) of all observations available at 
time t. It too requires a sensible initial value for S0. In particular, when α approaches 0, 
extra care needs to be exercised when recommending the value of this initial smoothed 
mean. A common approach to specifying S
0 requires the computation of the average of 
the first observations in the time series, or, S0 = ∑
m
j=1 Yj/m, where m gives the number of 
observations in the selected time window (e.g., 5, 10, T) and j is an integer between 1 and m.
Typically, the parameter α in equation (2.15) is either specified a priori—best prac-
tices recommend the use of an α value close to 0.30—or estimated from the data such 
that the in-sample mean squared error is minimized. A computed α value above 0.50 
typically reflects that either a trend, seasonal patterns or both are present in the data. If 
α is computed from the available time series data, the initial value S0 for the smoothed 
mean may impact the quality of the α estimate. Specifically, the approach that requires S0 
to be the mean of the first m observations leads at times to numerical instabilities in the 
presence, for example, of even moderate trends in the time series data. Thus, we recom-
mend an alternative initialization procedure which has been shown to be robust and has 
been implemented in environments for statistical computing such as R (R Core Team, 
2013). In particular, we consider that the recursive formulae of equation (2.15) apply to 
all time periods t, 1 ≤ t ≤ T, where we force S
1 to equal Y1. In this setup, at time t = 1, the 
forecasts for all future time periods including the second equal S1, and, implicitly, Y1.
The assumption that the time series does not show any noticeable patterns such as 
trend or seasonality leads to the long-term forecasts for the simple exponential smooth-
ing to follow a horizontal line. In abstract terms, the forecast for any future time period 
T + h, h ≥ 1, h integer, can be expressed as:
YSY S
TH T T T+− == ⋅ + − () ⋅αα 1 1
Thus, the forecast for the next period, T+1, is the same as the forecast for all future peri-
ods. We illustrate the flatness of the simple exponential smoothing long-term forecasts 
in Figure 2.5, which depicts the weekly unconstrained sales for a pack of roofing shingles 
at a Home Depot store. In spite of the forecasts being constant over time, you should 
recognize that the width of the corresponding 95.0% prediction intervals—the intervals 
in which future observations are expected to fall with a probability of 0.95—increases the 
further in the future you are forecasting. As expected, the forecasts for periods closer to 
the end of the observed time series display tighter prediction intervals, or, equivalently, 
are expected to be more accurate.
ˆ

---

## Page 39

28  Forecasting
In formal terms, the limits of the 1–αPI prediction intervals for forecasts Yˆ
T+h are com-
puted as: 
Yz hTh ePI+ ±⋅ ⋅ + − () ⋅α σα2
211 ,
where Yˆ
T+h is the long-term forecast h periods after the end of the time series, σe is the stand-
ard deviation of the forecast errors calculated from the estimation data, α is the smoothing 
parameter, αPI is the significance level for the prediction intervals (e.g., 5% or 10%), and 
zαPI
/H208822 returns the inverse of the standard normal cumulative distribution computed at αPI/H208822. 
To be consistent with the material discussed in the Theory of Forecasting section on p. 10 
and, we mention that the prediction interval limits for the simple exponential smoothing 
are computed by assuming that an ARIMA(0,1,1) model is the true underlying model. For 
more details on this and other related topics, we refer the interested reader to the compre-
hensive work of Yar and Chatfield (1990, p. 129) and Chatfield and Yar (1991, p. 33).
The construction of the forecast lines depicted in Figure 2.5 is detailed in Table 2.6, 
which leaves out several of the time series observations due to space constraints. At time 
t =1, the forecast for all subsequent time periods, including the second one, can be com-
puted as Yˆ
t+h = St, or, equivalently, as Yˆ
1+h = S1 = Y1 =152. Once the second observation 
becomes current, we update the estimate of the smoothed mean such that S2 = α·Y2+ 
(1–α)· S1. For an α value of 0.428, S2 becomes 0.428 · 163 + (1–0.428) · 152, or, S2 = 156.7. 
At this time, the forecast for all future time periods, including the third one, equals S2, or, 
Yˆ
2+h = S2= 156.7. This iterative process repeats until all observations of the time series are 
exhausted. The smoothed mean S104 for the last time series observation is used then as the 
forecast for all upcoming and, therefore, unobserved time periods. Thus, the long-term 
forecasts Yˆ
T+h, h ≥ 1, all equal 141.4 units.
The one-step-ahead in-sample forecasts Yˆ
t+1, t < T, together with the observed values 
of the time series help compute the in-sample forecasting accuracy measures. We show 
0
150
100
50
250
200
300
20 40 60 80 100
Time (Weeks)
Unconstrained Weekly Sales
(units)
Long-Term Forecast
95.0% Prediction Intervals
Unconstrained Sales
In-Sample Forecast
Figure 2.5 Simple Exponential Smoothing—In-Sample and Long-Term Forecasts.
ˆ

---

## Page 40

Forecasting  29
some of these measures in the last columns of Table 2.6. For this example, the value of 
0.428 for the α parameter minimizes the in-sample mean squared error, or, the MSE 
computed at T=104. Spreadsheet-like computing environments such as Excel (Micro-
soft, 2010) or Calc (The Apache Software Foundation, 2012) or proprietary or freeware 
statistical software packages such as SAS (SAS Institute Inc., 2012), Stata (StataCorp, 
2012) or R (R Core Team, 2013) all have advanced capabilities for optimizing the value 
of 
α. The MAE104 of 21.7 and MAPE104 of 12.6% alone suggest that the forecasts describe 
the time series fairly well. In contrast, the MASE104 of 0.91 together with how the tracking 
signal TS evolves as new data become available (not fully visible in Table 2.6) implies that 
the simple exponential smoothing does only marginally better than the simpler reference 
forecasting method and that the forecasts are consistently under- or over-estimating the 
product demand based on the upward or downward trends present in the data. Based on 
these additional insights, the firm may consider at this time to experiment with alterna-
tive forecasting methods.
DOUBLE EXPONENTIAL SMOOTHING
The double exponential smoothing method builds on the concepts introduced in the 
Simple Exponential Smoothing section on p. 25 but provides for the computation of 
time series with trends and no seasonality. The formulae for the recursive calculations 
and forecasts revised to account for the presence of a trend component are given below:
Table 2.6 In-Sample Forecasting Accuracy Measures—Simple Exponential Smoothing
α 0.428
MSET 837.7
Period
     t Yt S t Y ˆ
t et ME t At MAEt MSEt RMSE t % |et| MAPEt MASEt TSt 
1 152 152.0 –
2 163 156.7 152.0 11.0 11.0 11.0 11.0 121.0 11.0 6.7 6.7 – 1.00
3 155 156.0 156.7 –1.7 4.6 1.7 6.4 62.0 7.9 1.1 3.9 0.79 1.46
4 168 161.1 156.0 12.0 7.1 12.0 8.2 89.5 9.5 7.2 5.0 0.79 2.59
5 72 123.0 161.1 –89.1 –17.0 89.1 28.5 2052.9 45.3 123.8 34.7 0.73 –2.38
6 161 139.3 123.0 38.0 –6.0 38.0 30.4 1931.5 43.9 23.6 32.5 0.59 –0.98
7 168 151.6 139.3 28.7 –0.2 28.7 30.1 1747.3 41.8 17.1 29.9 0.71 –0.03
8 179 163.3 151.6 27.4 3.8 27.4 29.7 1605.3 40.1 15.3 27.8 0.80 0.89
9 210 183.3 163.3 46.7 9.1 46.7 31.8 1677.2 41.0 22.2 27.1 0.87 2.30
10 157 172.0 183.3 –26.3 5.2 26.3 31.2 1567.7 39.6 16.7 26.0 0.81 1.50
...
95 183 180.4 178.5 4.5 0.7 4.5 21.6 839.9 29.0 2.5 12.1 0.91 3.07
96 135 161.0 180.4 –45.4 0.2 45.4 21.9 852.7 29.2 33.6 12.3 0.91 0.96
97 109 138.7 161.0 –52.0 –0.3 52.0 22.2 872.0 29.5 47.7 12.7 0.92 –1.40
98 127 133.7 138.7 –11.7 –0.4 11.7 22.1 864.4 29.4 9.2 12.7 0.92 –1.94
99 134 133.8 133.7 0.3 –0.4 0.3 21.9 855.6 29.3 0.2 12.5 0.92 –1.94
100 166 147.6 133.8 32.2 –0.1 32.2 22.0 857.4 29.3 19.4 12.6 0.92 –0.47
101 114 133.2 147.6 –33.6 –0.4 33.6 22.1 860.1 29.3 29.5 12.8 0.91 –1.99
102 130 131.8 133.2 –3.2 –0.5 3.2 21.9 851.7 29.2 2.5 12.7 0.91 –2.15
103 146 137.9 131.8 14.2 –0.3 14.2 21.8 845.3 29.1 9.7 12.6 0.91 –1.51
104 146 141.4 137.9 8.1 –0.2 8.1 21.7 837.7 28.9 5.5 12.6 0.91 –1.15
Note: Entries for time periods t ∈[11, 94] are not shown due to space constraints.

---

## Page 41

30  Forecasting
 
ˆYS h T
SY S T
TS S
th t t
tt t t
tt t
+
++
++
=+ ⋅
=⋅ +− () ⋅+()
=⋅ −() +−
11
11
1
1
αα
ββ (() ⋅Tt
 (2.18)
where t, 0 ≤ t ≤ T, is the current time period, Yt+1 is the newly observed value of the time 
series at time t + 1, St and St+1 are the smoothed means of the time series at times t and 
t + 1, respectively, Tt and Tt+1 are the estimates for trend computed at times t and t + 1, 
respectively, Yˆ
t+h is the forecast for time instances t + h, h ≥ 1, computed at time t and 
α and β are smoothing parameters with values between 0 and 1. The parameters α and 
β adaptively weight the current and old values of the smoothed mean and trend. As for 
the other forecasting techniques we have discussed already, if T provides the length of 
the time series, the forecasts Yˆ
t+h computed for periods t < T are all in-sample forecasts. 
Further, if h = 1, the forecasts are the one-step-ahead in-sample forecasts. Typically, the 
α and β parameters are optimized over forecasting accuracy measures that employ the 
latter of these types of forecasts. Parameter values close to 0 lead to estimates for the 
smoothed mean and trend that translate into smooth in-sample forecasts. In contrast, α 
and β values close to 1 suggest that the smoothed mean and trend depend heavily on the 
most recent information available. Thus, the in-sample forecasts are to be expected to be 
responsive to the actual changes in the time series. For t = T and h ≥ 1, S
T + h · TT provides 
an estimate for the long-term forecasts for all time periods in the future.
The recursive formulae shown in equation (2.18) and the subsequent results depend 
upon the values assigned to S0 and T0. Traditionally, a linear model is fitted to the first 
few observations of the time series (e.g., 5, 10,  T) and the resulting intercept and slope 
are used to initialize S0 and T0, respectively. Since this initialization leads at times to poor 
overall forecasting performance, we recommend an alternative approach that requires 
the recursive formulae of equation (2.18) to iterate over all periods t, 2 ≤ t ≤ T, where S
2 
and T2 are assigned Y2 and Y2 – Y1, respectively. This more robust approach is coded in 
the specific functions of some of the leading environments for statistical computing such 
as R (R Core Team, 2013).
The assumption that the time series follows an underlying trend with no seasonal-
ity components leads to the long-term forecasts for the double exponential smoothing 
to follow a straight line. Its slope coincides with the value of the last smoothed slope 
T
T computed using observations from the actual time series. Figure 2.6 highlights this 
point using a subset of the monthly data describing the seasonally adjusted levels of the 
finished goods inventories in the US textile industry (EconStats, February 17, 2012). As 
with the flat forecasts for the simple exponential smoothing, the point forecasts in Figure 
2.6 display prediction intervals with variable width confirming the expectation that the 
forecasts for closer future periods are more accurate. Formally, the limits of the 1 – αPI 
prediction intervals for forecasts Yˆ
T+h are computed as:
Yz jTh e
j
h
PI
  +
=
−
±⋅ ⋅ + ⋅ + ⋅ ()
⎛
⎝
⎜
⎜
⎞
⎠
⎟
⎟∑α σα β2
2 2
1
1
11 ,
where Yˆ
T+h is the long-term forecast h, h > 1, periods after the end of the time series, σe 
is the standard deviation of the errors and is calculated from the estimation data, α and 
Yˆ

---

## Page 42

Forecasting  31
β are the smoothing parameters, αPI is the significance level for the prediction intervals 
(e.g., 5% or 10%) and zαPI
/H208822 returns the inverse of the standard normal cumulative dis-
tribution computed at αPI /2. For h = 1, the square root factor next to σe is replaced by 1. 
These prediction limits are computed assuming that an ARIMA(0,2,2) model, which is 
the ARIMA model equivalency to double exponential smoothing, is the true underlying 
model that governs how the time series data has been generated.
The construction of the forecast lines in Figure 2.6 is explained in Table 2.7. At time 
t = 2, the forecast for all subsequent time periods can be computed as Yˆ
t+h = St + h · Tt, 
or, equivalently, as Yˆ
2+h = S2 + h · T 2. Hence, the one-step-ahead forecast for period t = 
3 becomes Yˆ
3 = S2 + T2 = 1,525.0 + 9.0 = 1,534.0. Once the third observation becomes 
current, we update the estimates of the smoothed mean and trend such that S3 = α . Y3 
+ (1 – α) . (S2 + T2) and T3 = β . (S3 – S2) + (1 – β) . T2. For an α value of 0.821 and a β 
value of 0.025, S3 and T3 are 1,511.0 and 8.4, respectively. At this time, the forecasts for 
all future time periods can be computed using Yˆ
t+h = St + h . Tt, or, Yˆ
3+h = S3 + h . T3, h ≥ 
1. This iterative process applies to all 42 monthly data points present in the time series. 
The final smoothed mean S42 of 1,731.0 and trend T42 of 6.4 determine thereafter all long-
term forecasts Yˆ
T+h, h ≥ 1.
The one-step-ahead in-sample forecasts Yˆ
t+1, t < T, together with the actual values of 
the time series allow us to compute the in-sample forecasting accuracy measures, some 
of which we depict in the last columns of Table 2.7. In this example, we estimate the val-
ues of the 
α and β parameters, that is, 0.821 and 0.025, respectively, as so to minimize the 
in-sample mean squared error MSE42. Relative to the size of the forecast, both MAE42 and 
MAPE42 show values that are quite competitive. In contrast, the evolution of the tracking 
signal up to period 42 (only partially available in Table 2.7) together with the MASE42 
value of 1.02 suggests that double exponential smoothing tends to over forecast the value 
of the textile finished goods inventories and performs, on average, marginally worse than 
the reference forecasting method of random walk without drift.
1994
1600
1500
1800
1700
1995 1996 1997
Time (Months)
Textile Finished Goods Invetories
(millions of US dollars)
Long-Term Forecast
95.0% Prediction Intervals
Actual Inventories
In-Sample Forecast
Figure 2.6 Double Exponential Smoothing—In-Sample and Long Term Forecasts.

---

## Page 43

Table 2.7 In-Sample Forecasting Accuracy Measures—Double Exponential Smoothingα 0.821
β 0.025
MSET 338.6
Month 
t 
Month 
Index Y
t S t T t Y t e t ME t A t MAE t MSE t RMSE t % |et| MAPEt MASE t TS t
Jul-93 1 1,516
Aug-93 2 1,525 1,525.0 9.0
Sep-93 3 1,506 1,511.0 8.4 1,534.0 –28.0 –28.0 28.0 28.0 784.0 28.0 1.9 1.9 – –1.00
Oct-93 4 1,510 1,511.7 8.2 1,519.4 –9.4 –18.7 9.4 18.7 436.6 20.9 0.6 1.2 4.68 –2.00
Nov-93 5 1,501 1,504.4 7.8 1,519.9 –18.9 –18.8 18.9 18.8 410.3 20.3 1.3 1.2 2.89 –3.00
Dec-93 6 1,563 1,553.9 8.9 1,512.2 50.8 –1.4 50.8 26.8 952.3 30.9 3.2 1.7 1.07 –0.21
Jan-94 7 1,576 1,573.6 9.2 1,562.8 13.2 1.5 13.2 24.1 796.9 28.2 0.8 1.6 1.09 0.32
Feb-94 8 1,606 1,601.8 9.6 1,582.8 23.2 5.1 23.2 23.9 753.8 27.5 1.4 1.5 1.01 1.29
Mar-94 9 1,597 1,599.6 9.3 1,611.5 –14.5 2.3 14.5 22.6 676.1 26.0 0.9 1.5 1.07 0.73
Apr-96 34 1,710 1,711.5 7.2 1,718.6 –8.6 –2.7 8.6 13.8 306.0 17.5 0.5 0.9 1.03 –6.23
...
May-96 35 1,691 1,696.0 6.6 1,718.8 –27.8 –3.4 27.8 14.2 320.0 17.9 1.6 0.9 1.05 –8.00
Jun-96 36 1,688 1,690.6 6.3 1,702.6 –14.6 –3.8 14.6 14.2 316.9 17.8 0.9 0.9 1.07 –9.02
Jul-96 37 1,697 1,697.0 6.3 1,697.0 0.0 –3.7 0.0 13.8 307.9 17.5 0.0 0.9 1.05 –9.29
Aug-96 38 1,696 1,697.3 6.2 1,703.3 –7.3 –3.8 7.3 13.6 300.8 17.3 0.4 0.8 1.07 –9.95
Sep-96 39 1,717 1,714.6 6.5 1,703.5 13.5 –3.3 13.5 13.6 297.6 17.3 0.8 0.8 1.05 –8.96
Oct-96 40 1,682 1,689.0 5.7 1,721.0 –39.0 –4.2 39.0 14.3 329.9 18.2 2.3 0.9 1.05 –11.27
Nov-96 41 1,726 1,720.4 6.3 1,694.7 31.3 –3.3 31.3 14.7 346.6 18.6 1.8 0.9 1.02 –8.81
Dec-96 42 1,732 1,731.0 6.4 1,726.7 5.3 –3.1 5.3 14.5 338.6 18.4 0.3 0.9 1.02 –8.58
Note: Entries for time periods t 
∈ [10, 33] are not shown due to space constraints.

---

## Page 44

Forecasting  33
TRIPLE EXPONENTIAL SMOOTHING
The triple exponential smoothing method performs well on time series that show sig-
nificant linear trends and seasonality patterns. To account for seasonality, a third equa-
tion supplements the revised smoothed mean and trend formulae provided in equation 
(2.18). Since the type of seasonality present in the data impacts the expressions for the 
forecasts and the recursive updates, in what follows, we explore and point out the differ-
ences between possible seasonal patterns.
Often, time series exhibit a seasonal behavior that repeats every f period. For example, 
the annual auto sales in the United States have been shown to be steady during the first 
seven months (i.e., January through July), experience a significant increase during the 
months of August and September followed by a significant drop in October and Novem-
ber and return to the steady levels in December. While this pattern occurs every year (i.e., 
f = 12 months), the steady levels and/or the relative sales increases or decreases noticed 
throughout the year may change from one year to the next.
Relative to the annual monthly average, the sales in August and September may depict 
a 25K unit increase every year irrespective of the overall annual performance. Thus, the 
monthly activity is insensitive to the economic environment that leads to an above or 
below annual performance. The seasonality in this case is said to be additive. Hence, 
if the annual monthly average is computed (forecast), the August and September per-
formance could easily be estimated by adding 25K units to the average baseline. Con-
versely, the sales for August and September may consistently show a 15% increase over 
the annual monthly average. In this case, the monthly activity reflects the overall annual 
performance. Mediocre annual sales result in mediocre, but still above average, August/
September sales. Similarly, high annual sales translate into very strong August/Septem-
ber sales. Hence, the seasonality patterns are said to be multiplicative.
In practice, the identification of the underlying type of seasonality is not a trivial task. 
The visual exploration of time series data, however, can be helpful in the discovery of 
the proper seasonal patterns. An example of hypothetical additive and multiplicative 
patterns is provided in Figure 2.7. In panel A, which depicts an additive seasonality, the 
sales data show similar absolute value quarterly fluctuations from one year to the next. 
In contrast, as shown in panel B, the multiplicative seasonality implies that the quarterly 
fluctuations vary based on the absolute values of the time series.
Dependent on how seasonality is approached, the equations for the forecasts and the 
recursive updates for the triple exponential smoothing are described by one of the fol-
lowing sets of analytical expressions:
Additive Seasonality:
 ˆ
modYS h T s
SY s
th t t tf h f
tt t f
+ −+ + − ()
++ + −
=+ ⋅+
=⋅ −() +−()
11
11 1 1
  
αα ⋅⋅ +()
=⋅ −() +−() ⋅
=⋅ −() +−()
++
++ +
ST
TS S T
sY S
tt
tt t t
tt t
11
11 1
1
1
ββ
γγ ⋅⋅+−stf 1
 (2.19)

---

## Page 45

34  Forecasting
Multiplicative Seasonality:
 ˆ
modYS h T s
SY s
th t t tf h f
tt t f
+ −+ + − ()
++ + −
=+ ⋅() ⋅
=⋅ () +−(
11
11 1 1
  
αα ) )⋅+()
=⋅ −() +−() ⋅
=⋅ () +−()
++
++ +
ST
TS S T
sY S
tt
tt t t
tt t
11
11 1
1
1
ββ
γγ ⋅⋅+−stf 1
 (2.20)
where t, 0 ≤ t ≤ T, is the current time period, f is the periodicity of the time series, Yt+1 
is the newly observed value of the time series at time t + 1, st and st+1 are the smoothed 
means of the time series at times t and t + 1, respectively, Tt and Tt+1 are the estimates for 
trend computed at times t and t + 1, respectively, st+1 and st+1– f are the seasonal param-
eters for the season corresponding to period t + 1 computed at t + 1 and t + 1– f, respec-
tively, st – f +1+(h–1) mod f is the last updated seasonal parameter for the season corresponding 
to period t + h (mod is the modulo operator), Yˆ
t+h is the forecast for time instances t 
+ h, h ≥ 1, computed at time t and α, β and γ are smoothing parameters with values 
between 0 and 1. Note that in equations (2.19) and (2.20), the updated estimates for the 
smoothed mean, trend and seasonal parameters are all weighted averages of the observed 
values and the old estimates. As with the simple and double exponential smoothing, if 
T provides the length of the time series, the forecasts Yˆ
t+h computed for periods t < T are 
all in-sample forecasts. Further, if h = 1, the forecasts are the one-step-ahead in-sample 
forecasts. Typically, the α, β and γ parameters are optimized over forecasting accuracy 
measures calculated using the in-sample actual observations. For t = T and h ≥ 1, ST + h . 
TT + sT – f +1+(h–1) mod f or (ST + h . TT) · sT – f +1+(h–1) mod f provides an estimate for the long-term 
forecasts for all time periods in the future.
The recursive formulae shown in equations (2.19)–(2.20) and the subsequent results 
depend upon the values assigned to S0, T0 and the initial seasonal parameters sk
0, k ∈ [1, f], 
0
2004 2006
Time (Quarter) Time (Quarter)
A. Additive Seasonality B. Multiplicative Seasonality
Quarterly Sales (thousands)
Quarterly Sales (thousands)
2008
100
200
300
0
2004 2006 2008
100
200
300
Actual Sales
Annual Average Sales
Figure 2.7 Additive and Multiplicative Seasonality.

---

## Page 46

Forecasting  35
k integer. To fit the purpose of these recursive formulae, the starting seasonal parameters 
sk
0 are operationalized as sk, k ∈ [–f + 1, 0], k integer, where s1
0 corresponds to s– f +1, s2
0 to 
s– f +2, and, finally, s f
0 to s0. To initialize S 0 and T0, a linear model is usually fitted to the 
first few multiple of f observations of the time series. The resulting intercept and slope 
are then assigned to S0 and T0, respectively. Next, the initial seasonal parameters s k
0 (or, 
sk) are computed from the data de-trended based on the fit of this linear model. Since the 
estimation of the linear slope in the presence of seasonality typically leads to biased trend 
estimates, we discuss an alternative initialization procedure that is robust and relies on 
the decomposition of the time series. In particular, to seasonally adjust some of the data, 
we fit a centered weighted moving average of order f + 1, or, equivalently, a 2 x f centered 
moving average, to the first few multiple of f observations of the time series. In this setup, 
all but the first and the last observations in the rolling window of size f + 1 are weighed by 
1/f. The two exceptions are weighed by 1/(2 . f). As before, we fit next a linear model to 
these seasonally adjusted data to get the initial estimates for S
0 and T0. The initial seasonal 
parameters sk
0 are then computed by referencing, either additively or multiplicatively, 
the deseasonalized data to the corresponding actual time series observations. The results 
of this referencing process are averaged over all present seasons and then normalized 
to sum to 0 (additive seasonality) or f (multiplicative seasonality) to finally lead to the 
seasonal parameters s
k
0. In the discussion above, the seasonal adjustment formulated in 
terms of the centered weighted moving average of order f + 1 is particularly attractive 
given that most seasonal time series show an even periodicity (e.g., f = 4 for quarterly 
data, f = 12 for monthly data). For the cases where periodicity is an odd integer, the cen-
tered weighted moving average of order f + 1 is replaced in our initialization procedure 
by a simple centered moving average of order f. No other changes are needed in order for 
the procedure to compute initial estimates for the parameters S0, T0 and sk
0.
To avoid overfitting problems—possibly due to estimating S0, T0 and sk
0 and comput-
ing forecasts Yˆ
t+h on the same data subset—we revise the recursive formulae of equations 
(2.19) and (2.20) to iterate over all periods t, f ≤ t ≤ T where Sf = S0, Tf = T0 and sk = sk
0, 
1 ≤ k ≤ f. To provide the reader with some reference points, we acknowledge that this 
initialization procedure is coded in the specific functions provided with the base distri-
bution of the environment for statistical computing R (R Core Team, 2013). In practice, 
slightly different variants of this approach are also routinely used (see, e.g., Hyndman 
et al., 2008; Makridakis et al., 1998); the work of Hyndman et al. (2008), for instance, is 
implemented in the package forecast, one of R’s many contributed libraries (Hyndman 
& Khandakar, 2008; Hyndman, Razbash, & Schmidt, 2012).
The presence of seasonality in the time series data leads to very distinct patterns in the 
long-term forecasts. As with the other exponential smoothing methods, the prediction 
intervals for triple exponential smoothing also display variable widths with more accu-
rate forecasts being produced for time periods immediately following the actual time 
series data. A relevant multiplicative seasonality example is provided in Figure 2.8 which 
looks at the monthly totals of international airline passengers between 1949 and 1952 
(Box, Jenkins, & Reinsel, 1994, Series G). This time series shows a periodicity f of 12 
months.
The construction of the forecast lines in Figure 2.8 is detailed in Table 2.8 and Table 
2.9. We estimate the initial parameters S
0, T0 and sk
0 using the time series data for 1949 
and 1950. We start by fitting a centered weighted moving average of order 13 (i.e., 
CW-MA(f + 1)= CW-MA(13)) to all monthly data entries in this time period for which

---

## Page 47

36  Forecasting
support data exist. In particular, all monthly observations Yt between July 1949 and June 
1950 can be deseasonalized using the weights provided in the upper part of Table 2.8. 
In this setup, the deseasonalized value of 126.79K for July 1949, for example, is com-
puted by weighting and averaging the monthly totals of international airline passengers 
reported for the period in between and including January 1949 and January 1950. Using 
the resulting deseasonalized figures, we determine S
0 and T0 by estimating a linear regres-
sion model that expresses the expected deseasonalized monthly passenger totals as a 
function of time. With the monthly indices replaced by a vector of f consecutive integers 
that starts at 1, we obtain the linear model E (CW-MA (13))=124.32 + 1.15 t which we 
depict in Figure 2.9. Following the standard approach, we assign the linear intercept of 
124.32K to S
0 and the slope of 1.15K to T0. Next, we compute some intermediate seasonal 
parameters sk
0– by dividing the actual monthly data by the deseasonalized monthly val-
ues. For July 1949, the value of 1.17 for sk
0– is computed by dividing the actual number of 
passengers of 148K by the corresponding deseasonalized value of 126.79K. To compute 
the starting seasonal parameters s
k
0, we normalize sk
0– (through division by the average of 
sk
0–) such that the sum of sk
0 is f, or, in this case, 12. Thus, sk
0 that corresponds to July 1949 
becomes 1.18. By reordering the sk
0 values to account for the natural order of the months 
in a year, we obtain the starting seasonal parameters sk
0 for the airline passenger problem 
which we show on the right side of Table 2.8.
Continuing the international airline passengers example, at time  t = f = 12, the fore-
cast for all subsequent time periods can be computed as Yˆ
t+h = (St + h . Tt) . st – f +1+(h–1) 
mod f, or, equivalently, as Yˆ
f+h = (Sf + h . Tf) . s1+(h–1) mod f = (S0 + h . T0) . s1+(h–1) mod f . Hence, 
the one-step-ahead forecast for period t = 13 becomes Yˆ
13=(S0 + T0) s1, or, 111.1K. The 
difference of about 0.6K between the reported forecast of 111.1K and the forecast com-
puted by directly replacing S
0, T0 and s1 in the expression of Yˆ
13 are due to rounding 
errors. Once the monthly total of 115K for January 1950 becomes current, we update 
1949
150
50
100
200
250
1950 1951 1952 1953 1954
Time (months)
International Airline Passengers
(thousands)
Long-Term Forecast
95.0% Prediction Intervals
Actual Number of Passengers
In-Sample Forecast
Figure 2.8 Triple Exponential Smoothing—In-Sample and Long Term Forecasts.

---

## Page 48

Forecasting  37
the estimates for the smoothed mean, trend, and seasonal parameters such that S 13= 
α · (Y13 / s1) + (1– α) · (S12 + T12), T13 = β · (S13 – S12) + (1– β) · T12 and s13 = γ · (Y13 / 
S13) + (1 – γ) · s1. For an α of 0.215, β of 0.107 and γ of 0.109, S13, T13 and s13 evaluate to 
126.41K, 1.25K and 0.89, respectively. With these estimates in place, the forecasts for 
all future time periods h can be computed using Yˆ
13+h = (S13 + h . T13) . s13– f +1+(h–1) mod f . 
As for the simple and double exponential smoothing, the iterative process of comput-
ing the in-sample forecasts Yˆ
t+h and updating St+1, Tt+1 and st+1 repeats for all remaining 
monthly data points t present in the time series. The final smoothed mean ST = S48 and 
trend TT = T48 together with the set of the last f seasonal parameters {s 37, …, s48} help 
one compute the long-term forecasts Yˆ
T+h, h ≥1. For example, the forecasts for January 
and February 1953 are given by Yˆ
T+1 = (S T + TT) · s37 and Yˆ
T+2 = (S T + 2 · TT) · s38 and 
equal 190.71K and 206.25K, respectively.
Table 2.8 Triple Exponential Smoothing—Initialization of Seasonal Parameters
Weights for the rolling window of the centered weighted moving average of order f +1
w1 w2 w3 w4 w5 w6 w7 w8 w9 w10 w11 w12 w13
0.042 0.083 0.083 0.083 0.083 0.083 0.083 0.083 0.083 0.083 0.083 0.083 0.042
Computation of seasonal parameters sk
0–
Month
       t
Month
index Y
t CW – MA (13) sk
0– sk
0 Season sk
0
Jan-49 1 112 Jan 0.89
Feb-49 2 118 –––––––––––h Feb 0.96
Mar-49 3 132 Mar 1.06
Apr-49 4 129 Apr 1.00
May-49 5 121 May 0.92
Jun-49 6 135 Jun 1.09
Jul-49 7 148 126.79 1.17 1.18 Jul 1.18
Aug-49 8 148 127.25 1.16 1.18 Aug 1.18
Sep-49 9 136 127.96 1.06 1.07 Sep 1.07
Oct-49 10 119 128.58 0.93 0.94 Oct 0.94
Nov-49 11 104 129.00 0.81 0.81 Nov 0.81
Dec-49 12 118 129.75 0.91 0.92 Dec 0.92
Jan-50 13 115 131.25 0.88 0.89
Feb-50 14 126 133.08 0.95 0.96
Mar-50 15 141 134.92 1.05 1.06
Apr-50 16 135 136.42 0.99 1.00
May-50 17 125 137.42 0.91 0.92
Jun-50 18 149 138.75 1.07 1.09
Jul-50 19 170
Aug-50 20 170
Sep-50 21 158
Oct-50 22 133
Nov-50 23 114
Dec-50 24 140
Yt is expressed in thousands.

---

## Page 49

Table 2.9  In-Sample Forecasting Accuracy Measures—Triple Exponential Smoothingα 0.215
β 0.107
γ 0.109 h Seasonal index used in the revised recursive formula of equation (2.20) 
MSET 45.2 h Monthly seasonal index (s1—season 1, s2—season 2, etc.)
Month 
t 
Month 
Index Y
t S t T t I s* I s** s t Y ˆt e t ME t A t MAE t MSE t RMSE t % |et| MAPEt MASE t TS t
Jan-49 1 112 s1 s1
0 0.89
Feb-49 2 118 s 2 s2
0 0.96
Mar-49 3 132 s 3 s3
0 1.06
Apr-49 4 129 s 4 s4
0 1.00
May-49 5 121 s 5 s5
0 0.92
Jun-49 6 135 s 6 s6
0 1.09
Jul-49 7 148 s 7 s7
0 1.18
Aug-49 8 148 s 8 s8
0 1.18
Sep-49 9 136 s 9 s9
0 1.07
Oct-49 10 119 s 10 s10
0 0.94
Nov-49 11 104 s 11 s11
0 0.81
Dec-49 12 118 124.32 1.15 s 12 s12
0 0.92
Jan-50 13 115 126.41 1.25 s 13 s1 0.89 111.1 3.9 3.9 3.9 3.9 15.4 3.9 3.4 3.4 – 1.00
Feb-50 14 126 128.53 1.34 s 14 s2 0.96 122.1 3.9 3.9 3.9 3.9 15.2 3.9 3.1 3.2 0.35 2.00
Mar-50 15 141 130.65 1.42 s 15 s3 1.06 137.1 3.9 3.9 3.9 3.9 15.1 3.9 2.7 3.1 0.30 3.00
...
Nov-52 47 172 207.42 2.40 s 47 s11 0.81 167.4 4.6 1.4 4.6 5.5 46.5 6.8 2.7 3.2 0.37 8.97
Dec-52 48 194 209.98 2.42 s 48 s12 0.92 193.3 0.7 1.4 0.7 5.4 45.2 6.7 0.4 3.2 0.36 9.33
Yt expressed in thousands.
Note: Entries for time periods t 
∈ [16, 46] are not shown due to space constraints.

---

## Page 50

Forecasting  39
The one-step-ahead in-sample forecasts Yˆ
t+1, t < T , together with the actual values 
of the time series are used to compute the in-sample forecasting accuracy measures of 
which we present the relevant ones in the right-most columns of Table 2.9 . As in the 
previous examples, we compute the smoothing parameters α, β and γ such that the in-
sample mean squared error MSE48 is minimized. Specifically, the smoothing parameter 
values of 0.215, 0.107 and 0.109 for α, β and γ lead in this case to a minimum MSE48 
of 45.2K. Relative to the range of the observed monthly passengers totals, the MAE48 
of 5.4K and the MAPE48 of 3.2% suggest that the forecasts fit well the seasonal profile 
present in the data. A strong forecasting performance is also advocated by the MASE48 
value of only 0.36 which implies that triple exponential smoothing performs superior 
to the naïve forecasting method of random walk without drift. In spite of the apparent 
methodological fit, however, a closer look at how the tracking signal evolves as more 
data becomes available (only partially available in Table 2.9) reveals that the triple expo-
nential smoothing tends to consistently under forecast which could be a sign that the 
forecasting method is inadequate or that the underlying demand patterns are changing 
and making the history less suitable for the task at hand. The information on the tracking 
signal being out of bounds is often an indication that a thorough review of the current 
forecasting practices is needed. For completeness, we highlight that we do not provide in 
Table 2.9 the full-time profiles of the tracking signal as well as of all the other forecasting 
accuracy measures due to space constraints.
CASE STUDY: FORECASTING SPSS MANUAL SALES
In the late 1990s, SPSS Inc., a U.S. technology company, received worldwide recogni-
tion for its flagship software product SPSS (Statistical Product and Service Solutions). 
In 2008, a year before its acquisition by International Business Machines Corporation 
(IBM), SPSS Inc. reported sales of over a quarter of a billion US dollars (Dicolo, 2009) 
and served some 250,000 customers. Today, the statistical software SPSS, conveniently 
rebranded as IBM SPSS, is one of the many software packages available for statistical 
analysis. In social sciences, IBM SPSS competes with other proprietary or open source 
2
130
125
140
135
E(CW−MA(13)) = 124.32+1.15∙t
468 1 0 1 2
Reset Month Index
CW-MA(13) (thousands)
Seasonally Adjusted Number of Passengers
E(.)- Expected Value Operator
Linear Model
Figure 2.9 Triple Exponential Smoothing—Initialization of S0 and T0.

---

## Page 51

40  Forecasting
statistical software packages including SAS (SAS Institute Inc., 2012), Stata (StataCorp, 
2012) or R (R Core Team, 2013).
Although a comparative analysis of the forecasting capabilities of these software pro-
grams would appeal to the statistics’ enthusiast, in this section, we focus on something 
else. In particular, we raise some general methodological awareness by using an example 
that deliberately builds on the SPSS Inc.’s early market experiences. In this context, we 
illustrate how a forecasting problem should be approached by using the sales of the SPSS 
manual as an example (Nie, Bent, & Hull, 1970). We selected this example partly because 
of the instrumental role the SPSS manual played in the advancement of research theory 
and practice in many areas of the social sciences. For instance, as a tribute to its signifi-
cant contribution to the progress in sociology, the SPSS manual has been suggested to 
be the most influential book in this field (Wellman, 1998). In our work, we focus on 
the sales of the second edition of the SPSS manual which was published and distributed 
by McGraw-Hill Inc. We report on the quarterly sales performance of this manual for 
the period that covers the time between Quarter 1 of 1976 and Quarter 4 of 1982 (for 
details, see Figure 2.10). This data set is publicly available at the DataMarket’s website, 
www.datamarket.com (Hyndman, 2012). At least visually, the data show a slight positive 
trend and annual seasonal patterns with peaks in Quarter 3. While Quarters 1 and 2 are 
consistently lagging behind, Quarter 4 shows high instability and alternates between low 
and high sales performance states. Overall, the data seem to be rather noisy.
With this background information in mind, let’s assume that you are a publisher with 
McGraw-Hill Inc. who is responsible for managing the 1983 post-secondary education and 
professional products both in the United States and internationally. The market for these 
products deals with three main product categories differentiated by the target audience 
and the geographic coverage. The second edition of the SPSS manual is part of the Higher 
Education product category which publishes about 500 titles. The other two product cat-
egories are Professional and International products. To fulfill the requirements of your job, 
you must provide the printing department at McGraw-Hill Inc. with quarterly estimates 
1976Q1
5000
0
15000
1978Q1 1980Q1 1982Q1
Time (quarters)
Sales of SPSS Manual (2nd. Edition)
Sales of SPSS Manual
Sales of SPSS Manual (1st Quarter of the Year)
Figure 2.10 Sales of SPSS Manual (2nd Edition).

---

## Page 52

Forecasting  41
of what they need to print at least a year in advance. Of these estimates, only the one for 
the next quarter goes into production; the other three are used for a rough cut capacity 
check and are allowed to change once the updated information for the next four quarters is 
ready and delivered. As the year 1982 is about to end, your task is to decide on the quarterly 
figures that need to be forwarded to the printing department. In what follows, we exam-
ine only the case of the second edition of the SPSS manual; however, some of other titles 
McGraw-Hill Inc. sells (e.g., staple-like titles that are not newly introduced or about to be 
retired) are expected to perform similarly so our discussion is relevant for them as well.
To accomplish the task, you could rely on your sound knowledge of the market and 
the characteristics of this particular title. You could then form an expectation of the 
title’s likely future performance and—based on your intuition—recommend the print-
ing department a set of expected quarterly sales. One drawback to this approach, how-
ever, is that your estimates could not be defended on any objective grounds. A differ-
ent publisher within the company with the same or slightly different knowledge of the 
market and the product would probably find just enough reasons to prove that you are 
wrong and could miss some significant profit opportunities. In addition, if you were 
asked to repeat the process again in slightly different circumstances, you could end up 
recommending different quarterly figures. To remove some of the inherent biases asso-
ciated with this intuition-driven forecasting, you could opt for a more analytical proce-
dure to compute the required sales estimates. In particular, if the business environment 
around this specific title is believed to be stable (e.g., an SPSS release with a redesigned 
manual is not scheduled to take place in the coming year), you could employ the tech-
niques discussed in sections 2.4–2.7 to forecast the 1983 sales of the SPSS manual. If such 
an approach is desired, you still need to decide on which of the competing techniques to 
use and evaluate what the magnitude of the expected error is.
To help select the appropriate forecasting technique and get a sense of the magnitude 
of the expected error, first split the data set into an estimation (1976Q1–1980Q4) and a 
validation (1981Q1–1982Q4) sample. Use the estimation sample to optimize the values 
of the smoothing parameters for the simple, double and triple (with additive and mul-
tiplicative seasonality) exponential smoothing by minimizing the mean squared error 
corresponding to the fourth quarter of 1980. Next, employ the optimized smoothing 
parameters to compute the one-step-ahead forecasts on the validation sample and evalu-
ate the forecasting accuracy measures on both estimation and validation samples. Given 
how the forecasts are computed, the accuracy measures on the validation sample are 
more representative than those on the estimation sample of the error likely to be experi-
enced for future sales. We provide a pictorial representation of the one-step-ahead fore-
casts in Figure 2.11 and show the values of the smoothing parameters and the forecast-
ing accuracy measures in Table 2.10. Across all forecasting techniques, the forecasting 
accuracy measures are better on the validation sample than on the estimation sample, 
probably because the data stabilizes toward the end of the observed time window. In 
general, however, the reverse behavior is to be expected. As seen by comparing the results 
in Table 2.10, the simple and double exponential smoothing are outperformed by the 
triple exponential smoothing, in particular because the former are unable to describe the 
seasonality patterns present in the data. Of the two triple exponential smoothing tech-
niques, both could be employed to produce forecasts, although, the one with additive 
seasonality seems to perform slightly better. In what follows, we use the triple exponen-
tial smoothing with additive seasonality to compute the 1983 forecasts.

---

## Page 53

42  Forecasting
1976Q1
Holdout Sample
(1981Q1–1982Q4)
Estimation Sample
(1976Q1–1980Q4)
10000
0
5000
15000
20000
1978Q1
SES, DES, TES-A and TES-M: Simple, Double, Triple (Additive) and Triple
(Multiplicative) Exponential Smoothing
1980Q1 1982Q1
Time (quarters)
Sales of SPSS Manual (2nd. Edition)
One-Step-Ahead Forecasts SES One-Step-Ahead Forecasts TES −A
One-Step-Ahead Forecasts TES−MOne-Step-Ahead Forecasts DES
Figure 2.11 Sales of SPSS Manual (2nd Edition)—One-Step-Ahead Forecasts.
Table 2.10 Sales of SPSS Manual (2nd Edition)—Smoothing Parameters and Forecasting Accuracy Measures
Estimation Sample: Optimal Smoothing Parameters (min MSE1980Q4)
Forecasting Method αβ γ MSE1980Q4
Simple Exponential Smooting 0.219 – – 13,500,997.8
Double Exponential Smoothing 0.123 1.000 – 14,423,085.0
Triple Exponential Smoothing 
     Additive Seasonality
0.065 0.000 0.805 11,732,441.6
Triple Exponential Smoothing 
    Multiplicative Seasonality
0.052 0.000 0.799 12,886,604.9
Forecasting Accuracy Measures for Model Selection
Forecasting Method ME MAE MSE MAPE Decision
Simple Exponential Smooting
Estimation Sample 1,170.8 3,189.9 13,500,997.8 33.0% No
Holdout Sample 1,171.7 2,874.3 10,522,195.6 24.9%
Double Exponential Smoothing
Estimation Sample –570.2 3,402.1 14,423,085.0 41.3% No
Holdout Sample 629.0 2,657.3 9,130,187.7 24.4%
Triple Exponential Smoothing 
Additive Seasonality
Estimation Sample –703.7 2,400.6 11,732,441.6 25.6% Maybe
Holdout Sample –367.6 1,519.5 2,619,656.7 12.7%
Triple Exponential Smoothing 
Multiplicative Seasonality
Estimation Sample –870.1 2,551.1 12,886,604.9 26.7% Maybe
Holdout Sample –116.7 1,558.7 3,482,750.4 11.8%

---

## Page 54

Forecasting  43
After choosing the appropriate forecasting technique, it is now straightforward to 
compute the quarterly forecasts for 1983. To account for the most recent observed data, 
we make use of the entire data set to re-optimize the smoothing parameters α, β and γ so 
as to minimize the mean squared error for the fourth quarter of 1982. With the updated 
values for S
1982Q4, T1982Q4 and s1982Q1 through s1982Q4, we then compute the quarterly fore-
casts for 1983 which evaluate to 13,828.0, 10,039.5, 17,401.2 and 15,829.8, respectively. 
Of these, only the estimate for Quarter 1 will go to print; the others will be revised 
sequentially once more data become available and only the updated values will be used 
in production (e.g., just before Quarter 2 of 1983 starts, data for Quarter 1 become avail-
able and should be used to update Yˆ
1983Q2). Given how noisy the original time series is, it 
comes as no surprise that the prediction intervals around the quarterly point forecasts 
are quite large. We show the lower and the upper bounds of these intervals together with 
other relevant statistics in Table 2.11 and Figure 2.12. We computed these bounds based 
on the techniques described in Yar & Chatfield (1990) and Chatfield & Yar (1991). Most 
advanced statistical software packages will calculate these prediction intervals for you.
SUMMARY
In this chapter, we discuss topics that surround forecasting, a concept which we con-
sider central to the success of any proactive business’s decision making. In this context, 
we first provide evidence for why forecasting, or, even better, superior forecasting, is a 
sought-after capability that many organizations invest significant resources to acquire. 
The recent experience of companies such as Continental Airlines Cargo or Procter & 
Gamble, to name a few, is illustrative of the efforts and the gains that accompany the 
ambition to forecast better. We build on these success stories to stress the importance of 
not only the forecasting algorithms but also of the organizational structure that allows 
Table 2.11 Sales of SPSS Manual (2nd Edition)—1983 Forecasts
Optimal Smoothing Parameters (min MSE1982Q4)
Forecasting Method αβ γ MSE1982Q4
Triple Exponential Smoothing 
    Additive Seasonality
0.108 0.013 0.697 8,618,376.7
Forecasting Accuracy Measures
Forecasting Method ME MAE MSE MAPE
Triple Exponential Smoothing 
    Additive Seasonality
–555.5 2,041.4 8,618,376.7 21.0%
1983 Forecasts and 95% Prediction Intervals (PIs)
Lower Bound PI Forecasts Upper Bound PI
Quarter 1983Q1 8,056.5 13,828.0 19,599.4
Quarter 1983Q2 4,233.5 10,039.5 15,845.3
Quarter 1983Q3 11,560.2 17,401.2 23,242.1
Quarter 1983Q4 9,953.0 15,829.8 21,706.5

---

## Page 55

44  Forecasting
the forecasting process to function as a whole. The availability of the right data, the qual-
ity of the staff and the IT systems, and the commitment of the upper management team 
are all important to the point that they cannot be overlooked.
To provide the reader with a picture of how a typical forecasting task is to be tackled, 
we review the common approaches to forecasting (i.e., qualitative, quantitative or mixed) 
and comment on the fundamental dissimilarities among the most known extrapolative 
forecasting models. Since in many practical situations, decisions are made based on the 
point forecasts alone as if they were known with certainty (Dalrymple, 1987), we provide 
an in-depth coverage of the most common forecasting accuracy measures. We supple-
ment these insights with a thorough examination of the role the holdout samples play in 
forecasting applications. Since it helps avoid making unfit and, oftentimes, costly poor 
decisions, we recommend the use of holdout samples as the standard practice for assess-
ing the likely future performance of any type of forecasts or forecasting techniques.
Next, we focus on the technical intricacies of the most common of the time series 
forecasting techniques. We cover the moving average and the exponential smoothing 
methods which we link to environments that replicate closely the conditions in which 
the science engines of many production forecasting systems operate. We conclude the 
chapter with a case study example that builds on the early market experience of SPSS 
Inc., one of the most successful players in the market for statistical and analytical soft-
ware products.
It is our expectation that after going through this chapter, the reader should be able 
to:
1. Understand why forecasting is a critical business enabler.
2. Employ time series techniques to forecast future business developments based on 
historical data.
Long-Term Forecasts
95% Prediction Intervals
In-Sample One-Step-Ahead Forecasts
1976Q1
Forecast Window
(1983Q1–1983Q4)
Actual Sample
(1976Q1–1982Q4)
0
5000
15000
25000
1978Q1 1980Q1 1982Q1 1984Q1
Time (quarters)
Sales of SPSS Manual (2nd. Edition)
Figure 2.12 Sales of SPSS Manual (2nd Edition)—1983 Forecasts.

---

## Page 56

Forecasting  45
3. Select a preferred forecasting method from a set of candidate techniques.
4. Quantify the forecast errors to be experienced when forecasting the future.
REFERENCES
Akaike, H. (1974). A new look at the statistical model identification. IEEE Transactions on Automatic Control, 
19(6), 716–723.
Azoff, M. E. (1994). Neural network time series: Forecasting of financial markets. New York, NY: John Wiley & Sons, 
Inc.
Bowerman, B. L., O’Connell, R., & Koehler, A. (2004). Forecasting, time series, and regression: An applied approach 
(4th ed.). Belmont, CA: Thomson Brooks/Cole.
Box, G., & Jenkins, G. (1970). Time series analysis: Forecasting and control. San Francisco, CA: Holden-Day.
Box, G., Jenkins, G., & Reinsel, G. (1994). Time series analysis, forecasting and control (3rd ed.). Engelwood Cliffs, 
NJ: Prentice Hall.
Box, G., Jenkins, G., & Reinsel, G. (2008). Time series analysis, forecasting and control (4th ed.). Hoboken, NJ: John 
Wiley & Sons, Inc.
Brown, R. G. (1963). Smoothing, forecasting and prediction of discrete time series . Englewood Cliffs, NJ: 
Prentice-Hall.
Chatfield, C. (1988). Apples, oranges and mean square error. International Journal of Forecasting, 4(4), 515–518.
Chatfield, C., & Yar, M. (1991). Prediction intervals for multiplicative Holt-Winters. International Journal of Fore-
casting, 7(1), 31–37.
Cooper, W. L., Homem-de-Mello, T., & Kleywegt, A. J. (2006). Models of the spiral-down effect in revenue man-
agement. Operations Research, 54(5), 968–987.
Dalrymple, D. J. (1987). Sales forecasting practices: Results from a United States survey. International Journal of 
Forecasting, 3(3–4), 379–391.
Dicolo, J. A. (2009). IBM to acquire SPSS. Adding to acquisitions. The Wall Street Journal, 30 July.
EconStats. (February 17, 2012). US new orders, shipments and inventories—Nondurable goods. Retrieved March 8, 
2012, from www.econstats.com/nosi/nosi_a14s___m212.htm
Fisher, M. L., Hammond, J. H., Obermeyer, W. R., & Raman, A. (1994). Making supply meet demand in an uncer-
tain world. Harvard Business Review, 72(3), 83–93.
Fisher, M. L., & Raman, A. (2010). The new science of retailing: How analytics are transforming the suply chain and 
improving performance. Boston, MA: Harvard Business School Press.
Gardner, E. S. (2006). Exponential smoothing: The state of the art—Part II.  International Journal of Forecasting, 
22(4), 637–666.
Harvey, A. C. (1989). Forecasting, structural time series models and the Kalman filter . Cambridge, UK: Cambridge 
University Press.
Holt, C. C. (2004). Forecasting seasonals and trends by exponentially weighted moving averages (Reprint). Inter-
national Journal of Forecasting, 20(1), 5–10.
Hooker, R. H. (1901). Correlation of the marriage-rate with trade. Journal of the Royal Statistical Society,  64(3), 
485–492.
Hyndman, R. J. (2008). Evaluating peak demand forecasts (Report for Electricity Supply Industry Planning Council 
(SA) and Victorian Energy Corporation (VenCorp). Monash University Business and Economic Forecasting 
Unit.
Hyndman, R. J. (2012). Time Series Data Library. Retrieved November 15, 2012, from http://data.is/RDpkrd.
Hyndman, R. J., & Khandakar, Y. (2008). Automatic time series forecasting: The forecast package for R. Journal of 
Statistical Software, 27(3), 1–22.
Hyndman, R. J., & Koehler, A. B. (2006). Another look at measures of forecast accuracy.  International Journal of 
Forecasting, 22(4), 679–688.
Hyndman, R. J., Koehler, A. B., Ord, J. K., & Snyder, R. D. (2005). Prediction intervals for exponential smoothing 
using two new classes of state space models. Journal of Forecasting, 24(1), 17–37.
Hyndman, R. J., Koehler, A. B., Ord, K., & Snyder, R. (2008). Forecasting with exponential smoothing: The state 
space approach. Berlin, Heidelberg: Springer-Verlag.
Hyndman, R. J., Koehler, A. B., Snyder, R., & Grose, S. (2002). A state space framework for automatic forecasting 
using exponential smoothing methods. International Journal of Forecasting, 18(3), 439–454.
Hyndman, R. J., Razbash, S., & Schmidt, D. (2012). Forecast: Forecasting functions for time series and linear models. 
http://CRAN.R-project.org/package=forecast. R package version 3.19.
JDA Software Group. (2007). 
Achieving sky-high success. Retrieved February 8, 2012, from www.jda.com/File_bin/
casestudies/ContinentalAirlinesCargo.pdf.

---

## Page 57

46  Forecasting
Kahn, K. B. (2006). New product forecasting: An applied approach. Armonk, NY; London: M.E. Sharpe, Inc.
Kapuscinski, R., Zhang, R. Q., Carbonneau, P., Moore, R., & Reeves, B. (2004). Inventory decisions in Dell’s supply 
chain. Interfaces, 34(3), 191–205.
Linstone, H. A., & Turoff, M. (eds.). (2002). The Delphi method: Techniques and applications. Boston, MA: 
Addison-Wesley.
Makridakis, S. G. (1993). Accuracy measures: Theoretical and practical concerns. International Journal of Forecast-
ing, 9(4), 527–529.
Makridakis, S. G., Wheelwright, S. C., & Hyndman, R. J. (1998). Forecasting: Methods and applications (3rd ed.). 
New York, NY: John Wiley & Sons.
McCullagh, P., & Nelder, J. A. (1989). Generalized linear models (2nd ed.). London: Chapman & Hall/CRC.
McNelis, P. D. (2005). Neural networks in finance: Gaining predictive edge in the market . Burlington, MA: Elsevier 
Academic Press.
Microsoft. (2010). Microsoft Excel. Redmond, WA: Microsoft Corporation.
Moad, J. (2008). Recognizing demand forecasting success. Managing Automation, December 9.
Neter, J., Kutner, M., Nachtsheim, C., & Wasserman, W. (1999). Applied linear statistical models (4th ed.). Chicago, 
IL: Irwin/McGraw-Hill.
Nie, N., Bent, D., & Hull, C. H. (1970). SPSS: Statistical package for the social sciences. New York, NY: 
McGraw-Hill.
Pankratz, A. (1991). Forecasting with dynamic regression models. New York, NY: John Wiley & Sons.
R Core Team. (2013). R: A language and environment for statistical computing. Vienna: R Foundation for Statistical 
Computing. Retrieved from www.r-project.org/.
Rozell, J. (2007). Demand forecasting success. Hospitality Technology, November 1.
SAS Institute Inc. (2009). Reserve forecast aids in saving millions at America West Airlines. Retrieved November 15, 
2009, from www.sas.com/success/awa.html.
SAS Institute Inc. (2012). SAS software. Cary, NC: SAS Institute.
Schwarz, G. (1978). Estimating the dimension of a model. The Annals of Statistics, 6(2), 461–464.
Seifert, D. (2003). Collaborative planning, forecasting, and replenishment: How to create a supply chain advantage  
AMACOM, a Division of American Management Association.
StataCorp. (2012). Stata statistical software. College Station, TX: StataCorp LP.
The Apache Software Foundation. (2012). Apache OpenOffice.org. Forest Hill, MD: The Apache Software 
Foundation.
Weatherford, L. R. (1997). A review of optimization modeling assumptions in revenue management situations. 
AGIFORS Reservations and Yield Management Study Group, Montreal.
Weatherford, L. R., & Belobaba, P. P. (2002). Revenue impacts of fare input and demand forecast accuracy in air-
line yield management. The Journal of the Operational Research Society, 53(8), 811–821.
Wellman, B. (1998). Doing it ourselves: The SPSS manual as sociology’s most influential recent book. In D. Claw-
son (ed.), Required reading: Sociology’s most influential recent books (pp. 71–78). Amherst: University of 
Massachusetts Press.
Winters, P. R. (1960). Forecasting sales by exponentially weighted moving averages. Management Science, 6(3), 
324–342.
Yar, M., & Chatfield, C. (1990). Prediction intervals for the Holt-Winters forecasting procedure. International 
Journal of Forecasting, 6(1), 127–137.
Yule, G. U. (1909). The applications of the method of correlation to social and economic statistics. Journal of the 
Royal Statistical Society, 72(4), 721–730.
Zhang, P. G. (2004). Neural networks in business forecasting. Hershey, PA: Idea Group Publishing.

---

## Page 58

3
PROMOTION FORECASTING
INTRODUCTION
A basic underlying assumption when using the time series forecasting techniques 
described in the previous chapter is that demand is something that occurs and can-
not be influenced, at least in the short term, by the firm. This is a common approach 
taken by a production or operations department, as their primary concern has histori-
cally been how to set inventory or capacity levels to best meet some exogenous demand. 
A marketing department, however, typically views demand as the outcome of efforts 
and resources put into advertising, placement, and promotions. This is a fundamentally 
different mindset from a modeling standpoint, as demand becomes endogenous (and 
controllable) rather than exogenous (and uncontrollable). In practice, the truth typi-
cally falls somewhere in the middle. There is often some portion of demand that can be 
influenced by marketing efforts such as advertising, placements, and promotions but 
there is also some portion that cannot. Discerning how much demand can be influenced 
is the goal of promotion forecasting.
While there are thousands of studies on what exactly influences a consumer to pur-
chase a particular item, there is a general consensus that marketing actions such as adver-
tising (brand awareness, sponsorships, etc.), placement (end cap displays, location on a 
webpage, etc.) and promotion (buy-one-get-one-free, 50% off, etc.) play an important 
role for most consumer goods. Historically, it has been a major challenge to estimate 
how much of a role each plays. As an example, consider a grocery store manager decid-
ing between spending a limited marketing budget on an end-of-the-aisle display for a 
particular detergent brand or to offer a 25% discount on the brand. Both options are 
costly so the manager prefers to choose the most cost-effective option. The challenge is 
in estimating what the expected “lift” in sales will be for each option. While the manager 
may have offered these two different type promotions in the past (hopefully not always 
both at the same time), there is an inherent noisiness in the sales data that makes it dif-
ficult to attribute any particular sales lift specifically to each type of promotion. The tool 
that is most commonly used to accomplish this type of task is called regression analysis.
47

---

## Page 59

48  Promotion Forecasting
In this chapter, we introduce the method of regression analysis and show how the 
simplest versions (linear models) can be estimated using the common software pack-
age Microsoft Excel. We include promotions in our forecasts as an event rather than as 
a change in price, saving the discussion of including price effects for Chapter 6. While 
we only present the estimation of linear models in this chapter, the nonlinear, but often 
used, Logistic Regression is discussed in Appendix A along with the open-source sta-
tistical software package R, which can be used to estimate the more advanced models 
discussed in Chapters 6–8.
INTRODUCTION TO REGRESSION ANALYSIS
Regression is used for predicting (or explaining the relationship between) a single varia-
ble Y, called the response (or output or dependent) variable, using one or more predictor 
(or input, independent or explanatory) variables, X
1, …, Xn. Variables are, by definition, 
things that vary. Variables may vary on a continuous scale, such as the maximum tem-
perature over a set of days, but they can also vary on a discrete scale, or even categorically. 
An example of the latter could be the color of an automobile (red = 1, blue = 2, silver 
= 3, etc.). For our purposes, the response variable is typically sales of a product and the 
predictor variables often take the form of the prices offered or promotions run during 
the same time period when sales were recorded. Thus, the objective behind using regres-
sion is to explain as much of the variance of the response variable as possible using the 
variance of the predictor variables.
Linear Regression and the Least Squares Estimation Technique
The simplest type of regression analysis requires the use of a single predictor variable X  
to predict/explain the variable of interest Y . We formalize the relationship between X  
and Y such that
 Y
t = β0 + β1 · Xt + εt , (3.1)
or, equivalently,
 E [Yt] = β0 + β1 · Xt . (3.2)
In equations (3.1) and (3.2), t identifies the tth observation in the data set, Xt and Yt are 
the values of the predictor and response variables that correspond to the tth observation, 
εt is an error term assumed to have zero mean and variance σ2 (in addition, any two 
error terms εi and εj are considered to be uncorrelated), E[.] is the expectation operator 
and β0 and β1 are unknown parameters often referred to as the regression coefficients. 
The assumptions imposed on the error term εt imply that the observed responses Yt are 
realizations from random variables with means E[Yt] = β0 + β1 · Xt  and variances σ2. The 
functional relationship (3.2) between X and E[Y] is of the same form as the familiar 
equation for a line, y = b + m · x, with β0 (≡ b) representing the intercept (i.e., where the 
line crosses the y-axis) and β1 (≡ m) representing the slope of the line. More formally, β0 
provides the mean of the random variable that describes the response at X = 0. In this 
context, β0 is of interest only when X = 0 is within the scope of the model; for cases when 
the model is oblivious of what happens around X = 0, β0, although estimable, carries

---

## Page 60

Promotion Forecasting  49
no particular meaning. In contrast to how β0 may or may not communicate a concrete 
meaning, β1 always reflects the change in the mean of the response random variable  Y 
due to a unit increase in X.
Returning to our example from Chapter 2 of predicting the daily sales of frozen cus-
tard at one of Rita’s Ice Cream stores, we can model the (hypothesized) linear relation-
ship between sales on day t (Salest) and the daily average temperature (DATt) by
 Sales t = β0 + β1 · DATt + εt , (3.3)
where t, εt, β0 and β1 carry the same meaning as in equations (3.1) and (3.2). For com-
pleteness, we highlight that the error terms εt in equations (3.1) and (3.3)  capture the 
effect on Yt of all relevant variables not included in the model due to their not being 
observed.
The linear regression model (3.1) (or, equivalently, (3.2)) is typically estimated by 
finding the regression coefficients β0 and β1 that minimize the sum of the squared devia-
tions of Yt from their expected values E[Yt]. For a data set consisting of N observed pairs 
(Xt, Yt),1 ≤ t ≤ N the sum of squared deviations amounts to
which for Rita’s becomes QS a l e s D A Ttt
t
N
=− + ⋅ ()()
=
∑ ββ01
2
1
. This estimation technique
is commonly referred to as the method of least squares because it minimizes the sum 
of the squared vertical distances from the actual values of the response variable to the 
fitted regression line (see Figure 3.1). To provide an intuition for how the estimation 
criterion Q for Rita’s varies with the regression coefficients, we color plot in Figure 3.2 its 
values across a limited range of β0s and β1s. The darker regions in this plot identify pairs 
(β0, β1) for which Q is far from its minimum value Qmin. On the lighter regions of the plot, 
which show all Q values that are close to Qmin, we depict a few representative curves of a 
contour plot to illustrate how Q eventually reaches its minimum value Qmin of 4,056.012. 
The parameter estimates βˆ
0 and βˆ
1 for which Qmin is obtained can be computed analyti-
cally as:
 
β1
1
2
1
1=
−() ⋅−()
−()
=
−() ⋅−
=
=
=
∑
∑
∑XXY Y
XX
DAT DAT Sales St
t
N
t
t
t
N
t
t
N
t aales
DAT DAT
YX S a l e s D A T
t
t
N
()
−()
=
=− ⋅= − ⋅ = −
=
∑
2
1
01 1
6 0728.
ββ β 253.4 4986,
 
(3.4)
where X−, Y−, DAT = 83.38 (degrees F) and Sales = 252.86 (units) are the means of Xt, Yt, 
DATt and Salest, respectively.
QY E Y Y Xtt
t
N
tt
t
N
=− []() =− + ⋅ ()()
==
∑∑
2
1
01
2
1
ββ
ˆ
ˆ ˆ

---

## Page 61

50  Promotion Forecasting
With βˆ
0 and βˆ
1 estimated, we can easily form an expectation about the mean of the 
response random variable that corresponds to any level of the response variable  X (i.e., 
Yˆ
t = βˆ
0 + βˆ
1 · Xt). However, without knowing the variance σ2, we cannot fully describe 
the distribution of Y given X. Similarly, we cannot make any valid inferences in regard 
to the estimates βˆ
0, βˆ
1, or, the regression line in general. To facilitate all these tasks, we 
need to estimate σ2 using the available data. For the linear regression model (3.1), the 
best estimate for σ2 is provided by:
60
23
3.7
1.4
5.3
8.2
5.1
9.1
3
21
19
126.9
−3.6
−6.3
−1.6
−26
−19
−30
−9.8
−10−10
150
200
250
300
350
70 80
Daily Average Temperature (F)
Ice Cream Sales (units)
90 100
Actual Sales Values Fitted Regression Line Deviations εt
−253.510
6.0726
6.0727
6.0728
β1 = 6.0728 Qmin = 4,056.012^
β0 = 253.4986^
6.0729
6.0730
−253.505 −253.500
β
0
β1
−253.495 −253.490
Figure 3.1 Illustration of the Deviations in the Linear Regression Analysis.
Figure 3.2 Estimation of Regression Coefficients via the Least Squares Method.

---

## Page 62

Promotion Forecasting  51
 
σ
ββ
2
01
2
1
2=
−+ ⋅()()
−
=
∑ YX
N
tt
t
N
 
(3.5)
where βˆ
0 + βˆ
1 · Xt is an estimate of the mean of the response random variable Y com-
puted at the level Xt of the response variable X, (Yt – (βˆ
0 + βˆ · Xt))2 provides the squared 
deviation of Yt from its mean estimate (βˆ
0 + βˆ
1 · Xt), and the integer 2 in the denominator 
adjusts the number of available observations over which the mean squared deviation is 
computed to reflect that two other parameter estimates (i.e., βˆ
0 and βˆ
1) must be com-
puted before the estimation of σ2 is to take place. For Rita’s, equation (3.5) becomes:
 
σ
ββ
2
01
2
1
22
4 056 012
19 213=
−+ ⋅()()
− = − ===
∑ Sales DAT
N
Q
N
tt
t
N
min ,. .447 . (3.6)
Hence, the estimate of the standard deviation of the probability distribution 
of the response random variable Y at any level of the predictor variable X is given by 
σˆ  = √σˆ 2 = √213.47 = 14.61 (units). Relative to the means of the distributions of Y (i.e., 
Yˆ
t = βˆ
0 + βˆ
1 · Xt), which cover within the scope of X in a range between 129.1 and 
353.8 units, the estimate of the standard deviation appears to be quite small, a finding 
that suggests that the average daily temperature explains the majority of the variation 
observed in daily sales. Analytical expressions similar to those provided in equations 
(3.4) and (3.5)  are available to compute the estimates for the regression coefficients 
β and the variance σ2 when several predictor variables X (i.e., X 1,…, Xn) are used to 
explain/predict the response variable  Y. These expressions are provided in many text-
books that cover the concepts of regression analysis (see, e.g., Cohen, Cohen, West, 
& Aiken, 2003; Kutner, Nachtsheim, & Neter, 2004; Neter, Kutner, Nachtsheim, & 
Wasserman, 1999).
Estimating the Linear Regression Equation in Microsoft Excel
Linear regression models can be estimated in Excel through two different ways. Both 
methods build on the least squares concept and are illustrated on the data set of average 
daily temperatures and ice cream sales shown in Figure 3.3.
The first and simplest way to estimate the regression model (3.3) is to simply add a 
trendline to the scatter plot of temperature and ice cream sales. This method only works 
when there is only one predictor variable, which is the case with the ice cream sales data 
set. The predictor variable for this data set is Temperature so the objective of running 
a regression on this data set is to determine if the expected daily temperature for some 
future day will help you better predict what the total sales of ice cream will be that day. 
To use the trendline method, you first need to plot a scatterplot of the predictor and 
response variable together, as shown in Figure 3.3. After creating the plot, move the 
mouse cursor over the datapoints in the graph and right click. From the menu that pops 
up, choose trendline. A box similar to the one in Figure 3.4 should now appear. Click 
the circle next to Linear and the two boxes at the bottom: Display Equation on chart and 
Display R-squared value on chart.
ˆ ˆ
ˆ
ˆ
ˆ ˆ

---

## Page 63

52  Promotion Forecasting
Figure 3.3 Daily Sales of Ice Cream and Daily Average Temperatures.
Figure 3.4 Trendline Option in Excel.

---

## Page 64

Promotion Forecasting  53
After clicking the close button, a straight line, regression equation and R-squared value 
should appear on the chart as in Figure 3.5. In this example, the intercept for the regres-
sion line is β0 = –253.5 and the coefficient for the predictor variable (temperature) is 
β1 = 6.0728. The temperature coefficient can be interpreted to imply that each degree 
warmer in the average temperature results in an additional 6.0728 units of ice cream 
sales. The R 2 value of 0.94 indicates that 94% of the variability in the response vari-
able (sales) is explained by the predictor variable (temperature). R-squared values range 
between zero and one, with values closer to one representing better fits. An R-squared 
value of zero indicates that there is no correlation between the predictor and response 
variables. In this case, you are as well off using the average value of the response variable 
to predict future observations as you are from using a regression model with an R
2 = 0.
Now suppose that you need to order supplies for your ice cream shop and tomorrow’s 
forecast is for an average temperature of 90 degrees. Using the regression equation for 
ice cream sales, you can estimate that the number of ice cream sales corresponding to the 
average temperature of 90 degrees is 
y = 6.0728*90 – 253.5 = 293.052≈293.
Thus, you should order enough supplies for an expected demand of 293 (in Chapter 4, 
we describe why you may want to order a little more or less than this amount). Before 
presenting the second estimation method, we first discuss a few ways a regression-based 
forecast should not be used.
Common Mistakes When Using Regression Models to Forecast
There are several common mistakes that are used when regression models are used for 
forecasting. The first common mistake is to not factor in the inaccuracy of the estimates 
for the predictor variables. Note that the ice cream sales regression equation is only use-
ful as long as you have access to a reasonably accurate weather forecast. If you need an 
estimate for demand for a particular day that is two months from today, for example, 
350
300
250
150
60 70
E(Sales) = −253.5 + 6.0728 · DAT
R2 = 0.94
80
Daily Average Temperature (F)
Ice Cream Sales (units)
90 100
200
Figure 3.5 Ice Cream Sales with Trendline.

---

## Page 65

54  Promotion Forecasting
you will probably be better off using one of the time series models discussed in the last 
chapter. This is because weather forecasts typically do not provide any better forecasts 
than the historical average monthly temperature for dates further out in the future than 
around eight days.
A second common mistake is to use the regression equation to make forecasts outside 
of the range for the predictor variables that the regression equation was estimated on. 
We demonstrate this point using an extreme example. Suppose that the location for 
your ice cream store is predicted to have an unusually cold day tomorrow, with an aver-
age temperature of 0 degrees. Plugging the value of 0 degrees into the regression model 
results in a prediction of –253.5 sales of ice cream tomorrow. Clearly, this prediction is 
not accurate as you cannot sell a negative number of bowls of ice cream. Thus, great care 
must be taken when a regression based forecast is used on values of the predictor vari-
ables outside of the range used to estimate the model (63–100 degrees in our example).
Estimation Using the Regression Feature in Excel
The second method for estimating a regression equation in Excel takes a few more steps 
than the trendline approach but it provides additional information and can be used 
when there are more than one predictor variables. We will demonstrate it on the same 
ice cream sales data set that we used to demonstrate the trendline method. To use the 
second method, first insure that the Data Analysis add-in has been installed in your ver-
sion of Excel. If it is, then you should see a Data Analysis option on the Data ribbon (in 
Excel 2010). After clicking on the Data Analysis button, a pop-up menu such as the one 
in Figure 3.6 should appear. Click on the Regression option on this menu.
After clicking the regression option, a pop-up box such as the one shown in Figure 3.7 
will appear. Enter the cells with the response variable in the first field and the cells with 
the predictor variables in the second field. The cell values shown in Figure 3.7 correspond 
to the cells on the sheet shown in Figure 3.3. In this example, we included the headings 
in the cell references so we checked the Labels box on the left-hand side. Keep the rest of 
settings at their default values and click the OK button at the top right corner.
The first thing to notice from the regression results in Figure 3.8 is that the R square 
value and the estimated regression coefficients are the same values estimated using the 
Figure 3.6 Data Analysis Menu.

---

## Page 66

Promotion Forecasting  55
trendline. Thus, the forecasting equation and interpretation is the same as discussed 
previously. Using the regression function in Excel provides a lot of additional informa-
tion over the trendline approach however. For example, the Significance F value in the 
ANOVA table provides the probability that you are gaining additional predictive power 
using the regression line versus just using the mean of the response variable (4.59 × 10
–13 
in our example). It is typical to only accept regression models where this value is less than 
0.05, that is, significant at the 95% level. You also get information about the significance 
of the predictor variables. To see if a predictor variable is significant, look at the P-value 
in the lower table. The P-value for the temperature variable is 4.59 × 10
–13 which is also 
well below the 0.05 cut off for a 95% significance level. While the significance of the 
overall regression and of the predictor variable are the same when there is only a single 
predictor variable, this will typically not be true after introducing more than one predic-
tor variable.
Linear Regression and the Maximum Likelihood Estimation Technique
An alternative approach to estimating the linear regression models (3.1)–(3.3) through 
the method of least squares requires finding the parameters 
β0, β1and σ 2 such that the 
likelihood of the observed data is maximized. The estimation method for doing so is 
referred to as the maximum likelihood estimation technique which, similar to the least 
squares method, builds on the standard assumption that the error terms 
εt are uncor-
related random variables with zero mean and variance σ 2. The maximum likelihood 
technique, however, imposes an additional assumption that requires the functional form 
of the distribution of the error term 
εt be known. The most common assumption is that 
the error terms εt are normally distributed, which in effect means that εt are independ-
ent normal random variables with zero mean and variance σ 2 (i.e., εt are independent 
Figure 3.7 Regression Pop-up Box.

---

## Page 67

56  Promotion Forecasting
N (0, σ 2)). The assumption on the form of the distribution of εt necessarily requires 
that the dependent variable observations in the linear regression model (3.3), for exam-
ple Salest, are also independent normal random variables with means E[Salest] = β0 + 
β1 · DATt and variance σ 2. 
Before we discuss the intricacies of the estimation of the linear regression model (3.3) 
through maximum likelihood, let’s build some intuition for how the technique is to be 
operationalized. Consider, for example, that the daily ice cream sales for three consecu-
tive days amount to 230, 250 and 270 units, respectively. In the absence of any other 
information, we could assume that these sales values are random realizations from a nor-
mal random variable with a mean 
µ and variance σ 2 and we wish to find out those values 
for µ and σ 2 that best represent the observed data best. In slightly more formal terms, we 
want to compute µ and σ 2 such that the likelihood of the observed data is maximized. 
For illustration purposes only, we plot our sales data together with the probability den-
sity functions of some candidate normal distributions in Figure 3.9. As it becomes appar-
ent from this figure, a normal distribution with a mean of 175 and a variance of 30
2 does 
not describe the observed sales data well since all three observations show in the right tail 
of the distribution. In practical terms, having the observed data so far to the right of the 
assumed mean of 175 units (i.e., 1.8, 2.5 and 3.2 standard deviations, respectively) means 
that it is quite unlikely for the observed sales data to have been drawn at random from a 
normal random variable N(175, 30
2). While it is quite easy to rule out N(175, 302) as an 
unfit distribution, things get more difficult as we evaluate the relative performance of the 
other two normal distributions, which differ only in regard to their assumed variances 
(i.e., 
σ 2 = 302 vs. σ 2 = 152). Since eyeballing cannot really help us here, we make use of 
Figure 3.8 Output of the Linear Regression on the Ice Cream Sales.

---

## Page 68

Promotion Forecasting  57
the densities (i.e., the heights) of the probability density functions computed at the levels 
of the observed data to characterize how well the assumed normal distributions describe 
the data. For any given normal distribution N(µ, σ 2), we multiply the densities that cor-
respond to all observed sales data points to obtain the data likelihood function, a unique 
descriptor of how well 
µ and σ 2 characterize the observed sales data. Of all competing 
(µ, σ 2) pairs, we choose as our preferred estimate the pair that maximizes the likelihood 
function. For our three data point example, we show the density values in Figure 3.9 
and the corresponding data likelihoods in Table 3.1. We compute the densities using the 
generic form of the probability distribution function of a normal random variable N (µ, 
σ 2) given by:
fx x,, e x pμσ
σπ
μ
σ
2
2
2
1
2
1
2() =
⋅⋅
⋅− ⋅ −()⎡
⎣
⎢
⎢
⎤
⎦
⎥
⎥
.
For the observed sales value of 230, for example, the densities evaluate to:
f 230 175 30 1
30 2
1
2
230 175
30
2
2
2,, e x p() =
⋅⋅
⋅− ⋅ −()⎡
⎣
⎢
⎢
⎤
⎦
⎥
⎥
=
π
2.477044E-03,
f 230 240 30 1
30 2
1
2
230 240
30
2
2
2,, e x p() =
⋅⋅
⋅− ⋅ −()⎡
⎣
⎢
⎢
⎤
⎦
⎥
⎥π
= =
() =
⋅⋅
⋅− ⋅ −()
1.25794E-02, and,
f 230 240 15 1
15 2
1
2
230 2402,, e x p
π
2 2
215
⎡
⎣
⎢
⎢
⎤
⎦
⎥
⎥
= 2.12965E-02.
Using a similar approach to compute the densities for all other observed sales values (i.e., 
250 and 270), we can conclude that of the three normal distributions considered, the 
one that describes the observed data best is N(240, 15
2). For this normal distribution, the 
data likelihood function amounts to 1.63248E-06 (see Table 3.1).
100
0.000
0.010
0.020
150 200
Sales
Probability Density Function ƒ(x)
250 300
Observed Sales ValuesN (175,302) N (240,302) N (240,152)
Figure 3.9 Illustration of the Maximum Likelihood Estimation Mechanism.

---

## Page 69

58  Promotion Forecasting
Building on this admittedly simple example, we return now to the linear regression 
model (3.3) and discuss how the parameters β0, β1 and σ 2 should be computed so as to 
maximize the likelihood of the observed data. To facilitate the discussion, we use the 
data provided in Figure 3.3 and show in Figure 3.10 the scatterplot that characterizes the 
relationship between the ice cream sales and the daily average temperature. We formal-
ize this relationship by fitting a regression line through the points of the scatterplot. We 
leave the regression line specified generically as E[Sales] = β0 + β1 · DAT and acknowledge 
again that the sales to be experienced at any daily average temperature DATt are all ran-
dom normal variables with means E[Salest] and variance σ 2. The last of these points is a 
direct result of the assumption that the error terms εt are independent normal random 
variables with zero mean and variance σ 2. With this in place, we can proceed to the next 
task of computing the data likelihood function. Since the observed sales values Salest are 
realizations from the underlying normal distributions N(E[Salest],σ 2) = N(β0 + β1 · DATt, 
σ 2), we can compute the densities that correspond to these observed data values as:
f Sales E Sales
Sales E Sales
tt
tt,, e x p[]() =
⋅⋅
⋅− ⋅
− []()σ
σπ σ
2
2
2
1
2
1
2
⎡ ⎡
⎣
⎢
⎢
⎤
⎦
⎥
⎥
=
⋅⋅
⋅− ⋅
−+ ⋅()()⎡
⎣
⎢
⎢
⎤
⎦
⎥
⎥
1
2
1
2
01
2
2σπ
ββ
σ
exp .
Sales DATtt
 
(3.7)
To help visualize how these densities are evaluated, we illustrate this task graphically in 
Figure 3.10 where, for a few pairs (DATt, Salest), we show the probability density func-
tions of the underlying normal distributions N(E[Salest], σ 2) as well as the densities  
f(Salest, E[Salest], σ 2) that correspond to the observed sales values Salest.
Next, we construct the data likelihood function as before by multiplying the densi-
ties computed using equation (3.7) for all observed sales values Salest. For the Rita’s Ice 
Cream data set, which consists of N = 21 observations, the likelihood function is:
L
Sales DATttββ σ
σπ
ββ
σ
01
2 01
2
2
1
2
1
2,, e x p() =
⋅⋅
⋅− ⋅
−+ ⋅()()⎡
⎣
⎢
⎢
⎤
⎦
⎥
⎥
⎧ ⎧
⎨⎪
⎩⎪
⎫
⎬⎪
⎭⎪
=
⋅⋅
⎛
⎝⎜
⎞
⎠⎟ ⋅−
⋅
⋅− + ⋅
=
∏
t
N
N
ttSales DAT
1
2 01
1
2
1
2σπ σ
ββexp (()()
⎡
⎣
⎢
⎢
⎤
⎦
⎥
⎥=
∑
2
1t
N
Table 3.1 Illustration of the Maximum Likelihood Estimation Mechanism
Normal Distribution Densities at the Observed Sales Values of
Data Likelihood 
(D1) x (D2) x (D3)/H9262/H9268 /H92682 230 250 270
(D1) (D2) (D3)
175 30 30 2 2.47704E-03 5.84277E-04 8.83659E-05 1.27890E-10
240 30 30 2 1.25794E-02 1.25794E-02 8.06569E-03 1.27633E-06
240 15 15 2 2.12965E-02 2.12965E-02 3.59940E-03 1.63248E-06

---

## Page 70

Promotion Forecasting  59
and is maximized at
β
β
1
1
2
1
0
6 0728=
−() ⋅−()
−()
==
=
∑
∑
DAT DAT Sales Sales
DAT DAT
t
t
N
t
t
t
N .
==− ⋅= −
=
−+ ⋅()()
==
∑
Sales DAT
Sales DAT
N
tt
t
N
β
σ
ββ
1
2
01
2
1 19
253.4986
331 4.,
                                              where DAT = 83.38 (F) and Sales = 252.86 (units) are the means of DATt and Salest, 
respectively. Comparing the parameter estimates shown in equation (3.8) with those 
provided in the related equations (3.4) and (3.6), we note that the least squares and the 
maximum likelihood estimation techniques suggest identical estimates for the regres-
sion coefficients β. In terms of the estimates for the variance σ 2, which obviously differ 
across methods, the one recommended by the least squares estimation technique is typi-
cally preferred (see equation(3.6)) as the maximum likelihood estimate is biased (i.e., 
E[
σˆ2] ≠ σ 2. For some more advanced demand models (some of which are given in Table 
3.3) however, the maximum likelihood estimation technique is preferred. 
Figure 3.10 Estimation of the Linear Regression Model via Maximum Likelihood.
0.08
0.06
60 70 80
Daily Average Temperature (F)
ƒ(Sales, E[Sales], σ2)
Ice Cream Sales (units)
ƒ(Salest , E[Salest ], σ2)
E[Salest ]
90 100
100
150
200
250
300
350
400
0.04
0.02
0.00
E[Sales] = β0 + β1 . DAT
Salest
ˆ
ˆ
ˆ

---

## Page 71

60  Promotion Forecasting
Multiple Linear Regression
Multiple linear regression is used to estimate the relationship between more than one 
predictor variables and a single response variable. Suppose that you want to include the 
effect of a certain promotion in estimating ice cream sales. During the time period that 
the ice cream sales data was collected, the store manager would sometimes include a flyer 
in the daily paper promoting the store. The manager feels that demand is higher on days 
that she uses the flyer promotion but is not sure how much additional demand is driven 
by this promotion. The relation between sales and the now two explanatory variables can 
be formalized as:
Sales
t = β0 + β1 · DATt + β2 · FLYt + εt
where DATt continues to represent the daily average temperature and the new variable, 
FLYt, indicates if a flyer was included in the paper that day. The FLY variable is an indica-
tor variable, meaning that it only takes a one or zero value. If a flyer promotion was used 
on a particular day, then FLY = 1, if not then FLY = 0. The data used for this regression is 
shown in Figure 3.11 and the regression results are shown in Figure 3.12.
Observing the new regression results, notice that the R-squared value increased 
slightly compared to the single variable regression results in Figure 3.8. This will always 
be the case as you add more predictor variables, the R-square value will only go up. The 
Adjusted R-square value, however, is smaller than the original regression (.9338 versus 
.9368) because it includes a penalty for adding additional predictor variables. When a 
new variable is added and this value goes down, it is an indication that the new variable is 
not adding any additional predictive power to the model. This is confirmed by looking at 
the P-value of the Flyer variable (.715188), which is much larger than the 0.05 threshold 
required for significance at the 95% level. Thus, it does not appear from these results that 
the flyer promotion provides any additional sales lift, at least on the day that it appears 
in the daily paper. Care must be taken, however, in making broader interpretations of 
regression results. For example, you could conclude from the lack of significance in the 
regression model that the flyer promotion does not add any value. This conclusion may 
be incorrect, however, because the regression equation only measures the sales lift of 
the promotion on the day that the flyer appears. Thus, it could be the case that the flyer 
does increase the overall brand awareness of the store and, in its absence; the overall sales 
could be lower over an extended period of time.
ESTIMATING PROMOTION EFFECTS
In this section, we build on the example that targeted the effectiveness of the newspaper 
flyer on generating incremental demand and provide a deeper understanding of what 
estimating the promotion effects typically entails. In our exposition, we acknowledge that 
many organizations rely on promotion activities to spur the demand for the products they 
sell. Retailers, for example, offer their clients a multitude of in-store promotions in an 
attempt to convert the incoming traffic into sales and build store and brand loyalty. “Buy 
one, get one free,” “Now for a limited time only, 25% off,” and “Buy one, get the second 
for 50% off” are just some of the special displays and promo signs intended to capture the 
interest of passing customers and increase their purchasing likelihood. Similarly, in the 
hospitality industry, hotel chains attempt to boost sales, improve hotel occupancies and

---

## Page 72

Promotion Forecasting  61
Figure 3.12 Regression Output with Promotional Flyer Variable Included.
Figure 3.11 Ice Cream Sales with Promotional Flyer Variable Included.

---

## Page 73

62  Promotion Forecasting
increase the discretionary spending on hotel-related activities by promising more for less. 
Wyndham Hotels and Resorts, for example, promotes specific US and international travel 
destinations by offering the night following a three consecutive night stay free of charge. 
Along the same lines, Hotels.com, an affiliate of Expedia Inc., rewards its loyal customers 
with a complimentary one-night stay at any of the hotels it sells once customers collect ten 
nights booked through the Hotels.com’s websites or call centers. Whether communicated 
to customers as simple temporary price discounts or through a more complex advertising 
mechanism (e.g., display and feature advertising), these promotions are intended to make 
up for the reduction in unit margins through an increase in sales volumes. The timing and 
promotion attributes are usually suggested based on the organization’s understanding of 
its business specificities. At times, however, the complexity of this task overwhelms those 
in charge with the promotion planning duties and results in unexpected revenue and/or 
profit losses. For example, it is not unusual for an otherwise carefully designed promotion 
to lead to out-of-stock (OOS) events in cases where the promotion effects are underesti-
mated. Similarly, promotions that hurt the bottom line may occur when their effectiveness 
is overestimated and the organization is left with high excess inventory. Since success in 
this case means to be right on target when estimating the promotion effects, in what fol-
lows, we refer to several instances that may impede us from doing so.
For maximum product exposure, retailers oftentimes plan their promotions such that 
they overlap with periods known for high incoming store traffic. It is not uncommon 
to walk into Macy’s jewelry department days before Mother’s Day and notice a sale on 
all women’s jewelry. It is also not uncommon to see this pattern repeat during similar 
high-traffic-generating events, including Christmas, Easter, and Valentine’s Day. In the 
absence of other intelligence, this situation may impede retailers from differentiating 
(or, separating) the effects of the price promotions from those that naturally arise as a 
result of elevated in-store traffic. In this case, whichever effects retailers decide to com-
pute reflect the intrinsic presence of the other ones. Hence, the promotion effects are 
either underestimated or overestimated.
In addition to a possible confounding problem, organizations need to cope with their 
inability to correctly estimate the true demand for a product or service. To our knowl-
edge, the retail industry faces one of the toughest challenges in this area. As opposed to 
other industries such as airlines and hospitality, where mechanisms are in place to cap-
ture the demand lost due to the product being unavailable (e.g., the central reservation 
systems developed by such software vendors as Sabre Hospitality Solutions or Amadeus 
provide hotels with detailed intelligence on lost business), in retail such attempts have 
proven to be difficult. Typically, the existence of OOS events is not documented and/or 
the purchasing intentions of customers facing OOS events are largely unknown. Thus 
retailers often rely solely on the sales history to infer the product future performance, 
even though the history may be biased upward or downward by the presence of the same 
product or other substitutable products’ OOS events. In the short term, the downward 
bias caused by the product stock-outs leads to the retailer underestimating the full poten-
tial of promoting an item. In the long term, unless it discovers and adjusts its sales figures 
to account for this bias (see, e.g., the techniques discussed in Chapter 5), the retailer may 
experience a dangerous spiral-down phenomenon that could ultimately lead to it being 
artificially reluctant to promote or assort an item anymore.
Another important factor that impacts the success of a promotion is its timing. For 
example, organizations that historically promote their fashion-like products close to the

---

## Page 74

Promotion Forecasting  63
end of the season may discover that the same price discounts employed while still in the 
season may result in significantly higher sales uplifts. This seems intuitive as customers 
tend to value similar discounts more when the product they purchase is still in fashion. 
Yet, unless organizations experiment to understand and plan the timing of their pro-
motions accordingly, they will continue to experience recurrent stock-outs or excess 
inventory.
All else equal, the promotion timing is not the only factor that may lead to undesired 
results. Quite often, the expectations associated with certain promotions turn out to be 
unrealistic because no clear differentiation between what contributes to the expected 
sales uplift exists. For example, the effectiveness of a 25% off promotional offer should 
be judged on several factors, including the promotional vehicles used to execute it. Yet 
oftentimes, retailers do not or cannot differentiate between promotional vehicles such as 
“Now 25% off “ or “Buy three, get the fourth free” and plan their promotions unsatisfac-
torily. In these cases, the retailers’ promotion stock levels are frequently amiss.
The digression above shows that estimating the promotion effects is not a simple task. 
To put some structure around it, we present it in the context of the overarching theme of 
promotion planning and optimization (PPO). Table 3.2 provides a simplified overview 
of what PPO typically entails. We include the estimation of promotion effects in the 
Analytical Modeling step and preface an in-depth discussion of what this step requires 
with a few remarks about its role within the overall PPO framework.
The goal of both the Analytical Modeling and the Validation and Refinement steps is 
to forecast the likely outcomes of a planned promotion usually at the intersection of three 
dimensions: product (e.g., blue Hugo Boss stretch jeans), location (e.g., Macy’s Herald 
Square store), and time (e.g., promotion planned for the coming Easter week). To ful-
fill this goal, insights acquired over time along these dimensions as well as the planned 
promotion type itself are used. Typically, the promotion histories along the product and 
location dimensions are first revisited. This effort leads to the estimation of the base-
line sales and all other promotion and time-related special event effects. The promotion 
effects as computed at this stage constitute the basis for the forecast of the results of the 
planned promotion. They are, however, validated against the historical performance of 
the planned promotion type across all three dimensions and possibly refined further to 
account for factors as diverse as their statistical significance, the presence of the planned 
promotion mix among the historical promotion events, the geographic or time locali-
zation of the planned promotion, and so on. In Table 3.2, all data steps that precede 
Analytical Modeling aim to ensure the accuracy and consistency of aggregate promotion 
histories at the required product, location, and time dimensions. Similarly, the steps that 
follow Validation and Refinement are critical as well, as they ultimately supply and grow 
the historical collection of promotion effects used in benchmarking and refinement.
Returning to the Analytical Modeling step, the literature on promotion planning and 
optimization approaches the estimation of promotion effects in two distinct ways. The 
first way uses data on the promotion histories along the product and location dimen-
sions and attempts to explain individual sales, exposed or not to promotions, via the use 
of some explanatory variables. Typical explanatory variables are the own and substituta-
ble products’ selling prices or its many variants, including percent discount or percent of 
regular price, the own and substitutable products’ promotion types (e.g., feature adver-
tising and/or display), the promotion frequency, the inventory availability (extremely 
relevant for apparel), the presence of special events such as Christmas and Easter,

---

## Page 75

Table 3.2 Promotion Planning and Optimization
1. Data Collection 2. Data Cleansing and Storage 3. Data Imputation and Aggregation 4. Analytical Modeling a)
a. Point of Sales/scanner 
data enriched with promo 
information (e.g., display 
or feature conditions, 
advertisement types, etc.) 
and (shelf) out-of-stock 
intelligence.
a. Cleanse and permanently 
store the raw data in the 
Enterprise Data Warehouse 
(EDW).
b. Typically executed in real 
time or as a batch process 
every night.
a. Impute sales data to reflect own and 
substitutable products’ out-of-stock 
conditions.
b. (Optional) Aggregate data to reflect the 
needs of downstream processes (e.g., 
daily data to weekly data).
c. Typically executed as a weekly or 
nightly batch process.
d. (Optional) Employ ETL processes to 
Extract, Transform and Load data into 
external partners’ databases.
a. Employ mathematical models to compute 
baseline forecasts and promotion and other 
effects (e.g., discount, special events and 
seasonality effects).
b. (Optional) Compute price elasticity of demand.
c. Store results in the Enterprise Data Warehouse.
d. Typically executed as a weekly batch process 
over the most recent relevant promotion 
histories.
e. Some companies outsource this task (see the last 
entry at Step 3).
5. Validation and 
Refinement
b)
6. Promotion Planning 7. Promotion Execution 8. Promotion Evaluation
a. Adjust the forecasts and 
promotion effects based 
on intimate market 
knowledge (i.e., query 
the Promotion Database 
in the EDW) or through 
additional data mining.
b. Typically executed 
together with Step 4.
a. Order product as per the 
recommendations of Task 5.
b. Order promotion and other 
support material.
c. Communicate to field 
personnel all required promo 
details.
a. Execute the promotion. a. Analytically evaluate the success of the 
promotion.
b. Store results in the Promotion Database in the 
EDW.
Note: a) For details, see Achabal, McIntyre, & Smith (1990), Cooper, Baron, Levy, Swisher, & Gogos (1999), Foekens, Leeflang, & Wittink (1994, 1998), Narasimhan (1984), Smith & 
Achabal (1998), and Van Heerde, Leeflang, & Wittink (2000, 2004). b) For details, see Cooper et al.(1999) and Trusov, Bodapati, & Cooper (2006).

---

## Page 76

Promotion Forecasting  65
seasonal variation, and the competitors’ response. The assumed relationships between 
sales and the explanatory variables are either additive or multiplicative. Additive rela-
tionships operationalized as linear regression models are typically employed when pro-
motion effects are thought to be insensitive to the overall level of the baseline sales. This 
implies, for example, that under similar promotion conditions, Macy’s would expect to 
sell 20 more pairs of blue Hugo Boss stretch jeans when this item’s baseline sales were 
either 10 or 100 units. Conversely, the multiplicative relationships, log transformed to 
be operationalized as linear regression models (see Table 3.3), are usually preferred when 
the promotion effects are considered to be proportional to the absolute values of the 
baseline sales. Effectively, this means that a similar promotion effect multiplier of 3.0 
applied to Macy’s baseline sales of 10 and 100 units would lead to incremental sales of 
20 and 200 units, respectively. As we acknowledge that the operationalization of these 
models is quite subtle, we illustrate them in Table 3.3. In all cases, the estimation of the 
model parameter estimates can be done by minimizing the sum of squared errors (or, 
deviations) using the ordinary least squares method.
The second approach to estimating and subsequently forecasting the promotion 
effects focuses on promotion events only as the natural promotion planning unit as the 
promotion event (Cooper, Baron, Levy, Swisher, & Gogos, 1999; Trusov, Bodapati, & 
Cooper, 2006). Its intent is to build accurate predictive regression models by combin-
ing all historical promotion events across the product, location, and time dimensions 
while controlling for factors as diverse as the various variants of the long-term average 
of the baseline sales, the promotion attributes, the promotion frequency, the presence 
of special events, and so on. As these models can be calibrated on any promotion data 
partitions including those temporally driven, this approach seems to be better suited to 
accommodate the planning of promotions of various durations (e.g., one week vs. two 
weeks vs. three+ weeks).
To see how the promotion effects are estimated in practice, we discuss the example of 
a staple fashion item (e.g., basic denim products such as blue jeans and hosiery) sold by 
a major retailer throughout the United States. Due to space constraints, we restrict our 
analysis to 26 weeks of sales as experienced by one of the retailer’s stores in the southeast 
region. Since the promotion events in this sample do not support a thorough discussion 
of the second approach to estimating the promotion effects, we focus instead on discov-
ering a reasonable relationship between the weekly sales and the available explanatory 
variables. For simplicity (and, partly, due to data unavailability), we do not consider in 
our work any temporal effects (e.g., cross-period promotion effects due to demand being 
shifted backward or forward or seasonality effects) or secondary effects (e.g., cross-prod-
uct promotion effects that reflect in the sales of nonpromoted sister products). For the 
former of these topics, we refer the interested reader to Van Heerde, Leeflang, & Wittink 
(2000) and the references therein; for the latter, relevant insights can be found in Van 
Heerde, Leeflang, & Wittink (2004).
The sample spans about six months of history (i.e., 26 consecutive weeks) and covers 
the period from February to August. In total, four major holidays, including Easter and 
the Fourth of July, are represented in the data and counted as special events. The item 
of interest is typically sold at $135.00. At times, to increase store traffic and incentivize 
customers to purchase, the retailer runs a simple price discount promotion on this item. 
When offered, the promotion lasts a week at the most. In our sample, there are six price 
discount instances: three relate to a 15% discount and are offered in the spring, while the

---

## Page 77

Table 3.3 Additive and Multiplicative Promotion Models
(A) Additive Model (Transformation Required: None) (Narasimhan, 1984)
General form (linear regression model): Example:
YXtk t k
k
K
t=+ ⋅ +
=
∑
ββ ε0
1
, Sales P SEtk t k
k
K
tt=+ ⋅ + ⋅ +
=
∑
ββ γ ε0
1
,
where Y is the response variable; Xk, 1 ≤ k ≤ K, are the explanatory 
variables; t is a general index such as time; 
εt is a zero mean and 
constant variance random normal error term; 
β0 and 
βk, are the 
parameter estimates (or, regression coefficients) that have to be 
computed from the data.
where Salest are the sales during time period t (e.g., week t); 
β0 is the average sales at the full 
price P0 (or, the baseline sales); Pt,k, k ≤ 1 ≤ K, are indicator variables (or, dummy variables) 
equal to 1 if at time t the price point Pk is offered, 0 otherwise; SEt is an indicator variable 
equal to 1 if special events are associated with time t, 0 otherwise; 
εt is a zero mean and 
constant variance random normal error term; and, 
β0, βk and γ are the parameter estimates.
(B-1) Multiplicative Model (Transformation Required: Natural Log) 
(Achabal et al., 1990; Foekens et al., 1994, 1998; Narasimhan, 1984; 
Wittink, Addona, Hawkes, & Porter, 1988)
General form: Example
YX ett k k
k
K
l
Xtl
l
L
t=⋅ ⋅ ⋅
==
∏∏
βγ
βε
0
11
,
, Sales P
P et
t SEtt=⋅ ⎛
⎝
⎜
⎞
⎠
⎟ ⋅⋅
βγ
β
ε
0
0
1
Transformed form (variant of a Power model): Transformed form: 
log log log log,,YX Xtk t k
k
K
lt l
l
L
t() = () +⋅ () + () ⋅+
=+
==
∑∑
ββ
γ ε0
11
0Β
ββεkt k
k
K
lt l
l
L
tXX⋅ () +⋅ +
==
∑∑ log ,,
11
Γ
log log log log
l
Sales P
P SEt
t
tt() = () +⋅ ⎛
⎝
⎜
⎞
⎠
⎟+ () ⋅+
=+ ⋅
ββ
γ ε
β
01
0
01Β oog P
P SEt
tt
0
⎛
⎝
⎜
⎞
⎠
⎟+⋅ +Γ
ε
where Y is the response variable; Xk, 1 ≤ k ≤ K, and Xl, 1 ≤ l ≤ L, are the 
explanatory variables (Xl are typically indicator variables); t is a general 
index such as time; 
β0 = antilog (B0); γl = antilog (Γl); εt is a zero mean 
and constant variance random normal error term; and, B0, βk and Γl 
are the parameter estimates that have to be computed from the data.
where Salest are the sales during time period t (e.g., week t); 
β0 is the average sales at the 
full price P0 (or, the baseline sales); Pt refers to the selling price at time t; SEt is an indicator 
variable equal to 1 if special events are associated with time t, 0 otherwise; β0 = antilog (B0); 
γ = antilog (Γ) εt is a zero mean and constant variance random normal error term; and, B0, 
β1 and Γ are the parameter estimates.

---

## Page 78

(B-2) Multiplicative Model (Transformation Required: Natural Log) (Narasimhan, 1984; Smith & Achabal, 1998)
General form: Example:
Ye et k Xt k
k
K
t=⋅ ⋅ ⋅
=
∏
β
βε
0
1
, Sales e e et
Pt PS E tt=⋅ ⋅ ⋅ ⋅− ⋅
β
βγ ε
0 1 1 0(/ )
Transformed form (Exponential model): Transformed form:
log log ,
,
YX k
Xk
tk t
k
K
t
kt
k
() = () +⋅ +
=+ ⋅ +
=
=
∑
ββ ε
β
0
1
0
1
            B
K K
t∑
ε
log( ) log ( ) ( )Sales P
P SEt
t
tt=+ ⋅ − ⎛
⎝
⎜
⎞
⎠
⎟+⋅ + 
           
ββ γ ε01
0
1
        = + ⋅ − ⎛
⎝
⎜
⎞
⎠
⎟+⋅ +B01
0
1
βγ ε P
P SEt
tt
where Y is the response variable; Xk, 1 ≤ k ≤ K are the explanatory 
variables; t is a general index such as time; 
β0 = antilog (B0); 
εt is a 
zero mean and constant variance random normal error term; and, β0 and 
β? are the parameter estimates that have to be computed from 
the data.
where Salest are the sales during time period t (e.g., week t); 
β0 is the average sales at the 
full price P0 (or, the baseline sales); Pt refers to the selling price at time t; SEt is an indicator 
variable equal to 1 if special events are associated with time t, 0 otherwise; β0 = antilog (B0); 
εt is a zero mean and constant variance random normal error term; and, B0, β1 and 
γ are the 
parameter estimates.

---

## Page 79

68  Promotion Forecasting
other three are associated with a 25% discount and are featured in the summer. In four 
of these cases, the price discounts and the special events overlap. The sales in the nonpro-
moted weeks are quite stable and average about 59 units per week. The price promotions 
coupled with the high-traffic special events seem to have a significant impact on sales. 
Across both of these events, the average weekly sales are 203 units. During the period 
of study, no formal OOS events have been reported for this item, so we could assume 
that the data reflects the true demand. The start of the week inventory is unknown, but 
we assume further that there was enough stock available in terms of sizes for a proper 
product display. This assumption essentially implies that the sales values are not con-
strained by the appropriate size-level merchandise not being available (i.e., apparel and 
seasonal goods retailers may essentially experience OOS events if all they are left with is 
the unpopular sizes that no one wants to purchase). The underlying data are provided in 
Table 3.4 and graphically depicted in panel A of Figure 3.13.
To estimate the promotion effects, we choose to link the observed weekly sales to the 
explanatory variables using an additive relationship (see model type A in Table 3.3). Our 
choice is motivated primarily by the regular patterns noticed in sales and the amount of 
data available. We model the price discount effects through the use of two dummy vari-
ables corresponding to the discounted price points of $114.75 and $101.25, respectively. 
We incorporate the special events effects by using another dummy variable that appro-
priately identifies the presence of these events. We use the ordinary least squares method 
for fitting linear models, as implemented in R, to compute all parameter estimates. The 
estimation results are provided in Table 3.5.
The price promotion estimates in Table 3.5 suggest that the price discounts do have 
a significant and differential effect on sales. To this end, a price discount of 15% is esti-
mated to result in incremental sales of 85.6 units. Similarly, a price discount of 25% is 
estimated to result in incremental sales of 110.6 units. This differential response to the 
levels of discount offered implies that customers’ willingness to pay is unevenly distrib-
uted across price ranges ($114.75, $135.00) and ($101.25, $114.75), respectively, which 
would be a valuable insight if the optimization of the product price were attempted. 
Table 3.4 Promotion History for a Staple Fashion Item
Week Sales Price 
[$]
Special Events 
(SE)
SE 
Indicator
Week Sales Price 
[$]
Special Events 
(SE)
SE 
Indicator
1 230 114.75 Presidents Day 1 14 50 135.00 0
2 71 135.00 0 15 225 101.25 Memorial Day 1
3 70 135.00 0 16 46 135.00 0
4 65 135.00 0 17 51 135.00 0
5 60 135.00 0 18 50 135.00 0
6 195 114.75 Easter 1 19 46 135.00 0
7 76 135.00 0 20 253 101.25 4th of July 1
8 51 135.00 0 21 47 135.00 0
9 79 135.00 0 22 59 135.00 0
10 146 114.75 0 23 55 135.00 0
11 69 135.00 0 24 168 101.25 0
12 52 135.00 0 25 48 135.00 0
13 60 135.00 0 26 73 135.00 0

---

## Page 80

Promotion Forecasting  69
In addition, whenever a special event similar to the ones in the sample takes place, the 
sales are expected to increase by 68.8 units. From a managerial perspective, this finding 
is also relevant as high levels of store traffic seem to significantly impact the product’s 
sales at no additional costs. Thus even if no actions are taken to sustainably increase the 
customer base, rethinking the store product placement may lead to immediate and/or 
similar incremental gains.
As we already hinted, a special word of caution seems appropriate regarding the differ-
ential response to the levels of discount shown in Table 3.5. The price discount effects we 
have explored so far are all estimated based on a limited promotion history of 26 weeks. 
Had we considered more of the product history in our exploration, it is quite likely that 
we would have obtained different results. In addition, our analysis is constrained by the 
usage of a single type of special events. In practice, however, given the richer information 
available to your disposal, you may want to differentiate between these events and treat 
some of them as independent special event instances. It is our expectation that had we 
done so our price discount effects would have changed as well.
(A) Sales, Price Promotions, and Special Events Information
Time
Sales
Price ($)
Mar
0
100
200
300
0
50
100
150
Discount and SE
Discount and SE
Discount and SE
Discount and SE
Discount
Discount
Apr May Jun Jul Aug
(B) Linear Price-Response Function
Price ($)
Sales
100
S = 516.49 − 3.35  p60
120
180
120 140
Figure 3.13 Promotion History for a Staple Fashion Item.
Table 3.5 Summary Statistics and Model Fit
Estimate Std. Errors t value p value
Baseline sales at $135.00 58.9 2.7 21.6 0.00
Discount Price $114.75 85.6 10.3 8.3 0.00
Discount Price $101.25 110.6 10.3 10.7 0.00
Special Events Indicator 68.8 10.5 6.5 0.00

---

## Page 81

70  Promotion Forecasting
While going through the material presented in this section, you may have wondered 
if there are other uses of the results provided in Table 3.5. In fact, there are as it is rare 
for a price/demand data set to not include some time periods when (price) promotional 
events occurred. Fortuitously, as long as price variation exists and customers are price 
responsive, we can usually separate the effect(s) of price on sales from those attributed to 
other sales contributors such as other promotion attributes, seasonality, special events, 
and so on. This separation allows for the easy computation of price-response functions 
appropriate for the dominant market conditions (e.g., no feature advertising or display 
and no special events). Based on how complex the expressions of these functions are, 
the price elasticity of demand is subsequently derived either analytically or numerically. 
Returning to the previous example, we can compute the point estimates of the sales 
expected to materialize at the three discount levels offered by using the information from 
Table 3.5. Through simple analytical manipulations, it is easy to show that the expected 
sales at $135.00 (0% off), $114.75 (15% off), and $101.25 (25% off) are 58.9, 144.5, and 
169.5 units, respectively. If a linear price-response function of the form depicted in equa-
tion (3.2) were considered appropriate for this application (which we already concluded 
is a questionable assumption), then the methodology described in the previous sections 
could be employed to yield the following relationship between sales and price S(p) = 
516.49 – 3.35 · p. Such a relationship would ultimately allow us to compute the unit-free 
elasticity measures needed in a price optimization application. For completeness, we 
illustrate graphically the sales-price scatterplot together with the linear price-response 
function in panel B of Figure 3.13 but defer the discussion on how to compute the cor-
responding elasticity curves to Chapter 6.
CASE STUDY: PROMO FORECASTING AT DOMINICK’S FINER FOODS
Promotions are intended to stimulate sales and capture market share, but with all the 
complexities involved in making promotional investments, there is a lot of space for 
making mistakes. To reduce the likelihood of these mistakes taking place or to limit 
their consequences, retailers need to quantify as precisely as possible the impact on sales 
of independent or complementary promotion activities. Ideally, a retailer would like to 
know ahead of time that if a given product gets discounted by 25% in the week of the 
Fourth of July, sales of the product should increase by five times the normal amount. As 
an increase of this size may warrant such an aggressive discount level, the retailer could 
use this information to place an order with the supplier for a quantity that would allow 
it to satisfy the anticipated levels of demand. The likelihood of it facing a stock-out and 
losing revenues and/or profits would therefore be appropriately mitigated. In what fol-
lows, we discuss how to sensibly accomplish such a task by looking into the operations of 
a retailer that competes in the grocery industry.
We explore a variant of the model proposed by Foekens, Leeflang, & Wittink (1994) 
(for a relevant overview, see model type B-1 in Table 3.3) using a subset of the data made 
publicly available by the James M. Kilts Center, University of Chicago Booth School of 
Business. The data includes weekly store-level transaction prices, quantities, percent-
age markups, and discount information for more than 100 grocery stores operated by 
Dominick’s Finer Foods, a subsidiary of Safeway Inc., in the Chicago, Illinois, area. Of 
the available products, we focus on the 18 ounce Quick Quaker Oats from the Oatmeal 
category, sold in the River Forest store during a period of almost six years (i.e., June 6,

---

## Page 82

Promotion Forecasting  71
1991–May 1, 1997). We have selected this product–store pair based on convenience; 
that is, we have looked specifically for products and stores with consistent sales across 
an extensive selling window of more than 300 weeks. As no information on the OOS 
events accompanies the data set, all weekly records with zero sales are considered stock-
out events. This assumption seems reasonable since the total number of zero sales weeks 
accounts for only 1.9% of the available data. Because the methodology we employ to 
quantify the promotion effects breaks down when zero sales or price points are present 
in the data, all such instances have been replaced by the corresponding averages. Other 
smoothing methods (e.g., median smoothing and moving average) or imputation tech-
niques (e.g., nearest neighbor hot-deck and random hot-deck) can be used to replace 
missing (or, incomplete information) data with imputed values that are more local in 
nature. While sales for the weeks with nonzero sales can also be impacted by OOS events, 
we assume that these sales values are not constrained by any product shortages due to 
either an inappropriate in-store product handling or an ineffective management of the 
extended supply chain. This last assumption, while convenient, seems to be at times a 
rather strong assumption as several promoted weeks show insignificant or reversed sales 
uplifts.
As per the Dominick’s Finer Foods’ store zoning of 1992, the River Forest store oper-
ated in a high-price tier competitive environment. Throughout the study period, Quick 
Quaker Oats’s regular unit price of $1.99 did not change significantly. The steepest 
price decrease (vs. price discount) of $0.20 reported for about eight consecutive months 
between 1992 and 1993 was followed a year later by a $0.10 price increase which lasted 
for about four months. Various promotion activities, of which some involved price dis-
counts, also altered the product’s regular price for limited-time periods. In total, pro-
motions for Quick Quaker Oats were run in 43 of the 309 possible weeks. On average, 
500
400
300
200
100
1992 1993 1994 1995
Time
Sales
Price ($)
1996 1997
0
2.0
1.5
1.0
0.5
0.0
Promoted WeeksPriceSales
Figure 3.14 Sales and Price Plots: Quick Quaker Oats at River Forest Store.

---

## Page 83

72  Promotion Forecasting
relative to the closest preceding nonpromoted regular price, the product was sold at 
a 14.9% discount during the promoted periods. The maximum discount was close to 
50% and was offered during Labor Day in 1994. Typically, promotions involved various 
forms of Bonus Buys such as “Buy one, get one free” (34/43) and, to a lesser extent, true 
Simple Price Reductions (9/43). The changes in regular and promotion prices together 
with promotion timing are depicted in Figure 3.14.
The broken lines shown in Figure 3.14 are illustrative of the relationship between the 
offered prices and sales. In general, promotions that involve price discounts result in 
higher than normal sales levels. In addition, higher discounts lead to higher volumes 
sold. Thus the sales–price association implied by the power model or its variants (see 
model type B-1 in Table 3.3) seems appropriate for this situation. Although the impact 
on sales of promotion activities tends to mask its presence, a seasonal sales component is 
present in the data set. Across all years considered, the seasonal component peaks during 
the Christmas and the New Year’s Eve time. We study the impact on sales of seasonality 
through a set of weekly dummy variables. Besides seasonality, the effects of two other 
sales determinants are explored. The first is special events such as Christmas or Thanks-
giving, which are known to influence sales as stores during these periods usually witness 
elevated store traffic levels. The second is promotion types (e.g., Buy one, get one free 
vs. 25% off). As with seasonality, we employ dummy variables to assess how significant 
these effects are on the sales of Quick Quaker Oats.
These arguments have prompted us to use the following model specification to com-
pute the promotion effects:
 
Sc P
P
et
t
t l
Dtl
s
Dts
k
Xtk
k
T
t=⋅ ⎛
⎝⎜
⎞
⎠⎟ ⋅⋅⋅
⎛
⎝
⎜⎜
⎞
⎠
⎟
⎟⋅
=
−
∏
β
εγγ δ, , ,
1
1
 (3.9)
where St are the unit sales in week t; c is a constant equal to the base line sales; Pt is the unit 
price in week t; P–−
t is the regular unit price in week t (derived from the unit prices offered 
during the previous nonpromoted weeks); β is the elasticity of promotional sales with 
respect to the price reduction ratio;  l identifies a Bonus Buy promotion type;  Dt,l is an 
indicator variable equal to 1 if a Bonus Buy promotion is offered in week t, 0 otherwise; 
γl are the promotion effects associated with a Bonus Buy promotion; s identifies special 
events such as Thanksgiving and Christmas; Dt,s is an indicator variable equal to 1 if week 
t is a special event, 0 otherwise; γs is the special event multiplier at the product level; k 
and T refer to a season index (i.e., week) and the maximum number of seasons (i.e., 52 
weeks), respectively; Xt,k is a weekly indicator variable equal to 1 if  k=t, 0 otherwise; δk 
are the seasonal multipliers at the product level; and εt is an independent and identically 
distributed normal error term.
As a preamble to the discussion of how each of the aforementioned factors 
impacts sales, it may be worth providing an explanation of the reasons why the mul-
tiplicative form of the model shown in equation (3.9)  is preferred. In essence, this 
formulation posits that sales are affected multiplicatively by the discount rates, or equiv-
alently, that the percentage change in sales is proportional to the percentage change 
in the price discounts. This formulation departs from the theory of the additive mod-
els, which provides for a proportional relation between the absolute changes in sales 
and discount levels. From an implementation perspective, this subtle difference 
provides retailers with maximum convenience. The sales multipliers computed for

---

## Page 84

Promotion Forecasting  73
various discount levels are scale free, simple to understand, and immediately action-
able. The same applies to the sales multipliers corresponding to the seasonality, pro-
motion, and special events factors, although these are expressed mathematically in 
an alternative form. These multipliers are intended to explain the nonprice-related 
variation in sales.
In its current form, the model shown in equation (3.9) cannot be estimated using the 
linear regression techniques discussed in the previous sections of this chapter. This being 
said, this model can be converted to a linear equivalent through a log transformation. 
For example, if we take the natural logarithm on both sides of this model, we obtain a 
transformed equivalent that is linear in parameters and can thus be analyzed using linear 
regression. The log transformation yields:
 
log log log log ,Sc P
P
Dt
t
t
lt l() = () +⋅ ⎛
⎝⎜
⎞
⎠⎟+ () ⋅+βγ
                     + () ⋅+ () ⋅() +
=
−
∑log log,,γδ εst s kt k t
k
T
DX
1
1  (3.10)
or, equivalently,
 
log log ,, ,SC P
P
DD Xt
t
t
lt l st s kt k t
k
T
() =+⋅ ⎛
⎝⎜
⎞
⎠⎟+⋅ +⋅ + ⋅ () +
=
βε ΓΓ Δ
1
− −
∑
1
. (3.11)
In this formulation, the parameters of the multiplicative model (3.9) can be recovered 
using the following set of identities: c = antilog (C), β = β, γl = antilog (Γl), γs = antilog 
(Γs), and δk = antilog (Δk).
For Quick Quaker Oats, the parameter estimates for both the log transformed and the 
original models are shown in Table 3.6. From these results, it is apparent that only the 
ratio of promoted and regular unit prices and the Bonus Buy promotion significantly 
impact sales. In addition, relative to the reference season (i.e., Christmas week), certain 
weekly seasons lead to significantly differentiated sales levels. To simplify the model, we 
eliminate the insignificant variables from the full model specification and provide the 
parameter estimates for the reduced, or, the more parsimonious model in Table 3.7. In 
this case, a 1% decrease in the price ratio is expected to result in a 2.63% increase in sales 
which signals a price-ratio elastic demand. Similarly, all else equal, a Bonus Buy promo-
tion is expected to affect sales by a multiplicative factor of 1.80. The timing of school 
activities and other major summer holidays appear to also impact sales levels. Relative to 
other weekly seasons, the end of the school in mid-June leads to a moderate drop in sales 
(i.e., weeks 25 and 26). The Fourth of July is also important as the weeks that follow it 
immediately all show reduced levels of sales (i.e., weeks 29–32). Finally, the weeks before 
and after Labor Day, which typically coincide with the end of the summer recess, also 
experience reduced sales volumes (i.e., weeks 35, 36, and 38, respectively). Provided that 
the reduced version of the functional form (3.9) describes adequately the true relation-
ship between sales S
t and the predictor variables Pt/P−
t, Dt,l and Xt,k, the results provided 
in Table 3.7 suggest that the use of the predictor variables reduces the variation in log (St) 
by 56% (i.e., Multiple R-Squared = 0.56).

---

## Page 85

74  Promotion Forecasting
Table 3.6 Log-Transformed and Original Multiplicative Models (Full Model)
Log Transformed Model Original Model
Estimate Std. Errors t value p value Multipliers
Intercept C 3.44 0.2 17.2 0.00 Intercept c (base line) 31.24
Price Ratio β –2.73 0.2 –11.8 0.00 Price Ratio β –2.73
Bonus Buy Γl 0.50 0.1 5.8 0.00 Bonus Buy γl 1.65
Special Events Γs –0.05 0.1 –0.4 0.67 Special Events γs 0.95
Seasonality (Reference: Christmas week) Seasonality
……
Week 25 Δ25 –0.43 0.3 –1.7 0.10 Week 25 δ25 0.65
Week 26 Δ26 –0.44 0.3 –1.7 0.09 Week 26 δ26 0.65
……
Week 29 Δ29 –0.62 0.2 –2.5 0.01 Week 29 δ29 0.54
Week 30 Δ30 –0.47 0.3 –1.8 0.07 Week 30 δ30 0.62
Week 31 Δ31 –0.45 0.3 –1.7 0.08 Week 31 δ31 0.64
Week 32 Δ32 –0.45 0.3 –1.7 0.08 Week 32 δ32 0.64
……
Week 35 Δ35 –0.67 0.3 –2.6 0.01 Week 35 δ35 0.51
Week 36 Δ36 –0.52 0.3 –2.1 0.04 Week 36 δ36 0.60
……
Week 38 Δ38 –0.59 0.3 –2.3 0.02 Week 38 δ38 0.55
……
Residual standard error: 0.3984 on 254 degrees of freedom 
Multiple R-squared: 0.64, Adjusted R-squared: 0.57 
F-statistic: 8.455 on 54 and 254 DF, p-value: < 2.2e-16
Table 3.7 Log-Transformed and Original Multiplicative Models (Reduced Model)
Log Transformed Model Original Model
Estimate Std. Errors t value p value Multipliers
Intercept C 3.31 0.0 119.7 0.00 Intercept c (base line) 27.29
Price Ratio β –2.63 0.2 –12.6 0.00 Price Ratio β –2.63
Bonus Buy Γ1 0.59 0.1 7.4 0.00 Bonus Buy γ1 1.80
Seasonality (Reference: All other weeks) Seasonality
Week 25 Δ25 –0.29 0.2 –1.7 0.09 Week 25 δ25 0.75
Week 26 Δ26 –0.30 0.2 –1.8 0.08 Week 26 δ26 0.74
Week 29 Δ29 –0.49 0.2 –2.9 0.00 Week 29 δ29 0.61
Week 30 Δ30 –0.34 0.2 –2.0 0.05 Week 30 δ30 0.71
Week 31 Δ31 –0.32 0.2 –1.9 0.06 Week 31 δ31 0.73
Week 32 Δ32 –0.32 0.2 –1.9 0.06 Week 32 δ32 0.73
Week 35 Δ35 –0.53 0.2 –3.1 0.00 Week 35 δ35 0.59
Week 36 Δ36 –0.39 0.2 –2.3 0.02 Week 36 δ36 0.68
Week 38 Δ38 –0.46 0.2 –2.7 0.01 Week 38 δ38 0.63
Residual standard error: 0.4107 on 297 degrees of freedom
Multiple R-squared: 0.56, Adjusted R-squared: 0.54 
F-statistic: 33.78 on 11 and 297 DF, p-value: < 2.2e-16
Note: The Special Events indicator variable together with other 42 seasonal indicator variables is removed from the full 
model specification.

---

## Page 86

Promotion Forecasting  75
Armed with these insights, how should the promotion planner prepare for a scheduled 
“Buy three, get the fourth for free” promotion? The reduced variant of the model shown 
in equation (3.9) suggests that it all depends on the time of the year when the promotion 
is intended to be offered. If the promotion takes place close to Christmas, for example, 
then the baseline sales should be adjusted by a multiplier of 2.1 (or, (3/4)
β) to account 
for the implied price discount and then adjusted by a second multiplier of 1.8 (or, γl) to 
control for the Bonus Buy promotion. In contrast, if the promotion is to be offered in 
late July, then the resulting multiplier of 3.8 (or, 2.1 × 1.8) has to be adjusted again by 
a factor of 0.73 (or, 
δ31) to account for the appropriate seasonal effect. Now, what if the 
promotion planner speculates that the computed promotion effects and/or the season-
ality profiles are not appropriate anymore for the situation at hand? Even worse, what 
if she is confronted with a promotion type whose attributes she has not encountered in 
the past? What if, for example, she is strongly recommended to consider promoting the 
product using coupons or in-store cart flyers?
First, if it is felt that a product could borrow effects from the product category it 
belongs to, then the category-level effects could be used on a product holdout sample to 
assess their forecast accuracy and decide whether or not an effect substitution is justified. 
Based on our experience, at times, substituting the own effects for higher-level alternates 
may lead to significantly better results. This approach, however, requires not only a lot 
of additional computing power and IT capabilities but also a deep knowledge of how 
higher-level product groups should be defined. In particular, problems occur when the 
product hierarchies maintained internally by retailers prove to be impractical to forming 
the required groups (e.g., jeans, shirts and boots treated as a group).
The situations that may require you to consider promoting a product in the absence 
of any relevant past promotion history can be tackled in a similar fashion. You could 
attempt to quantify the performance of similar products or groups of products when 
promoted in this particular way and then borrow and apply this information to your 
particular case. Alternatively, across all your products and stores, you could link the 
performance of the promotion type to certain operational characteristics and use the 
discovered relationship to get an understanding of how the performance of your product 
could be impacted. Due to the inherent uncertainty that accompanies both approaches, 
their outcomes are to be expected to be highly variable and presumably less accurate.
SUMMARY
The main goal of time series forecasting is to explain as much of the variation in a prod-
uct’s sales data so that more precise predictions can be made for future sales. For firms 
who offer promotion events and price discounts, these actions produce additional varia-
tion in a product’s sales that can be estimated through causal forecasting models such as 
regression analysis. Causal techniques such as regression serve two important purposes: 
1) they explain some additional variation in a product’s sales that are due to planned 
events such as promotions; and 2) they can be used to measure the effectiveness of given 
promotion or price discount. An example of the latter is to use the estimated coefficient 
of a promotion variable to determine whether the lift in sales is worth the expense of the 
promotion.
One of the simplest causal forecasting methods is simple linear regression, where a 
single independent (predictor) variable, such as whether or not a promotion was offered,

---

## Page 87

76  Promotion Forecasting
is used as a predictor of a dependent variable, such as the sales of a product. Causal fore-
casting models can be estimated in one of two ways: finding the model coefficients that 
result in the minimum least squares fit of the model to the data or finding the model 
coefficients that result in the maximum likelihood that the historical data comes from an 
assumed relationship between the variables and an assumed distribution for the errors. 
The best estimation method to use depends on the model you are trying to estimate. 
When more than one independent (predictor) variable is included in the model (promo-
tion and temperature for example) then a more sophisticated causal method is required, 
such as multiple linear regression.
 The process of estimating promotional effects typically begins with data collection 
and cleaning. One important step that is often neglected is to record any time periods 
when the product was out of stock as well as any out of stocks for other products where 
the demand is likely to be transferred to the product of interest. At this stage, various 
forecasting models can be tested on a holdout sample of the historical data and evaluated 
on the remainder of the historical data. The chosen model can then be used to forecast 
the impact of future promotions, with a continuous refinement of the model as more 
data are collected.
REFERENCES 
Achabal, D. D., McIntyre, S., & Smith, S. A. (1990). Maximizing profits from periodic department store promo-
tions. Journal of Retailing, 66(4), 383–407. 
Cohen, J., Cohen, P., West, S., & Aiken, L. (2003). Applied multiple regression/correlation analysis for the behavioral 
sciences (3rd ed.). Mahwah, NJ: Lawrence Erlbaum Associates, Inc. 
Cooper, L. G., Baron, P., Levy, W., Swisher, M., & Gogos, P. (1999). PromoCast™: A new forecasting method for 
promotion planning. Marketing Science, 18(3), 301–316. 
Foekens, E. W., Leeflang, P. S. H., & Wittink, D. R. (1994). A comparison and an exploration of the forecasting 
accuracy of a loglinear model at different levels of aggregation. International Journal of Forecasting, 10 (2), 
245–261. 
Foekens, E. W., Leeflang, P. S. H., & Wittink, D. R. (1998). Varying parameter models to accommodate dynamic 
promotion effects. Journal of Econometrics, 89(1–2), 249–268. 
Kutner, M., Nachtsheim, C., & Neter, J. (2004). Applied linear regression models (4th ed.). New York, NY: 
McGraw-Hill/Irwin. 
Narasimhan, C. (1984). A price discrimination theory of coupons. Marketing Science, 3(2), 128–147. 
Neter, J., Kutner, M., Nachtsheim, C., & Wasserman, W. (1999). Applied linear statistical models (4th ed.). Chicago, 
IL: Irwin/McGraw-Hill. 
Smith, S. A., & Achabal, D. D. (1998). Clearance pricing and inventory policies for retail chains. Management Sci-
ence, 44(3), 285–300. 
Trusov, M., Bodapati, A. V., & Cooper, L. G. (2006). Retailer promotion planning: Improving forecast accuracy 
and interpretability. Journal of Interactive Marketing, 20(3–4), 71–81. 
Van Heerde, H. J., Leeflang, P. S. H., & Wittink, D. R. (2000). The estimation of pre- and postpromotion dips with 
store-level scanner data. Journal of Marketing Research, 37(3), 383–395. 
Van Heerde, H. J., Leeflang, P. S. H., & Wittink, D. R. (2004). Decomposing the sales promotion bump with store 
data. Marketing Science, 23(3), 317–334. 
Wittink, D. R., Addona, M. J., Hawkes, W. J., & Porter, J. C. (1988). SCAN*PRO: The estimation, validation and 
use of promotional effects based on scanner data. Unpublished manuscript.

---

## Page 88

4
CAPACITY-BASED REVENUE MANAGEMENT
Up to this point, we have discussed how firms group their customers into different 
segments based on their buying behavior and how they forecast the demand for each 
segment, sometimes including the price and/or promotion effects in their forecast. As 
mentioned in our discussion on forecasting, forecasts are never 100% accurate and thus 
any good forecast should include an error estimate. All three of these elements (cus-
tomer segments, forecasts for each segment, and error estimates for each forecast) are 
required before embarking on the topic of this chapter: capacity-based revenue man-
agement. Before beginning this topic, however, we will first explore some of the basic 
concepts behind its science by studying a related and, perhaps, more familiar problem of 
determining an inventory stocking level.
THE SINGLE ORDER OPPORTUNITY INVENTORY PROBLEM
Suppose that you work as a distributor of a product that only has a useful life of a single 
day and can only place a single order each day, before realizing any demand for that day. 
Examples of products with one-day useful lifetimes include newspapers or fresh baked 
goods. Walton’s bagel shop is in such a situation, as they do not have their own bakery 
and thus have to order their bagels to be delivered each morning before opening for busi-
ness. If they do not order enough bagels, they have to turn away demand and thus lose 
out on those sales. If they order too many bagels, they can sell the excess bagels to local gas 
stations at a loss, as the gas stations do not mind selling the “slightly stale” bagels the next 
day. Walton’s pays the bakery $0.40 per bagel, sells them to their customers for $1.00 per 
bagel, and sells any leftover bagels to the gas stations at a price of $0.25 per bagel.
The main decision that Walton’s bagel shop faces each morning is how many 
bagels to order each day. Suppose that Walton’s orders 200 bagels one day but 
demand turns out to be 150 for the entire day. In this case, Walton’s makes a profit of 
($1 – $0.40)150 – ($.0.40 – $0.25)(200 – 150) = $82.50. On another day, Walton’s orders 
200 bagels again but demand turns out to be 300. On this day, Walton cannot take full 
77

---

## Page 89

78  Capacity-Based Revenue Management
advantage of this good fortune because they can only sell the 200 bagels they have in 
stock, thus they make a profit of ($1 – $0.40)200 = $120. If Walton’s faces a daily operat-
ing cost (rent, salaries, general overhead) of $100, then they would lose money on the 
low demand day and make money on the high demand day. Thus, the long-term profit-
ability of their business depends heavily on their ability to make good order quantity 
decisions each morning.
After operating in this environment for a while, Walton’s has used their historical data 
(unconstrained daily sales transactions) to determine that daily demand for their bagels 
follows the distribution shown in Table 4.1. Oddly, daily demand always appears to occur 
only in increments of 50, ranging from a low of 100 to a high of 300. From the table, we 
can determine that daily demands turns out to be equal to exactly 100 20% of the time, 
150 another 20% of the time, all the way up to 300 which only happens 15% of the time. 
Note that we are assuming that demand can never be any value other than the ones listed 
in Table 4.1, that is, it can never be anything other than a multiple of 50 (it will never be 
102 or 276 for example). Because of this, we need only consider five possibilities for the 
daily order quantity (100, 150, 200, 250, or 300). It can be shown that it is never optimal 
to order any quantity outside of these options. If we order 120 for example, we will have 
20 left over if demand turns out to be 100 and be 30 short if demand turns out to be 150. 
Thus, if we decide we want to order more than 100, then the next increment up in the 
order quantity to consider is 150 rather than some quantity between 100 and 150.
Now that we know the demand distribution and our available options for order quanti-
ties, which order quantity should we choose? Demand is typically estimated, or predicted, 
using forecasting methods. In the case of Walton’s bagel shop, the mean of the distribution 
is the point estimate for our forecast and the distribution around the mean is our historical 
forecast error. Ordering the mean of the forecast means that, over time, you are as likely 
to end a day with too many bagels as you are to end the day being short of demand. The 
mean of the distribution in Table 4.1 is 200, which represents the 50th percentile of the 
distribution. This means that if we record the daily demand over a long period of time and 
take the average of these observations, it should be close to 200 bagels. It also means that 
for any particular day in the future, the most likely value for demand that day is 200. Thus, 
at first glance, it may seem logical that we should order the most likely value of demand, 
an order quantity of 200. Suppose we made this order quantity repeatedly, day after day. 
We can calculate what our expected daily profit will be by calculating how much profit 
we make under every possible demand realization and multiplying each one by the prob-
ability that demand will equal that amount. Table 4.2 shows the calculations for this order 
quantity. The values in the bottom row show the profits obtained under each demand 
realization (when demand is 250, for example, the profit is ($1 – $0.40)*200 = $120). The 
Table 4.1 Demand distribution
Probability Demand
0.20 100
0.20 150
0.10 200
0.35 250
0.15 300

---

## Page 90

Capacity-Based Revenue Management  79
expected profit is the sum of the probabilities times each of the resulting profits (.20*$45 + 
.20*$82.50 + .10*$120 + .35*$120 + .15*$120 = $97.5).
Unfortunately, repeatedly ordering 200 bagels every morning results in an average 
daily profit that is less than Walton’s daily operating cost of $100. Thus, the next ques-
tion is if you should order some other quantity instead of 200 and, if so, should it be 
lower or higher than 200. The answer depends on the marginal cost of having too much 
inventory versus the marginal cost of not having enough. If these two costs are equal, 
then ordering the forecast mean is the optimal decision. In most cases, however, these 
two costs are not equal. In Walton’s case, the cost of having one too many bagels at the 
end of the day is the cost of the bagel minus what we can sell the extra bagel for, or $0.40 
– $0.25 = $0.15. Thus, the cost of having more stock than demand is $0.15 per bagel. If 
you do not have enough bagels to meet demand, the marginal cost can be estimated as 
the loss of the profit margin you would have made if we had another bagel in stock, or 
$1.00 – $0.40 = $0.60. Of course, we are assuming here that we do not incur any loss of 
goodwill from the customers who show up wanting a bagel but we do not have any to 
serve them. Even ignoring this cost, the marginal cost of being short of demand (cost of 
underage) is greater than the marginal cost of having more stock than demand (cost of 
overage), as $0.60 > $0.15.
Consider for a moment what it means for the cost of underage to be greater than the 
cost of overage. This implies that you are typically better off if you end most days with 
excess inventory rather than with a shortage. Of course, you make the most money if 
you order the exact amount that is demanded, but you are unlikely to be able to do this 
consistently because of the forecast error. Ordering the mean of the forecast implies that, 
over a long period of time, around 50% of the time you will end the day having to turn 
some customers away who want to purchase bagels but you no longer have any to sell 
them (a 50% service level). Comparing marginal costs tells us that you want to have a 
higher service level than this, but how much higher?
Because the number of demand realizations (and thus order quantity options) is lim-
ited, this question can be answered for Walton’s bagel shop in a brute force method. One 
need simply calculate the expected profits for each of the order quantities possible and 
compare the resulting expected profits. This is done in Table 4.3, with an order quantity 
of 250 showing the largest expected profit of $108.75. This fits our intuition, as our com-
parison of the overage versus the underage cost indicted that we should order a larger 
quantity than the mean of the demand distribution. Ordering 250 each day should also 
make you profitable, as an average daily profit of $108.75 is greater than our daily oper-
ating cost of $100. Note that Walton’s does not actually make $108.75 on any given day. 
If you consistently order 250 bagels each morning, 20% of the days (those with demand 
of 100) you will make $37.50, another 20% of the days (those with demand of 150) you 
will make $75, etc., but the average over all of the days should be close to $108.75. Thus, 
Table 4.2 Expected Proﬁ  t Calculation for an Order Quantity of 200 bagels
Probability (top) and Demand Realization (bottom)
0.20 0.20 0.10 0.35 0.15 Expected 
Profit
  97.5
Order Qnty
   2 0 0
100 150 200 250 300
$45.00 $82.50 $120.00 $120.00 $120.00

---

## Page 91

80  Capacity-Based Revenue Management
consistently ordering 250 bagels each morning provides us with the highest average profit 
than does ordering any other amount. For this reason, we define 250 as the “optimal” 
order quantity.
For the example above, a brute force approach worked because the number of possi-
ble demand realizations was small. Suppose that instead of only having the five possible 
demand realizations, the daily demand for bagels could be any discrete number between 
0 and 1000. To use the brute force method in this case, you would need a probability for 
each possible realization of demand. You would also need a very large table, much larger 
than Table 4.3.
In practice, demand distributions are often first assumed based on looking at the his-
torical sales data and then estimated using the historical forecast error. The forecast is 
typically used to estimate the mean of the demand distribution and the forecast error is 
used to estimate the type and spread of the distribution. Thus, daily demand at Walton’s 
may be estimated by first assuming that it follows a Normal Distribution, with a mean 
of 200 and a standard deviation of 50. The Normal Distribution is a continuous distri-
bution which means, in theory, that demand can take on any fractional value such as, 
for example, 213.6 bagels. While Walton’s will probably never sell a fraction of a bagel, 
using a continuous distribution to approximate demand is common practice and should 
not be too bad of an estimate unless the mean of the demand distribution is small, say 
less than 30 units. If more accuracy is required, there are plenty of discrete distributions 
available to use instead.
Assume for now that the daily bagel demand is Normally distributed with a mean of 
200 and a standard deviation of 50. How should you use this information to determine 
the best ordering quantity? The brute force method described earlier will be too cumber-
some in this case so we need an alternative method. You could always do the trial and 
error method, where you try the same order quantity for a large number of days and 
record the average profit over those days. You could then compare this average profit 
against another average profit calculated after trying another order quantity. The prob-
lem with this approach is that you will probably be retired by the time you finally deter-
mine the best order quantity, or your firm will be out of business because you choose 
poorly for too many days in a row. A commonly used approach that approximates this 
practice is to use Monte Carlo Simulation. This method involves simulating the retail 
environment on a computer by taking a bunch of random draws from the demand dis-
tribution to replicate the randomness of demand over a large number of days. Different 
order quantities can be evaluated against these random draws and the average profits can 
Table 4.3 Expected Proﬁ  ts for Each Order Quantity Option
Probability (top) & Demand Realization (bottom)
0.20 0.20 0.10 0.35 0.15
Order Qnty 100 150 200 250 300 Expected Profit
100 $60.00 $60.00 $60.00 $60.00 $60.00 $60.00
150 $52.50 $90.00 $90.00 $90.00 $90.00 $82.50
200 $45.00 $82.50 $120.00 $120.00 $120.00 $97.50
250 $37.50 $75.00 $112.50 $150.00 $150.00 $108.75
300 $30.00 $67.50 $105.00 $142.50 $180.00 $106.88

---

## Page 92

Capacity-Based Revenue Management  81
be compared to see which order quantity is best. Thus, simulation replicates the trial and 
error method, but in a much safer and faster environment. An analogy for using simula-
tion to solve an inventory problem such as Walton’s is when an inexperienced gambler 
practices different strategies at home for a particular card game such as blackjack before 
playing the game for real money at a casino. Of course, most experienced players of 
blackjack already know there is an optimal strategy that tells you, for any combination of 
your cards and the card that the dealer is showing, the optimal next move. An equivalent 
optimal strategy for Walton’s problem is our next topic.
THE NEWSVENDOR MODEL
The basic problem that Walton’s faces for its daily bagel orders can be found in many dif-
ferent industries where the firm faces a single order opportunity where the order quan-
tity is used to meet some future uncertain demand and there is no cost effective means 
for altering the order quantity after the actual demand amount is realized. The classic 
example of where this problem occurs is where a vendor selling daily newspapers has 
to decide each morning how many copies of that day’s newspaper to pick up from the 
publisher. Since the demand for day-old newspapers is practically zero, when the vendor 
makes his/her ordering decision he/she must balance the cost of ordering too many, ver-
sus too few, newspapers. The solution to this problem serves as a foundation for most of 
the more advanced inventory theory and takes its name from this classic application: the 
newsvendor model. Before explaining the solution to this problem, we first review how 
demand uncertainty is typically captured in problems such as this one.
Let x represent the daily demand for bagels and F(x) represent the probability that 
the daily demand for bagels is less than or equal to x. A common assumption about the 
distribution of demand is that it is Normally distributed. The Normal distribution is 
symmetrical and is shaped like a bell, with the amount of variability in the distribution 
represented by its standard deviation (SD). Figure 4.1 shows a typical Normal distribu-
tion curve where the middle vertical line represents the mean of the distribution and the 
other vertical lines represent the standard deviations to the right or left of the mean.
x 1SD 2SD 3SD
Figure 4.1 Normal Distribution Curve

---

## Page 93

82  Capacity-Based Revenue Management
The shaded area under the Normal Distribution curve represents the percentage of 
the population to the left of a given value on the x-axis. Thus, if all of the area under the 
curve to the left of the mean is shaded, this corresponds to 50% of the population. As the 
shaded area moves to the right, this corresponds to larger percentages of the total popu-
lation. A useful tool for linking the percentage of the shaded portion of the distribution 
to any point on the x-axis (relative to the mean) is the Standard Normal Distribution 
table, a sample of which is shown in Table 4.4. In this table, the number of standard 
deviations from the mean is represented by the z-value, which is read by combining the 
integer values in the left-most column with the first digit values in the top row. The val-
ues in the table correspond to the percentage of the population that is contained to the 
left of z standard deviations to the right of the mean. Thus, a value that is z = 1.3 standard 
deviations to the right of the mean contains 90.3% of the distribution. You can calculate 
a z value for any value contained within a distribution. For example, suppose that the 
demand is Normally distributed with a mean of 200 and a standard deviation of 50. If, on 
a particular day, demand turns out to be 270, the corresponding z-value is 
z = − = − =270 270 200
50 14μ
σ .
Another way of stating this is that a demand realization of 270 is 1.4 standard deviations 
to the right of the mean.
Now let’s return to our example where the daily bagel demand is assumed to be Nor-
mally distributed with a mean of 200 and a standard deviation of 50. Knowing these 
three things about the demand (the mean, the standard deviation and the form of the 
distribution) allows you to convert any order quantity into a corresponding service level, 
as measured by the probability that you will run out of stock before the next replenish-
ment arrives. Thus, an order quantity of 250 is one standard deviation to the right of the 
mean which we can determine, by using Table 4.4, corresponds to an 84.1% probability 
that we will not stock out of bagels on any particular day, or F(Q = 250) = 0.841. Another 
way of interpreting this relationship is as follows: if Walton’s repeatedly ordered 250 
bagels each day over a very long time period, we would expect that they would not stock 
out approximately 84.1% of those days. Correspondingly, this means that they will run 
out of bagels on 15.9% of the days. Figuring out what exactly is the right service level to 
stock for is the focus of the newsvendor model. Before introducing the model, we first 
have to provide some notation as it relates to Walton’s problem of ordering bagels.
Let Q represent the quantity of bagels you decide to order each morning, p be the price 
a bagel is sold at, c be the unit marginal cost of making a bagel, and s be the salvage value 
(the price the leftover bagels are sold at to the gas station), where s < c. Assume you have 
Table 4.4 Standard Normal Distribution Table
z 0.0 0.1 0.2 0.3 0.4 0.5 0.6 0.7 0.8 0.9
0.0 0.500 0.540 0.579 0.618 0.655 0.691 0.726 0.758 0.788 0.816
1.0 0.841 0.864 0.885 0.903 0.919 0.933 0.945 0.955 0.964 0.971
2.0 0.977 0.982 0.986 0.989 0.992 0.994 0.995 0.997 0.997 0.998
3.0 0.999 0.999 0.999 1.000 1.000 1.000 1.000 1.000 1.000 1.000

---

## Page 94

Capacity-Based Revenue Management  83
currently been ordering Q = q bagels each morning. The decision you face is whether or 
not to increase the ordering quantity by one additional bagel, or Q = q+1. If the realized 
demand X is less than q+1, the effect on the expected profit of ordering the additional 
bagel is that Walton’s will have one additional unsold bagel at the end of the day, incur-
ring a cost of c – s. We term this difference the cost of overage, Co. If the realized demand 
X is greater than or equal to q+1, the effect on the expected profit of ordering the addi-
tional bagel is that Walton’s will sell one additional bagel, making an additional profit 
of p – c. This increase in profit can also be viewed as an opportunity cost of not ordering 
one additional bagel, or the cost of underage, C
u. Defining the overage and underage cost 
in this way allows a simple equation for determining the optimal order quantity, Q*. It 
turns out that the optimal ordering quantity should be set such that the percentage of 
demand met by that service level is greater than or equal to the underage cost over the 
sum of the overage and underage cost, or: 
FQ
C
CC
u
uo
() * ≥
+
The equation above is the infamous newsvendor model. The fraction on the right-hand 
side of the equation provides the optimal service level. As the cost of being under demand 
gets larger (relative to the cost of being over demand), it makes sense for a firm to stock 
more and provide a higher service level. This fraction is called the “critical ratio” because 
of its simplicity and importance. For Walton’s, the critical ratio is as follows:
C
CC
pc
pccs
u
uo +
=
−
−+−
= −
−
==14
12 5
6
75
08.
.
.
.
.
The calculation above shows that Walton’s should order enough bagels each day such 
that they have an 80% chance of not running out of bagels before the end of each day. 
Table 4.4 provides the z-value that corresponds to at least 80% of the population. Look-
ing at the values in Table 4.4 shows that a z-value of 0.9 provides the closest service level 
to 80% that still exceeds 80%. Thus, Walton’s optimal number of bagels to order each 
morning is:
Q = 200 + 0.9*50 = 245 bagels
A more precise estimate of the z-value can be found using the function = NORMSINV() 
in Microsoft Excel. For example, to find the z-value for an 80% service level, simply type 
the function = NORMSINV(0.8) in a cell to get the corresponding z-value = 0.8416 … 
This z-value gives the more precise optimal order quantity of Q = 200 + 0.8416*50 = 
242.8 or 243 bagels. Note that the Normal distribution is symmetrical, so Table 4.4 can 
also be used to find z-values corresponding to service levels of less than 50%. For exam-
ple, the z-value for a service level of 20% is found by taking the negative of the z-value for 
(1 – 0.2) in Table 4.4, or z = –0.9. The order quantity that results in a 20% service level 
is thus Q = 200 – 0.9*50 = 155 bagels (or Q = 200 – 0.8416*50 = 157.9 bagels using the 
more precise z-value).

---

## Page 95

84  Capacity-Based Revenue Management
DETERMINING BOOKING LIMITS IN REVENUE 
MANAGEMENT PROBLEMS
Capacity-Based Revenue Management, sometimes referred to as Yield Management, 
refers to techniques for allocating limited resources such as airplane seats or hotel rooms 
to different customer segments at different price points. Referring back to the first chap-
ter on customer segmentation, recall that travel customers are often segmented based on 
whether they are traveling for business or leisure. People traveling on business are typi-
cally less price sensitive than are people who travel for leisure, since the former are often 
being reimbursed for their travel expenses.
Imagine that you manage a hotel that serves both business and leisure customers. 
Since business travelers are willing to pay more for your hotel rooms, you prefer to price 
your rooms accordingly and only sell to business customers. Of course, like most things, 
the demand for business travelers is seasonal and contains forecast error. Thus, on most 
nights it is not possible to sell your entire capacity of rooms to only business travelers. 
Because the marginal cost of selling a room is typically very low, it is profitable to sell the 
remaining rooms to leisure customers at a lower price. This would be an easy problem if 
the business customers booked their rooms early and the leisure customers waited until 
the last minute. In this case, you could simply sell as much of your capacity to the busi-
ness customers as you could and then sell any remaining capacity to leisure customers.
Of course, the opposite is typically true in practice, as business customers often have 
to make their travel plans at the last minute while leisure customers, who are often 
traveling on vacation, may know their travel plans months in advance. Thus, the chal-
lenge becomes determining how many rooms to sell at a low price to the leisure cus-
tomers and how many to sell at a high price to any potential future business customers. 
Complicating this challenge is the fact that after a point in time, the capacity expires and 
any unsold capacity can never be sold again (e.g. an unsold room for Jan 24 cannot be 
sold on Jan 25). The problem of “expiring capacity” is faced by the majority of firms in 
the travel and hospitality industry, including airlines, hotels, rental cars, cruise lines and 
many others. Thus, it is not surprising that the science behind capacity-based revenue 
management was first developed in, and still most widely practiced in, this industry.
For the travel and hospitality industry, capacity-based revenue management is used 
to solve the problem of determining how many hotel rooms (or airline seats, rental cars, 
etc.) to allow lower willingness-to-pay customers to purchase when there is the possi-
bility of future higher willingness-to-pay customer demand. Note that this application 
of revenue management does not involve actually setting the prices, as the prices are 
assumed to be set exogenously to be competitive in the market. From the customer’s 
perspective, however, it often appears that prices are constantly changing. Every frequent 
traveler probably has a story of how they were ready to book an airline ticket online only 
to see the price increase by several hundred dollars just as they were ready to confirm the 
purchase. To the person trying to purchase the ticket, it appears that the airline changed 
the price just before they purchased. What actually happens, in most cases, is that some-
one else had just purchased a seat on that same flight which put the number of seats the 
airline was willing to sell at the lower price over something called a booking limit.
Booking limits allow firms to place a limit on the amount of their expiring capacity 
that they are willing to sell at a discounted price. This helps firms avoid selling all of their 
capacity at the discount rate so as to reserve some capacity for the higher willingness-
to-pay customers. The practice of placing booking limits grew out of the U.S. airline

---

## Page 96

Capacity-Based Revenue Management  85
industry immediately following the deregulation era in the early 1980s when the “legacy” 
airlines began facing competition from multiple startup “low cost” airlines. The legacy 
airlines knew that their cost structures were not competitive with the low cost airlines 
such that they could not profitably match the lower fares that the new airlines were offer-
ing. The legacy airlines did still have some advantages over the startup airlines, however, 
as they had a greater variety of flight times, higher service levels, and well-established 
frequent flyer programs. These advantages were valued higher by the frequent business 
travelers than by the less frequent leisure travelers, who flocked to the lower fares offered 
by the low cost airlines. The main problem for the legacy airlines was that there were not 
enough business travelers, who were willing to pay their full fare prices to fill up their 
planes, resulting in many empty seats on each flight. The full-fare prices were set such 
that the legacy airlines could still make a profit, even with their higher cost structures.
The epiphany that saved the legacy airlines (or at least bought them another 20 years) 
was that they did not need to consider their total cost when deciding how to price their 
seats but rather the marginal cost of one additional passenger, which is close to zero. 
Thus, any revenue that they could make for a seat that would be empty when the flight 
departed would add directly to their bottom line. By discounting their fares for the seats 
that would have flown empty, they could even undercut the prices of the low cost carri-
ers. This becomes a very profitable strategy as long as you can minimize the number of 
seats that are demanded, but no longer available, for the higher willingness-to-pay busi-
ness travelers. To accomplish this requires two things: 1) good segmentation fences, as 
discussed in Chapter 1, to keep the business travelers from buying the discounted fares; 
and 2) a booking limit to keep the leisure customers from taking up too many of the 
available seats. Our next topic is on how these booking limits are set.
To help introduce the science behind how to set booking limits, imagine that you are 
the manager for a Hyatt hotel in downtown Atlanta. This Hyatt has 100 identical rooms 
and has established two rate classes, or buckets, for pricing these rooms: a full price and a 
discount price. The Hyatt offers a discounted rate of r
L = $150 (low rate) for a mid-week 
stay targeting leisure travelers and a regular “rack rate” of rH = $400 (high rate) targeting 
business travelers. We denote the uncertain demand from the business travelers (and, 
subsequently, the demand for the high rate rooms) as DH. Let F(DH) represent the prob-
ability that the nightly room demand for business travelers is less than or equal to  DH. 
From historical transaction data, you have estimated that D H is Normally distributed 
with a mean of 30 and a standard deviation of 3. While the goal is to establish a booking 
limit (i.e., the number of rooms you are willing to sell at the discounted rate), it is easier 
to visualize the reciprocal problem of how many rooms to protect. The protection level 
(denoted as Q) is the number of rooms the hotel reserves for the business travelers (high 
rate). Since there are 100 rooms available in the hotel, and just two rates, the correspond-
ing booking limit = 100 – Q. Thus, the Hyatt will sell no more than 100 – Q rooms at 
$150 and protect (or reserve) Q rooms at the $400 rate for the later arriving business 
customers (Figure 4.2).
At the heart of the booking-limit problem is the trade-off between setting the booking 
limit too high and setting it too low. If you set the discount booking limit too low (we 
protect too many rooms, i.e., D
H < Q), you will turn away leisure (low rate) customers 
but will end up not selling all of the reserved rooms to the business (high rate) custom-
ers. Just as in our earlier inventory example, the marginal cost of reserving one too many 
rooms is captured by the overage penalty C
o, which, for a hotel such as the Hyatt, is the

---

## Page 97

86  Capacity-Based Revenue Management
opportunity cost of not selling one additional room at the discounted rate rL. However, if 
you protect one room too few, i.e., DH > Q,then you incur an underage penalty, Cu, equal 
to the opportunity cost of not being able to sell that room at the full rate: Cu = rH – rL. If 
this seems oddly familiar, it is because the concept of overage and underage costs is the 
same as in the previous inventory problem. In fact, the solution takes the same form as 
well, the critical ratio of the newsvendor model:
FQ
C
CC
u
uo
() * ≥
+
For the Hyatt, the critical ratio is calculated as:
C
CC
rr
r
u
uo
HL
H+
=
−
= − ==400 150
400
250
400
0 625.
To find the protection level that provides a 62.5% chance that the demand for business 
travelers will not exceed the number of rooms reserved for them, you find the corre-
sponding z-value in Table 4.4  that comes the closest to 0.625. Looking at the values in 
Table 4.4 shows that a z-value of 0.3 provides the closest value to this percentage. Thus, 
the Hyatt’s protection level is: Q = 30 + 0.3*3 = 30.9 or 31 rooms. Similarly, the booking 
limit is calculated as 100 – Q = 69 rooms. This implies that, assuming the leisure cus-
tomers arrive before the business customers, after the sixty-ninth room has been sold at 
the $150 rate, this discounted rate should be removed from the set of available options 
available to the customer. This is typically what is happening when you find a low rate 
or fare but it becomes unavailable before you can finalize the purchase—someone else 
has purchased the last unit of capacity available in that rate’s booking class or the entire 
capacity of the hotel has been sold. As with the inventory example, you can also calculate 
a z-value using the function = NORMSINV() in Microsoft Excel.
Booking Limits with More Than Two Customer Segments
The newsvendor model provides a simple solution for finding the optimal protection 
levels (or booking limits) in the special case where there are only two customer classes. 
Sell no more than the low 
room price booking limit, 
100 – Q
0 100 rooms
Q rooms protected for
high room price
customers
Figure 4.2 Protection Level and Booking Limit in a Hotel Context

---

## Page 98

Capacity-Based Revenue Management  87
In practice, most firms who practice capacity-based revenue management divide their 
customer base into more than two segments and offer more than two rates or fares.
The challenge in extending the newsvendor model to applications with more than 
two customer segments comes from two sources: determining how to estimate the 
overage and underage cost and estimating the demand distribution for the higher will-
ingness-to-pay customer classes. As an example, consider the case where the Hyatt 
introduced a third customer segment whose willingness-to-pay fell in between that of 
the leisure and business travelers. This segment could consist of self-employed busi-
ness travelers, who have to pay for their own travel expenses rather than being reim-
bursed by their employee. Thus, expecting that this segment is not as price sensitive 
as the leisure traveler but is more price sensitive than the original business traveler 
segment, you introduce a third room rate option of $250. Now, return to the problem 
of determining how many rooms to protect for customers booking at the $400 rate. 
How should you estimate the overage cost, the cost of reserving one too many rooms 
at the $400 rate? If a room goes empty, it could have been filled at either the $250 rate 
or the $150 rate. A similar problem arises in estimating the underage cost; is it $400 
– $250 or $400 – $150?
A second complication of determining booking limits for more than two segments is 
that a strict enforcement of a prescribed booking limit for each rate class does not make 
logical sense. Using the three rates for the Hyatt as an example, suppose that booking 
limits are set as follows: 69 room limit at the $150 rate, 16 room limit at the $250 rate, 
and 15 room limit (the remaining capacity) at the $400 rate. Often times, in practice, 
the higher rate products contain fewer restrictions than the lower rate products, such as 
being fully refundable. The result of having products with different restriction levels is 
that there is no longer a strict order of arrival, with the demand for the lower rate rooms 
always occurring before the demand for the higher rate rooms. Thus, it is common for 
some demand for rooms at the higher rate to occur even if options are still remaining 
at the lower rates. Therefore, it is plausible for the Hyatt to have sold all of its allotted 
rooms at the $400 rate but still have not reached the booking limit for the rooms at the 
$250 rate. Of course, it is not optimal to deny someone who is willing to pay $400 so as 
to save a room for someone else who is only willing to pay $250. To avoid scenarios such 
as this, most capacity-based revenue management systems today use something called  
nested booking limits.
When using nested booking limits, a high rate room request will never be refused as 
long as any rooms remain available in lower rate classes. It is thus binding in its limits 
on lower rate classes, but its limits are “transparent” for higher rate classes. To describe 
how nesting works, we first switch our example to an airline selling multiple fares for the 
same coach-class seats on a flight. As a first step, you should number the different fare 
classes so that 1 is the highest fare class and n is the lowest. Figure 4.3 provides an exam-
ple with four fare classes, with each nested booking limit termed a bucket. Define b
i as the 
nested booking limit for fare class i. Each nested booking limit represents the maximum 
number of seats that may be sold to a fare class, including all lower fare classes with their 
own smaller booking limits (Belobaba, 1987). The nested booking limit on the highest 
fare class b
i is the total capacity of the coach-class cabin. The equivalent nested protec-
tion level for class i is the total number of seats available to fare class i customers and to 
all the higher fare classes.

---

## Page 99

88  Capacity-Based Revenue Management
Solving the Nested Booking Limit Problem: The EMSR-b Solution
Now suppose the airplane has a total capacity of 300 coach-class seats. Table 4.5 shows 
fare prices and demand estimates for each fare class.
Note that the fare classes are numbered in descending fare order, that is,  f 1 > f 2> 
f3> f4. We have used the historical booking data for this flight to estimate that demand for 
each fare class is Normally distributed, with the mean and the variance of each distribu-
tion provided in Table 4.5. Note that we are providing the variance of each distribution 
in Table 4.5 rather than the standard deviation (for reasons that will become obvious 
shortly). The standard deviation can easily be calculated by taking the square root of 
the variance. Also note that the demand for fare class 4 is essentially unlimited, for our 
purposes. This simply means that we can always sell out the entire 300-seat capacity at 
the $50 per seat rate.
A major assumption behind most newsvendor-type revenue management models is 
that the demand distributions for each of the fare classes are independent of the demand 
in the other classes. This means that, for example, a very high demand for fare class 2 
does not tell us anything about whether demand will be high or low for fare class 1, 3, or 
4. We will return to this assumption later in this chapter. A second major assumption 
is that there will be no failures to show or cancelations. The challenge for handling the 
Bucket 2
Bucket 3
Bucket 4:
lowest fare
Bucket 1: Higest fare
Figure 4.3 Nested Fare Class Buckets.
Table 4.5 Fare class prices and distribution parameter values
Class Fare Demand
Mean Variance
f 1 250 50 50
f 2 150 75 75
f 3 100 125 125
f 4 50 Unlimited

---

## Page 100

Capacity-Based Revenue Management  89
“no-show” and cancelation problem is termed the overbooking problem . Incorporating 
overbooking levels into the capacity-based revenue management solution is common in 
practice, but it is beyond the scope of this chapter. We are now ready to explore the solu-
tion to the more than two segment revenue management problem.
Expected Marginal Seat Revenue Model (EMSR)
Belobaba (1987, 1989) extended the basic newsvendor problem and developed a heuristic 
decision rule for finding seat protection levels and booking limits for more than two fare 
classes. He named his new model the Expected Marginal Seat Revenue (EMSR) model 
for nested booking classes. EMSR comes in two flavors: EMSR-a and EMSR-b, but the 
latter is the most commonly used, so this is the version we discuss in this chapter.
To use the EMSR- b model, assume that a customer displaced by an additional book-
ing for a lower fare class customer would be paying a fare equal to a weighted average of 
all the fares above the fare class where the booking actually occurred. To model this, cre-
ate an “artificial class” with demand equal to the sum of the demand distributions for all 
the higher fare classes and a fare equal to the weighted average of the higher fare classes. 
Then use the previously discussed newsvendor critical ratio to calculate the booking 
limit of the current class with respect to the artificial class. The solution to the model 
provides a set of nested protection levels that protect a block of seats for each fare class 
and any higher fare classes. Explaining the model first requires some notation.
Consider an application where there are n distinct fare classes, labeled from the highest 
fare class i = 1 to the lowest fare class i = n. Assume that demand in all the fare classes fol-
lows independent normal distributions, let the demand distribution in class i (denoted 
by d
i) be represented with a mean of µ i and a standard deviation of σi. Denote θi as the 
nested protection level for all fare classes i and higher. For example, θ1 is the protection 
level for Fare Class 1 while θ2 is the protection level for Fare Classes 1 and 2. Let Xi denote 
the cumulative demand of all the fare classes from Class 1 to Class i, which has a mean 
and standard deviation of
μμ σ σi j
j
i
i j
j
i
==
==
∑∑
1
2
1
and
It is important to remember here that the sum of two independent Normal distributions 
forms a new Normal distribution with a mean equal to the sum of the two means and 
a standard deviation equal to the square root of the sum of the variances. This is why 
we described the demand distributions in Table 4.5 using variances instead of standard 
deviations. Finally, let fi denote the weighted average fare for Classes 1 to Class i, which 
is calculated as follows
f
f
i
jj
j
i
j
j
i
=
=
=
∑
∑
μ
μ
1
1

---

## Page 101

90  Capacity-Based Revenue Management
The optimal nested protection levels, θi, can now be found by finding the largest integer 
value that satisfies
fP X f
PX ff
f
ii ii
ii
ii
i
>() =
≤() = −
+
+
θ
θ
1
1or 
Notice that the second equation is of the same form as the critical ratio of the newsven-
dor model. The cost of underage is the weighted average fare of all the higher fare classes 
minus the next lowest fare (
fi – fi+1) while the cost of overage is the price of the next 
lowest fare (f i+1). Once the optimal nested protection levels are found, the equivalent 
nested booking limits can be calculated by subtracting the protection levels from the 
total capacity. EMSR-b is considered a heuristic because it uses a weighted average of the 
higher fares, which are calculated using the means of the higher fare class distributions. 
The use of means, however, is an approximation because booking limits will also be set 
on the higher fare booking classes. Thus, the actual observed mean demand of each class 
will typically be different than the true mean. In various simulation studies, however, the 
resulting protection levels calculated using EMSR-b have been shown to be very close to 
the true optimal protection levels (see, e.g., Talluri & van Ryzin, 2004, section 2.2.4.3). 
Next, we demonstrate how to apply the EMSR-b method on our example data from 
Table 4.5.
Example of EMSR-b Method
To demonstrate the EMSR-b method, consider a 300-seat capacity plane with four fare 
classes defined by the prices and demand distribution parameter values provided in 
Table 4.5. The nested protection levels for the top three fare classes (Fare Classes 1–3) 
can be found via a three-step process.
1. Find the cumulative distributions.
Class Fare Mean Variance Cum-Mean µ¯i Cum-Var /H9268¯i
2
f1 250 50 50 50 50
f2 150 75 75 125 125
f3 100 125 125 250 250
f4 50 Unlimited
Thus X–
1~N(50,50), X–
2~N(125,125) and X–
3~N(250,250)
2. Find the weighted average fares.
f
f
f
jj
j
j
j
1
1
1
1
1 1 250== =
=
=
∑
∑
μ
μ

---

## Page 102

Capacity-Based Revenue Management  91
f
f jj
j
j
j
2
1
2
1
2
250 50 150 75
50 75 190== +
+ =
=
=
∑
∑
μ
μ
() ( ) () ( )
f
f jj
j
j
j
3
1
3
1
3
250 50 150 75 100 125
50 75 12== ++
++
=
=
∑
∑
μ
μ
() ( ) () ( ) () ()
5 5 145=
3. Solve for the protection levels.
For Fare Class 1: 
f2 = f1 P(X–
1 > θ1)
PX ff
f() .11
12
1
100
250 4≤= − ==θ
X–
1~N(50,√50—) gives
θ1 = NORMINV (.4,50,√50—) = 48.2 or 49 seats
For Nested Fare Class 2: 
f3 = f2 P(X–
2 > θ2)
PX ff
f() .22
23
2
90
190 47≤= − ==θ
X–
2~N(125,√125) gives
θ2 = NORMINV (.47,125,√125) = 124.2 or 125 seats
For Nested Fare Class 3:
f
4 = f3 P(X–
3 > θ3)
PX ff
f() .33
34
3
95
145 66≤= − ==θ

---

## Page 103

92  Capacity-Based Revenue Management
X–
3~N(250,√250) gives
θ3 = NORMINV (.66,250,√250) = 256.5 or 257 seats
Because the airplane has a total capacity of 300 seats, you should not sell more than 43 
seats (300–257 = 43) at the $50 fare. Once the number of seats sold at the $50 and $100 
fare prices exceeds 175 (300–125 = 175), you should not sell any more seats below the 
$150 fare price. The resulting nested protection levels are summarized in Table 4.6.
NETWORK REVENUE MANAGEMENT
Setting protection levels via methods such as EMSR-b tends to work well for a single-
capacity resource on a single date. Complications arise, however, when the capacity is 
spread over multiple resources such as a multi-leg flight or multiple time periods such as 
a multi-night stay at a hotel. To understand why this is the case, consider a connecting 
flight from Columbia, SC to New York, NY. Delta Airlines, for example, does not offer 
a direct flight for this route but they do offer a connecting flight through Atlanta. Thus, 
a customer who books a Delta flight from Columbia to New York potentially displaces a 
Columbia to Atlanta passenger as well as an Atlanta to New York passenger. Of course, 
since Atlanta is the hub terminal for Delta, they could also be displacing a Columbia to 
Chicago passenger, or, a Columbia to Paris passenger. The same problem occurs when 
the resource can be used over multiple time periods, as a customer who reserves a hotel 
room for a Wednesday night potentially displaces a customer who wants to reserve the 
room for a Monday–Friday stay. The challenge in trying to apply a newsvendor-type 
model to this problem comes from deciding what fares or rates to use to calculate the 
overage and underage costs. The calculations of booking limits (or protection levels) for 
problems such as these that involve multiple resources or time periods are done through 
Network Revenue Management Models. The most common method used for solving Net-
work Revenue Management problems is a technique termed Bid Price Controls.
Bid Price Controls
Bid Price Control methods avoid the problem of calculating a booking limit (or, a 
protection level) for every fare class by calculating instead a single bid price that is a 
function of the remaining capacity and the time remaining until the consumption of 
the resource. Once calculated, total revenue projections are made for all requests for a 
unit of capacity and this revenue is compared to the bid price (the minimum accept-
able revenue for a unit of capacity) to see if the request should be accepted. If the esti-
mated revenue for a request is above the bid price for that resource, then the request 
is accepted; if it is not, then it is rejected. Thus, bid prices represent the opportunity 
Table 4.6 Nested Protection Levels Calculated Using EMSR-b
Class Fare Mean Variance Protection Levels /H9258i 
f1 250 50 50 49
f2 150 75 75 125
f3 100 125 125 257
f4 50 Unlimited – 300

---

## Page 104

Capacity-Based Revenue Management  93
cost for one unit of capacity of a resource. The reason bid price systems work well 
for network revenue management problems is that bid prices can be calculated for 
every resource or every time period and then added together for evaluating requests 
that involve multiple resources or time periods. Returning to our Columbia to New 
York flight example, if the bid price for the Columbia to Atlanta flight is $100 and 
the bid price for the Atlanta to New York flight is $200, then Delta should only make 
fare classes available for the Columbia to New York flight that exceed the combined 
$300 bid price. The logic behind how a bid price system would work for managing the 
selling of hotel rooms is shown in Figure 4.4 . In practice, this logic takes place proac-
tively and behind the scene such that the customer is only shown (displayed) the room 
options that are priced higher than the bid price.
While there are clear advantages from using bid prices for network revenue manage-
ment problems, the calculation of the bid prices is typically much more complicated 
than is the calculation of booking limits via the newsvendor models such as EMSR-b. 
For this reason, the most common approach used in practice is to simplify the problem 
by assuming that there is no uncertainty in the forecasts for each fare class. As discussed 
in Chapter 2 , there is no such thing as completely accurate forecasts, so this is clearly 
an approximation. This approximation does, however, allow the problem to be solved 
using deterministic methods such as linear programming. In fact, some simulation stud-
ies have shown that a deterministic approximation of the network revenue management 
problem (with frequent re-optimization) may even outperform the more complex, and 
computationally intensive, stochastic versions of the same problem. Thus, we only out-
line the deterministic version of the problem in this chapter and refer the reader to chap-
ter 3 in Talluri and van Ryzin (2004) for a discussion on the robustness and limitations 
of bid price controls.
To illustrate the capacity-based revenue management problem as a linear program, 
assume that the Hyatt hotel segments its customers into n distinct segments. Let r
i repre-
sent the rate paid by a customer from segment i(i = 1,…, n). Let direpresent the forecasted 
Room request
arrives from
customer
segment i
Demand for
segment i is
recorded
Update
forecast for
segment i
Customer is awarded
a room and capacity
is reduced by 1
No
Yes
Value for
segment i
> current
bid price
Customer’s
room
request is
denied
Figure 4.4 Flowchart of Bid Price Revenue Management Logic

---

## Page 105

94  Capacity-Based Revenue Management
total demand for rooms from customers in segment i . The decision variable is  Xi, the 
number of rooms to allocate to customers in segment  i. Consider a 15-room hotel that 
offers three rates— r1 = $300, r 2 = $200, r3 = $100—for three distinct segments . The 
demand for each segment is d1 = 10, d2 = 10, d3 = 10 such that the cumulative forecasted 
demand exceeds the total capacity. The revenue management problem faced by the hotel 
is to decide how many rooms to allocate to each class in order to maximize the expected 
total revenue. The linear programming formulation of this problem is:
max e
. . , ,...,
Total venue r X
st X d i
iii
n
ii
 
              
R =
≤=
=∑ 1
1 n n
Xi n
X Capaci
i
ii
n
                   
         
≥=
≤=∑
01
1
, ,...,
tty
Solving the optimization problem above results in an optimal solution of X1 = 10, X2 = 5, 
X3 = 0; that is, save ten rooms for segment one customers, five rooms for segment two 
customers and do not sell any rooms to the segment three customers . The formulation 
of the linear program in Excel is shown in Figure 4.5. The problem can be solved using 
Excel’s solver function (solver is typically not included in a standard installation of Excel 
and must be installed as an add-in).
The solution to the Hyatt’s problem is straightforward and you could probably have 
guessed it without the need of solving a linear program. In practice, however, the size of 
network revenue management problems and the number of decision variables are mas-
sive and require advanced optimization techniques just to reduce solution times down to 
a few hours. To understand why, imagine all the possible original origins for a passenger 
on a Delta flight from Atlanta to New York. Since Atlanta is a major hub of Delta, that 
Figure 4.5 Linear Programming Formulation of Revenue Management Problem in Excel.
Decision Variables Capacity 15
X1 10 Forecast Segment 1 10
X2 5 Forecast Segment 2 10
X3 0 Forecast Segment 3 10
Objective Function 4000 Revenue Segment 1 $300.00
Revenue Segment 2 $200.00
Revenue Segment 3 $100.00
Constraints
X1 <= Demand Segment 1 10 <= 10
X2 <= Demand Segment 2 5 <= 10
X3 <= Demand Segment 3 0 <= 10
Tot Cap Used <= Tot Cap Avail 15 <= 15

---

## Page 106

Capacity-Based Revenue Management  95
passenger could have originated at any of the other airports that Delta flies out of, and 
each of these flights has their own set of fare classes.
Even after solving the Hyatt’s problem directly, you still do not have an estimate of the 
opportunity cost of selling one additional room (i.e., a bid price). Recall that for network 
revenue management problems, the goal is to establish a bid price for each individual 
resource so that a request that involves multiple resources can be priced by adding up 
the corresponding bid prices. A major benefit of the linear programming formulation is 
that, in addition to being able to the directly solve for each decision variable, the solution 
also provides something called a shadow price for each constraint. The shadow price 
provides the value of increasing the right-hand side of the constraint by one additional 
unit. For the capacity constraint, this is exactly what we need to estimate a bid price for 
that resource. When using the solver feature in Excel, the shadow prices are provided in 
the sensitivity report. The sensitivity report for the Hyatt’s problem is shown in Figure 
4.6, which shows that when there are 15 rooms remaining then the shadow price for a 
one room is $200. Using the shadow price as a bid price results in a decision rule of only 
allowing room requests that provide a rate of at least $200.
Resolving the problem with an adjusted capacity of ten rooms results in the solution 
and sensitivity report shown in Figure 4.7. Notice that the shadow price of the capacity 
constraint changes to $300, such that the decision rule changes to only accept customers 
willing to pay room rates of $300. Recall that in practice, these calculations take place 
in the background and most systems will only display products with prices greater than 
the shadow price (bid price). In addition, as sales occur over time, the linear program is 
resolved after each sale and a new shadow price is determined.
A major drawback of bid prices is that they provide only marginal guidance—that is, 
a bid price only tells you whether or not you should accept a request for a single unit of 
capacity. Thus, the bid price does not give a definitive answer to the question of whether 
or not you should accept a booking request for more than one units of capacity (i.e., 
two or more seats or rooms). Despite these concerns, bid prices are frequently used in 
Figure 4.6 Solution Report to the Linear Programming Formulation.
Name Final 
Value
Reduced 
Cost
Objective 
Coefficient
Allowable 
Increase
Allowable 
Decrease
X1 10    0 300 1E+100 100
X2  5    0 200 100 100
X3  0 100 100 100 1E+100
Constraints
Name Final 
Value
Shadow 
Price
Constraint 
R.H. Side
Allowable 
Increase
Allowable 
Decrease
X1 <= Demand Segment 1 10 100 10 5  5
X2 <= Demand Segment 2  5   0 10 1E+100  5
X3 <= Demand Segment 3  0   0 10 1E+100 10
Tot Cap Used <= Tot Cap Avail 15 200 15 5  5

---

## Page 107

96  Capacity-Based Revenue Management
practice because they provide a reasonable estimate of the opportunity cost of selling 
one additional unit of a resource. For this reason, they are commonly used in network 
revenue management problems (managing the sale of products consisting of more than 
one resource).
SUMMARY
The logic behind capacity-based revenue management is very similar to the logic behind 
any capacity allocation decision under uncertain demand. We began this chapter with 
a review of how safety stocks are determined in supply chain settings. When there is 
demand uncertainty and the cost of being under demand is not equal to the price of 
being over demand, it is rarely optimal to set an inventory level equal to the forecast. This 
same logic applies to capacity-based revenue management when higher value customers 
arrive closer to the date of consumption than the lower value customers. Capacity-based 
revenue management is the science of how much capacity to reserve for the later arriving 
but higher value customers. Just as with the safety stock example, when there is uncer-
tainty in the demand of the higher value customers, it is frequently optimal to reserve 
some amount of capacity other than the forecast of the higher value customer demand. 
The exact amount of capacity (or safety stock) to reserve (or stock) depends on the ratio 
of the cost of reserving too little versus the cost of reserving too much. This ratio is called 
the newsvendor model.
For most firms, the number of customer segments is typically much larger than two. 
Thus, the simple newsvendor model is insufficient for determining the right amount of 
capacity to reserve for each segment. In response, we present the two most commonly 
used methods for applying capacity-based revenue management in situations with mul-
tiple segments. The first method is a simple extension of the newsvendor model termed 
EMSR-b. This method is used to calculate nested protection levels, such that all customer 
segments above a certain price point are aggregated together and capacity is reserved 
at the group level. This method tends to work well until the revenue management 
Figure 4.7 Solution Report After Total Capacity is Set to Ten Rooms.
Name Final 
Value
Reduced 
Cost
Objective 
Coefficient
Allowable 
Increase
Allowable 
Decrease
X1 10    0 300 1E+100 100
X2  0 100 200 100 1E+100
X3  0 200 100 100 1E+100
Constraints
Name Final 
Value
Shadow 
Price
Constraint 
R.H. Side
Allowable
Increase
Allowable 
Decrease
X1 <= Demand Segment 1 10   0 10 1E+100  0
X2 <= Demand Segment 2  0   0 10 1E+100 10
X3 <= Demand Segment 3  0   0 10 1E+100 10
Tot Cap Used <= Tot Cap Avail 10 300 10 0 10

---

## Page 108

Capacity-Based Revenue Management  97
problem involves network effects, such as the hub-and-spoke system of the large air-
lines. In such cases, firms have simplified the problem by assuming away the uncertainty 
around the forecasts and using linear programming methods to solve for the optimal 
solution. Rather than solve for the capacity of each segment directly, however, it is more 
common for a firm to use the shadow price of the linear program solution as a bid 
price. This bid price is used to remove the available capacity for any product whose pre-
established price is below this amount.
REFERENCES
Belobaba, P. P. (1987). Air travel demand and airline seat inventory management. PhD thesis, Flight Transporta-
tion Laboratory, MIT, Cambridge, MA.
Belobaba, P. P. (1989). Application of probabilistic decision model to airline seat inventory control. Operations 
Research, 37(2), 183–198.
Talluri, K.T. & van Ryzin, G. J. (2004) The theory and practice of revenue management. New York, NY: Springer.

---

## Page 109

5
UNCONSTRAINING
INTRODUCTION
Every organization that sells a physical product faces out-of-stock events. Airlines and 
hotels, for example, deliberately ration the capacity made available to low-fare custom-
ers to protect capacity for the more profitable, high-fare customers. Oftentimes, how-
ever, the capacity protected for these customers is insufficient to serve all those who 
would like and could afford the service. Hence, a portion of willing-to-buy customers 
are frequently turned down a service due to lack of available capacity. While retailers do 
not intentionally allocate their merchandise, they too face stock-out situations whenever 
demand exceeds their forecasted demand plus their safety stock. Consider, for example, 
what happens when the Sparkling Mint, Optic White Colgate toothpaste at a Wal-Mart 
supercenter runs out of stock. While some customers who would otherwise purchase the 
product and counted on it being available in the store will substitute for another product 
type or brand, others will leave disappointed and most likely purchase their preferred 
product at another store. The examples above, arguably different in regard to how out-
of-stocks form and manifest, do share some important similarities. First, stock-outs (or, 
sell-outs) typically lead to lost sales which erode the already thin margins in place at 
many organizations. Second, unless controlled for, the out-of-stock/sell-out events typi-
cally downgrade the performance of the systems that iteratively base current/future deci-
sions on historical data. In this chapter, we focus on the latter of these points and discuss 
how out-of-stock/sell-out events are accounted for in various industry settings.
UNCONSTRAINING: IS IT REALLY NEEDED?
To better understand what unconstraining is and why it is needed, consider the follow-
ing hypothetical example, which is intended to be representative of how some small 
hotels operate. The Royal Hotel in Groningen, the Netherlands, sells the same type of 
room at two different price points. The nightly rate of €150 (or, about $195) targets tour-
ists and university students who are believed to be price conscious and usually plan their 
98

---

## Page 110

Unconstraining  99
trips in advance. This rate is available up to 14 days prior to the actual check-in date but 
can be closed earlier based on how fast the demand for low-fare rooms materializes. The 
nightly rate of €225 (or, about $290) targets business travelers who visit businesses in 
areas around the city and have shown to be less price sensitive than the tourists. Contin-
gent on the hotel not being sold out, this rate is available until the midnight of the actual 
check-in date. The typical length of stay at the Royal Hotel is one night. Similarly, most 
bookings are single-room bookings.
Based on her experience, the hotel revenue manager saves parts of her room capacity 
to meet the expected demand of business travelers. For example, for Tuesday check-in 
dates, she protects ten of her 30 rooms specifically for this type of customers. Most of the 
time, if not always, the remaining unprotected capacity is filled with tourists or univer-
sity students who enjoy the lower room rates. Figure 5.1 shows the booking curves for 
the business travelers for three consecutive Tuesday check-in dates, which chart how on-
hand business bookings evolved in the two weeks prior to the check-in. The first two of 
these booking curves do not show anything out of the ordinary as the revenue manager 
appears to have protected enough rooms such that all business demand was served. In 
these two cases, the rooms sold at the end of the booking horizon (i.e., seven and ten for 
booking curves 1 and 2, respectively) reflect the real demand for the business customer 
rate. In contrast, the third of the booking curves is flat from six days before the check-
in date until the day of arrival. This means that the ten business-rate rooms reported as 
booked for the third Tuesday are right censored. In other words, the on-hand bookings 
are a constrained reflection of the true demand for the business rate customers. Had the 
protection level been set at a higher value, the hotel could have probably sold more than 
ten rooms for that Tuesday at the higher rate of €225.0 (this implicitly means that the 
block of 20 unprotected rooms sold-out at the lower rate of €150.0). Building on this 
admittedly simple example, we define demand unconstraining as the task intended to 
infer the parameters of the true demand distribution from the historical sales data col-
lected over previous sale opportunities.
In the context of the Royal Hotel, why is unconstraining the sales data important? 
As discussed in Chapter 4, the protection level of ten rooms is computed based on the 
parameters of the business-rate customer demand distribution. Intuitively, if the con-
strained data are used to infer these parameters, their values would be negatively biased. 
For the limited example shown in Figure 5.1, for instance, if without censoring the 
business booking curve 3 showed 13 rooms sold, the expected value of the true busi-
ness demand distribution would be ten rooms. In the presence of demand censoring, 
however, the expected value turns out to only be nine rooms. Hence, the protection 
level computed on constrained data is underestimated and the likelihood of not having 
enough capacity reserved for the high-fare customers will increase. In the likely case that 
the parameters of the demand distribution are revised periodically, the iterative update 
process may actually make matters worse by recommending monotonically decreasing 
protection levels that lead to a spiral down phenomenon, resulting in a downward trend 
in the hotel’s revenue performance (Cooper, Homem-de-Mello, & Kleywegt, 2006).
Much of the work on analyzing and preventing the problems that may arise from 
making strategic, operational, or tactical business decisions using censored data has been 
done in settings specific to airline and hotel industries (see the review paper by Guo, 
Xiao, & Li, 2012, pp. 7–8, and the substantive list of references therein). Published work 
outside of these focus areas targets problems specific to the retail (Agrawal & Smith, 1996;

---

## Page 111

100  Unconstraining
Kök & Fisher, 2007; Lariviere & Porteus, 1999; Lau & Lau, 1996; Tan & Karabati, 2004) 
or vending (Anupindi, Dada, & Gupta, 1998; Conlon & Mortimer, 2008) industries. In 
what follows, we build on our retail experience and provide a few more subtle examples 
where unconstraining the demand may help organizations make better decisions.
To reiterate just how important unconstraining the demand may be, we discuss next 
the case of an organization which is one of the market leaders in online retailing in the 
Netherlands. This online retailer sells a wide assortment of goods in both hardlines (e.g., 
home furnishings and electronics) and softlines (e.g., apparel and footwear) product 
groups. It assorts about 100,000 stock-keeping units, has more than 1.5 million custom-
ers, and makes some 7 million parcel shipments per year. In an attempt to expand its 
hardlines product range, improve inventory turnover and maintain or lower the work-
ing capital, the company moved recently from weekly to daily inventory replenishment, 
an initiative that fueled significant growth in some test product categories. As a result 
of this change, the inventory restocking decisions are driven primarily by the product 
demand and reflective of the shift from a push to a pull business model. In the new 
environment, supply chain planners of hard goods are provided with reliable demand 
information which helps them make better strategic, operational, and tactical decisions.
Due to the inherent buying/selling differences between hard and soft goods, this retailer 
still manages its softlines product groups in a conventional way. For example, for each 
season (e.g., Winter 2012) and product category (e.g., women shoes), a strategic plan is 
devised to strengthen the retailer’s market position. Following the guiding principles of 
this strategic plan, the supply chain planners and merchandise buyers decide on which 
products to assort across a range of price intervals (e.g., €20–€30, €30–€40, €40–€50), 
product classes (e.g., women boots, sandals or high heels), or, brands (e.g., designer or 
private brands/labels). Once the collection for the season is finalized, the merchandise 
is ordered from suppliers. Due to lead times as long as nine months, a single product 
Figure 5.1 Royal Hotel Business Booking Curves.
14
4
2
0
8
6
10 Protection Level 10 rooms
11 1012 13 9 6587 432 10
Days Before Check-In Date
On-Hand Bookings (Booked Rooms)
Business Booking Curve 2Business Booking Curve 1
Business Booking Curve 3

---

## Page 112

Unconstraining  101
purchase order is typically released, making it difficult for a product to be replenished 
multiple times throughout the season. Upon receipt of the ordered merchandise, the 
products are made available online and sell until the end of the season or for as long as 
the supply lasts.
Unlike the hardlines product groups which are managed in a pull system where cus-
tomer orders drive the supply chain, the soft goods are managed in a traditional push 
system where inventory is stocked in anticipation of the demand materialization. More 
specifically, the supply chain planners and buyers at this retailer forecast the customer 
demand for a product, purchase the product based on this forecast (typically using the 
point forecasts), push the product onto the online channel, and then anxiously wait to 
see whether or not the demand for the product materializes. If it does not and too much 
product is ordered, the retailer marks down the price to clear the excess inventory at 
the end of the selling season. If it does but at too high a rate, the retailer ends up losing 
margin and goodwill as there is insufficient supply to serve all latent demand. To make 
sensible purchasing decisions, planners and buyers use judgmental, consensus-seeking 
forecasts that reflect the planned merchandise mix and the performance targets for the 
collection. Both of these latter planning attributes are typically derived from high-level, 
product category forecasts driven by historical sales.
The fundamental problem with such an approach to planning is that a sequence of 
interrelated decisions are made based on sales data which may be heavily constrained due 
to frequent product out-of-stocks. To get a sense of just how severe this phenomenon 
may be, we monitored the online product availability at this retailer using a Mozenda 
custom-built web agent (Mozenda, 2012). We used a web crawler because while the 
retailer provides its customers with real-time product availability, it does not use this 
information to grow product availability histories. Within the product category women 
shoes, we targeted the boots product class and collected price and product availability 
every six hours (i.e., 3:00 a.m., 9:00 a.m., 3:00 p.m., 9:00 p.m.) during a time window that 
spanned the period from February 24, 2012 until March 2, 2012. We focused only on the 
products displayed on the first product page for the class and used the default values for 
all display/filter options. In doing so, we intended to recreate the shopping experience 
of a customer who is not necessarily fond of our retailer and leaves to shop somewhere 
else easily.
In total, we tracked the availability of 14 different boot styles (e.g., ClockHouse boots), 
25 style/color articles (e.g., dark blue or sea green ClockHouse boots) and 169 style/
color/size stock-keeping units (e.g., dark blue ClockHouse boots in the European size 
37). None of the style/color articles considered were marked down or sold at a promo-
tional price. Of these articles, only 20 were displayed at any one point in time on the 
first product page for the boots product class—this is a technical design option that the 
retailer uses consistently across many of its product classes. Typically, if a style/color 
article showed on the first page, all other color variants of the same style showed on this 
page too. Style/color articles for which at least one size was continuously available stayed 
displayed throughout the entire study period. Style/color articles that experienced an 
out-of-stock for all sizes did not show on the first product page for as long as the stock-
out lasted. An out-of-stock situation was sometimes ended when customers returned 
unfit and unbroken merchandise that was put back in stock.
Customers leaving the reference landing product page for the boots product class to 
inspect a product display page could have considered for purchasing, on average, 136

---

## Page 113

102  Unconstraining
different style/color/size stock-keeping units. At any point in time, on average, 39 (or, 
28.7%) of these stock-keeping units were out-of-stock in that the corresponding sizes 
were unavailable. The highest size-level out-of-stock rates were experienced during the 
weekend of February 25, 2012 when as many as 50 (or, 36.8%) of the shown style/color/
size items were unavailable. In total, there were 12 instances when style/color articles 
temporarily left the first product page for the class due to complete size out-of-stocks. 
These article out-of-stock events lasted anywhere from 12 hours to 6 days. To make the 
exposition more concrete, we show in Figure 5.2 how the product availability for three 
color variants of the same style progressed in time. Throughout the study period, most of 
these style/color/size items experienced out-of-stocks. However, when the product avail-
ability resumed due to the merchandise being returned, the resulting inventory typically 
depleted quickly. For example, in 4 of the 8 such instances apparent in Figure 5.2, the 
returned items sold in less than 12 hours. At the most, it took these items 60 hours to sell, 
which is still reasonable since multiple units of the same item could have been returned 
and may have reentered the selling cycle.
The obvious yet oftentimes overlooked lesson one can learn from Figure 5.2 is that 
unless the product is available, it cannot be sold. Hence, all periods during which the 
product is unavailable essentially impede the product from reaching its full sales poten-
tial. Yet, for the history-based planning to be unbiased and effective, assortment and 
buying decisions that reflect the latent sales potential of the products in one’s portfolio 
are needed. Unconstraining the demand then comes just as a natural step of an improved 
planning process. While we acknowledge that factors such as the product placement or 
the availability of close item substitutes complicate further an already complex uncon-
straining task, we also believe that the gains organizations may enjoy from properly 
executing this task are worth the effort.
Style Size
Feb  24, 2012
3:00 am
Mar  3, 2012
3:00 am
36 1
37 2
38
39
40 3
41 4
36
37 5
38
39 6
40 7
41
36
37
38
39 8
40
41
Legend:
Color 3
Time
Color 1
Style/Color OOS
Color 2
Style/Color OOS
Style/Color/Size Available Style/Color/Size Unavailable Style/Color Unavailable
Figure 5.2 Product Availability Progression in an Online Environment.

---

## Page 114

Unconstraining  103
Building on the issues we uncovered at the Dutch online retailer, we focus next 
on some of the current practices in place at many fashion companies that design and 
sell clothes and accessories (for a comprehensive review of how the fashion industry 
operates, see Åžen, 2008). These organizations prepare for the next season(s) by going 
through an involved merchandise planning process. Often assembled based on a finan-
cial plan reflective of the overall corporate strategy, merchandise planning specifies when 
in the season new collections or fashion styles are to be introduced and where and in 
what quantities they are to be made available. Since the past performance of individual 
style and seasonal goods is typically not indicative of their future performance (popular 
press quotes such as “in fashion apparel, there is nothing as boring as last season’s hot 
sellers” (Fisher & Raman, 2010, p. 31) are very common in this industry), fashion com-
panies devise their merchandise plans based on aggregate forecasts. For example, it is 
not unusual for the past sales of all style/color/size items that belonged to a certain class 
or category of products (e.g., men casual pants) to be combined to compute the class-
level forecasts. These aggregate forecasts are then used to do the entire pre-season plan-
ning including product, store, range, and assortment planning. The pre-season planning 
concludes with a fabric production plan based on which a product purchase order is 
released. At this stage, a high-level size scale is used to distribute the required quantities 
of all style/color items across the relevant item sizes. Once the merchandise is received 
and stored in distribution centers or warehouses, the in-season planning starts. This 
step determines the allocation of the merchandise to the stores as well as the timely store 
replenishment. To the extent possible, stores receive their product shares based on their 
individual store size scales.
Within the general framework sketched above, let’s consider the particular case of a 
major fashion company that sells its products worldwide through physical stores, virtual 
stores, and order catalogs (Osika, 2012). For confidentiality reasons, we cannot disclose 
the identity of this organization but its operations resemble well how most of the similar 
players compete in the marketplace. For ease of exposition, we call this organization Just 
for You, or, in short, JfY. During the pre-season planning, JfY places a purchase order 
for the needed style/color items based on country/class size scales. These size scales are 
computed based on the first four weeks of the relevant historical sales of all style/color 
items belonging to a given country/class pair. For example, the fall/winter pre-season 
planning for a country/class pair (e.g., the Netherlands/men casual pants) uses the first 
four weeks of the sales for all style/color items reported for this pair in the previous 
fall/winter season. The first four weeks of sales are believed, in this case, to reflect the 
full-price true size scales at JfY as the likelihood of stock-outs is considered negligible 
and markdowns are offered, if needed, only at eight weeks after the style/color items 
are introduced. Upon the receipt of the ordered merchandise and based on the product 
availability, the style/color items are allocated to stores following the individual store 
class size scales. These latter size scales are computed based on the full-price historical 
sales performance of all items belonging to a class. For example, for the JfY store located 
in midtown Groningen, the size scale for men casual pants for the fall/winter season is 
computed based on the full-price sales of all items belonging to the class as reported 
during the previous fall/winter season.
While the merchandise planning process described above represents the norm in this 
industry, it is clearly not an error-free approach. In particular, the way the size scales 
are put together to either order the merchandise or distribute it to the stores is subject

---

## Page 115

104  Unconstraining
to systematic biases. We illustrate this problem in Figure 5.3 where we show the evolu-
tion of the out-of-stock rates for 72 style/color/size stock-keeping units (e.g., black JfY 
women casual city blazer in size 42) sampled from 12 style/color items (e.g., black JfY 
women casual city blazer) in six different product classes (e.g., women casual blazers). 
These items are either high-volume or high-price products whose unavailability could 
hurt JfY’s profit margins. We follow the out-of-stock performance of all 72 stock-keep-
ing units across five family stores that JfY operates in the Netherlands. The family stores 
differentiate from other types of stores (e.g., women stores) in that they sell the full prod-
uct assortment. As it becomes apparent from Figure 5.3, across all five stores, on average, 
about 19 (or, 26.6%) and 32 (or, 43.8%) of the 72 stock-keeping units considered are 
out-of-stock by week 4 and 8, respectively. This suggests that the information based on 
which the size scales are put together is right censored due to the product not being avail-
able. Had these stock-keeping units been available throughout the entire selling season 
(or, throughout the full-price part of the selling season), they could have sold probably 
better and the resulting size scales might have been different. To provide the reader with 
a clearer picture of the extent and the cost of the size-level out-of-stocks at JfY, we show 
in panel A of Figure 5.4 the full size range availability across all 12 style/color items sold 
in store 5. Of these items, seven sell in an incomplete size range before week 4 and nine 
before week 8. For example, style/color 12 sells in an incomplete size range as early as 
week 3. For this style/color item, we depict in panel B of Figure 5.4 how the size-level out-
of-stocks form and progress. In this case, by weeks 4 and 8, the small sizes (i.e., sizes 32–
36) and small and medium sizes (i.e., sizes 32–40), respectively, are all out of stock. With 
the large sizes (i.e., sizes 42–44) not being able to sell even at the marked down price, JfY 
effectively lost, in the most optimistic of the scenarios, about €22 (two units, one of each 
available sizes x (unit cost – salvage value)). In the same context, however, had JfY had 
better size scales in place, it most likely would have made, in the most pessimistic of the 
scenarios, a profit of about €106 (two units, initially assigned to the unavailable sizes x 
1
20
0
60
40
80
Country/Class
Size Scales
Store/Class
Size Scales
45326 91 078 11 12 13 14 15 16
Weeks After Introduction
Percent OOS Items (%)
Store 2 Store 3Store 1
Store 4 Store 5 Store Average
Figure 5.3 Out-of-Stock Rates for the Sampled Style/Color/Size Items.

---

## Page 116

Unconstraining  105
(full price – unit cost)). To put these figures in perspective, go through a mental exercise 
and extrapolate even fractions of these figures to the full product and store portfolios of 
a typical fashion company. Along the same lines, we also refer to the findings of a U.S. 
sportswear and footwear retailer with global operations, which show that in Europe, 
about 18% of those who visit the retailer’s stores and do not purchase, do so because the 
requested/needed sizes are unavailable (Hofman, 2012). While admittedly many other 
factors influence the in-store product performance, a blindsided planning process which 
draws from censored sales data cannot but lead to unfit and costly decisions that are typi-
cally difficult, if not impossible, to revert. As an analogy to the spiral-down phenomenon 
Figure 5.4 In-Store Item Availability Measures.
1 2 3
Style/Color 2
Style/Color 1
Style/Color 3
Style/Color 4
Style/Color 5
Style/Color 6
Style/Color 7
Style/Color 8
Style/Color 9
Style/Color 10
Style/Color 11
Style/Color 12
4
5 6
(A) Full Size Range Availability in Store 5
7 8 10 11 129 161513 14
Weeks After Introduction
1 0 2 3
42
44
40
38
36
34
32
4 5 6
(B) Size Availability of Style/Color 12 in Store 5
7 8 10 11 129 161513 14
Weeks After Introduction
Style/Color 12 in
Size
In Store Availability

---

## Page 117

106  Unconstraining
discussed in the context of the travel industry, such an approach to planning perpetuates 
built-up poor performance since the distorted size profiles feed next seasons’ plans and 
purchases.
ESTIMATION OF DEMAND DISTRIBUTIONS OF 
CENSORED SINGLE-PERIOD ITEMS
In Chapter 4, we referred to the example of Walton’s bagel shop and discussed strategies 
related to the amount of bagels the store needed to order to maximize its expected prof-
its. The discussion therein relied heavily on a demand distribution which we assumed 
was known at the time the optimal order quantity was derived. In practice, however, 
the estimation of the demand distribution for a single-period item such as the bagels is 
all but a trivial task. For example, even in the presence of the right order quantity, the 
inherent variability in demand may lead to stock-outs which could censor, sometimes 
severely, the demand data. Similarly, things outside of the firm’s control can impact 
the quality of its demand data streams. A supplier that faces a product shortage due to, 
for example, extreme weather conditions or a strike, and is forced to adjust its shipping 
quantities effectively contributes to the unexpected out-of-stocks at the bagel store. In 
this case too, the demand data at Walton’s is corrupted and reflects a partial materializa-
tion of the true demand for a product.
Other more extreme examples come from grocery retailers such as Jumbo and Albert 
Heijn, two supermarket chains with a significant footprint in the Netherlands (Jumbo 
and Albert Heijn) and other European markets (Albert Heijn). In the Netherlands, for 
instance, each of the stores affiliated with these retailers is responsible for the production 
of the daily supply of fresh breads. This means that most activities around the making of 
the bread—baking, cooling, slicing, and packaging—happen in the stores. Due to lim-
ited peak-hour production capacity and in the absence of a coherent production plan, 
most of the assortment of fresh breads is out-of-stock by 6:00 p.m. each day. During this 
same time period, however, the production capacity is typically idle so it does not appear 
that the out-of-stocks are due to the demand being consistently greater than the capac-
ity. The corresponding low service level suggests, in this case at least, that the observed 
sales data represent just a portion of the entire demand distribution. Next, we discuss 
an appealing method for inferring the demand distribution for single-period items that 
experience frequent out-of-stocks. Our exposition follows closely the arguments put for-
ward by Lau & Lau (1996).
To start the discussion, consider the hypothetical daily sales of the bread Pain de 
Boulogne at an Albert Heijn store which we depict in Table 5.1. Of the total of 20 daily 
sales values, 13 (65%) are constrained, in that the product ran out of stock at some point 
in time during the day. By contemplating these sales figures, it is obvious that in many 
cases the daily product demand exceeded 40 units. Yet, since no actual observations in 
this domain exist, we cannot infer too much about the demand past this point. Up to 
the maximum of the unconstrained sales values (i.e., 39 units), however, we can use 
something called the Product-Limit estimation technique to form an understanding of 
what the demand distribution function on this limited domain looks like. The Product-
Limit method, a nonparametric estimation technique influential in reliability and life 
data analysis, was introduced by Kaplan & Meier (1958) and popularized, among others, 
by Lawless (2003), Nelson (2004) and Crowder, Kimber, Smith & Sweeting (1991).

---

## Page 118

Unconstraining  107
The Product-Limit estimation technique requires us to first sort in ascending order 
the unique actual demand levels observed (i.e., the unique sales data values shown in 
panel A of Table 5.1). We call this distinct and ordered demand value vector x j to dif-
ferentiate it from the raw demand data vector St = Dt. For our problem, xj is a four-ele-
ment vector, which consists of 20, 23, 31, and 39. Next, for each of the x js, we estimate 
the conditional probability p j that the demand is greater than x j given that it is greater 
than xj–1. If nj provides the count of all daily sales, constrained or not, with values greater 
than or equal to x j and δj provides the count of only the unconstrained daily sales that 
equal xj, then pj is simply the ratio of (nj –δj) and nj, or, pj = (nj –δj)/nj. By noting that at 
x0 = 0 the probability of the demand being greater than 0 is effectively 1, we can estimate 
the unconditional probability P (xj) that the demand is greater than xj using the product 
of the pk’s for all k indices such that k ≤ j. Hence, the cumulative distribution function 
F(xj) evaluated at xj, or, equivalently, the probability of the demand being smaller than or 
equal to xj, can be computed as 1 – P (xj). We illustrate how the Product-Limit method 
applies to the Pain de Boulogne data in Table 5.2. The last column in this table makes it 
obvious that the available data can help us infer about 37% of the cumulative distribu-
tion function for the product’s demand. While this finding represents a sound starting 
point, by itself it is insufficient to warrant the informative character of any subsequent 
production decisions. Hence, questions such as “How much fresh bread should be baked 
Table 5.1 Daily Sales of Pain de Boulogne at an Albert Heijn Store
(A) Unconstrained Regime (B) Constrained Regime (C) Both Regimes
Day Unconstrained Day Constrained Day Sales S t
t Sales St (St = Dt) t Sales St (St ≤ Dt) t (Combined)
63 1 14 0 14 0
82 0 24 0 24 0
93 1 34 0 34 0
11 23 44 0 44 0
16 39 54 0 54 0
18 39 74 0 63 1
20 31 10 40 74 0
12 39 82 0
13 31 93 1
14 40 10 40
15 40 11 23
17 23 12 39
19 40 13 31
14 40
15 40
16 39
17 23
18 39
19 40
20 31
St – Sales on day t
Dt – Demand on day t
Figures shown in bold and italic represent constrained sales values.

---

## Page 119

108  Unconstraining
today?” cannot be answered with too much confidence. To this end, what can we do to 
infer the rest of the cumulative demand distribution function?
In the absence of any other relevant data, we could attempt to learn the other 63% 
of the demand distribution using subjective probability elicitation techniques (see, e.g., 
Chesley, 1975, 1978; Smith, 2010, chapter 4; Wright, 1988 and the references therein). 
At their core, these techniques require us to subjectively assess the demand distribution 
function based on responses from the management team that either assign (1) prob-
ability values to specific demand points (P-methods), or (2) demand values to particular 
probability fractiles (V-methods). Of these techniques, the fractile method is perhaps the 
most popular among statisticians and psychologists.
This method requires a member of the management team to provide estimates x for 
which the probability of the demand being smaller than or equal to x equals a fractile 
f from a set of predefined fractiles such as 0.01, 0.10, 0.25, 0.50, 0.75, 0.90, and 0.99 
(e.g., What x gives Probability (Demand ≤  x) = 0.50?). For the specific problem of the 
Pain de Boulogne, we could ask a morning shift leader, for example, to provide the xs 
that correspond to the fractiles not covered by the available data (e.g., 0.50, 0.75, 0.90, 
0.99). Such practices may prove to be unreliable, however, as many workers lack a basic 
understanding of fractiles or of how the business operates. Along the same lines, even 
experienced operators could make unfit decisions due to inappropriate expectations that 
build on biased prior experiences (for in-depth details on how the optimism bias affects 
management decisions, see Kahneman & Tversky, 1979; Pezzo, Litman, & Pezzo, 2006). 
To this end, we focus next on some analytical methods of estimating the missing portion 
of a demand distribution.
The advances in the development of retail Point of Sales (PoS) systems witnessed 
in the last decade make it relatively easy for retailers to track their sales and monitor 
their inventory levels at the stock-keeping unit. Since many retailers own or operate 
advanced PoS systems, it is not unreasonable to assume that the daily sales history of 
a product is readily available and accessible at these retailers. The same holds even for 
small retailers since the new generations of cash registers allow for the electronic trans-
fer of the daily sales to other electronic equipment through USB ports or wireless/Blue-
tooth connectivity. Thus, it is reasonable to assume that hourly sales rates of a product 
are available such as those of Pain de Boulogne across 20 historical days shown in Table 
5.3. As it is readily apparent from these figures, out-of-stock events of various durations 
lead to identical daily cumulative sales. For example, daily sales of 40 units are reported 
for days with apparent out-of-stocks of 1 (day 19) and 7 (day 15) hours, respectively. 
Because the duration of out-of-stocks and the full unconstrained sales potential would 
appear to be related, it seems reasonable to account for the time the stock-outs first 
occur.
Table 5.2 Product-Limit Method Applied to the Pain de Boulogne Data
j x j n j δj p j P(x j) F(x j) 
1 20 20 1 0.950 = (20-1)/20 0.950 = 1.000 x 0.950 0.050
2 23 19 1 0.947 = (19-1)/19 0.900 = 0.950 x 0.947 0.100
3 31 17 3 0.824 = (17-3)/17 0.741 = 0.900 x 0.824 0.259
4 39 13 2 0.846 = (13-2)/13 0.627 = 0.741 x 0.846 0.373

---

## Page 120

Unconstraining  109
To compute the sales the retailer would have achieved had it not experienced any out-
of-stock events, and, subsequently, estimate the parameters for the full demand distribu-
tion function, we assume that the hourly sales rates hit observed during the i -th hour of 
day t are proportional to the demand Dt such that the proportionality constant does not 
change much across ts. This assumption implies, for example, that the first hour after 
the store opens sees the same percent of the daily demand irrespective of how small or 
large the daily demand may turn out to be. In grocery retailing, this assumption is usu-
ally reasonable, especially for fast-moving goods. If the demand exhibits an apparent 
day-of-week pattern, a similar analysis can be run for each day of the week. With this 
assumption in place, if we knew the daily demand D
t for a constrained sales day t , we 
could easily estimate the lost hourly sales for the stock-out periods by the product of the 
corresponding proportionality constants and D
t. Unfortunately, Dt is unknown, but the 
proportionality assumption between hit and Dt implies that the ratio between hit and Hit 
(the cumulative sales up to the i -th hour of day t ) is also stable across ts. This in turn 
implies that the average ri of all the hit / Hit ratios across all product histories with uncon-
Table 5.3 Hourly Sales Rates (Units/Hour) of Pain de Boulogne
Day Hourly Interval
12 34567891 0 1 11 21 31 41 51 6
Total
12 4 4 2 4 2 4 1 5 45 3 4 0
23 4 4 5 4 5 4 2 4 5 4 0
31 3 2 2 3 6 4 2 3 334 2 2 4 0
42 3 4 1 4 3 3 1 3 342 3 2 2 4 0
52 5 5 3 5 5 5 2 4 4 4 0
61 3 3 1 3 3 2 1 1 22 2 2 2 2 13 1
7 34 32455 3 2 4 3 2 40
81 2 2 1 1 1 2 1 1 12 1 1 1 1 12 0
91 2 3 2 2 2 2 1 2 22 2 2 3 2 13 1
10 2 6 6 3 4 2 4 2 6 5 40
11 1 2 1 1 2 1 3 1 1 1 2 2 1 1 2 1 23
12 2 3 4 2 2 1 2 2 3 2 3 4 3 3 3 39
13 2 3 2 1 3 2 3 2 2 1 1 2 3 4 31
14 1 4 3 1 2 1 3 2 3 2 4 5 6 3 40
15 3 6 8 4 5 3 5 6 40
16 1 3 1 2 3 3 3 1 2 3 3 4 4 3 2 1 39
17 1 3 2 1 1 1 2 1 2 2 1 2 2 2 23
18 2 3 4 3 2 1 1 2 3 3 1 4 4 3 2 1 39
19 1 4 3 3 1 2 2 3 2 3 2 4 3 4 3 40
20 1 2 3 2 2 2 1 1 1 3 2 3 3 2 2 1 31
Legend:  Out-of-Stock Periods
  Periods Possibly Affected By Out-of-Stocks
Figures shown in bold and italic identify constrained daily sales histories.

---

## Page 121

110  Unconstraining
strained sales for the i-th hour can be used as a representative estimate for the product 
of interest. Applying this logic to our example, the antepenultimate line in Table 5.4 
provides the r
i s for the Pain de Boulogne data. Building on the representativeness of r i, 
if we refer to the estimate of the average of the ratios Hit / Dt as Ri and to the estimate of 
the average of the ratios hit / Dt as Qi, we can derive the Ri s and Qi s recurrently (moving 
backwards) as Ri–1 = Ri – Qi and Qi–1 = ri–1 · Ri–1 where 2 ≤ i ≤ m, Rm = 1, rm = Qm and m is 
the last hourly interval of the day. The second from the last and the last rows in Table 5.4 
provide the R
i s and Qi s for the Pain de Boulogne data.
Continuing our example, for each of the constrained product histories, we can now use 
the Ri's to compute the likely demand the retailer would have seen had it not experienced 
any stock-out events. We illustrate how we can accomplish this task in Table 5.5 where, 
for each of the days t considered, we show the cumulative hourly sales H
it. If we focus on 
the first of these 20 days, we learn that up to the end of the 11th hour the store was open 
that day, the retailer sold a total of 37 units which were not impacted by any inventory 
shortages. Dividing this figure by the corresponding R
i of 0.673, we obtain 54.97 units 
as the unconstrained demand for that day. For convenience, we round up this value to 
55 units. We use a similar approach to compute the unconstrained demand for all con-
strained daily product histories. As an interesting point, you should note that the days 
that ended up with constrained sales of 40 units show unconstrained demand values that 
span a wide interval, with lower and upper bounds at 41 and 78 units, respectively.
The unconstrained demand values reported in the last column of Table 5.5 can be 
used to derive the cumulative demand distribution function past the interval covered by 
the Product-Limit technique. We show how this works in Table 5.6. Since the empirical 
data provides trustworthy information, we do not revise the estimates computed using 
the Product-Limit technique. Hence, we disregard all unconstrained demand values x
j 
smaller than or equal to 39 units (i.e., the unconstrained demand values of 26 and 33 
computed for days 17 and 13, respectively). For all other values, sorted in ascending 
order, we compute F(x
j), the probability that the demand is smaller than or equal to  xj, 
directly from the available data. For example, for the x j of 40 units (which incidentally 
characterizes day 12), F(xj) is 0.50 as there are ten demand values among the total of 20 
that are smaller than or equal to 40.
The cumulative demand distribution function depicted in Table 5.6 relies on a 
discrete set of 14 pairs (x j, F(xj)). Since many production or inventory purchasing 
decisions require the demand values that correspond to particular probabilities  p, we 
estimate a continuous inverse cumulative demand distribution function Fc
–1 (p) that rep-
resents the pairs (xj, F(xj)) well. Such a function can be computed directly by fitting an 
inverse cumulative distribution curve to the points (F(xj), xj,). For example, the Tocher’s 
general inverse cumulative distribution function (Tocher, 1963) is estimated using this 
approach. Alternatively, we can first compute a cumulative distribution function F
c(x) 
by fitting it to the pairs (x j, F(xj)) and then express F c
–1(p) analytically based on F c(x)’s 
distributional parameters. The inverse normal or Gumbel cumulative distribution func-
tions are examples that would fit this approach. For completeness, we briefly discuss 
next how the Tocher’s general inverse and the inverse Gumbel cumulative distribution 
functions can be estimated.
Given a set of data points (F(x
j), xj,) = (pj, Dj), we write the Tocher’s inverse cumula-
tive distribution function as:

---

## Page 122

Table 5.4 Hourly Sales Rates to Cumulative Sales Ratios
Day Hourly Interval i 
t 1 2 3 4 5 6 7 8 9 10 11 12 13 14 15 16
1 1.000 0.667 0.400 0.167 0.250 0.111 0.182 0.043 0.179 0.125 0.135 C C C C C
2 1.000 0.571 0.364 0.313 0.200 0.200 0.138 0.065 0.14 C C C C C C C
3 1.000 0.750 0.333 0.250 0.273 0.353 0.190 0.087 0.115 0.103 0.094 0.111 0.053 C C C
4 1.000 0.600 0.444 0.100 0.286 0.176 0.150 0.048 0.125 0.111 0.129 0.061 0.083 0.053 C C
5 1.000 0.714 0.417 0.200 0.250 0.200 0.167 0.063 0.111 C C C C C C C
6 1.000 0.750 0.429 0.125 0.273 0.214 0.125 0.059 0.056 0.100 0.091 0.083 0.077 0.071 0.067 0.032
7 1.000 0.571 0.300 0.167 0.250 0.238 0.192 0.103 0.065 0.114 0.079 C C C C C
8 1.000 0.667 0.400 0.167 0.143 0.125 0.200 0.091 0.083 0.077 0.133 0.063 0.059 0.056 0.053 0.050
9 1.000 0.667 0.500 0.250 0.200 0.167 0.143 0.067 0.118 0.105 0.095 0.087 0.080 0.107 0.067 0.032
10 1.000 0.750 0.429 0.176 0.190 0.087 0.148 0.069 0.171 C C C C C C C
11 1.000 0.667 0.250 0.200 0.286 0.125 0.273 0.083 0.077 0.071 0.125 0.111 0.053 0.050 0.091 0.043
12 1.000 0.600 0.444 0.182 0.154 0.071 0.125 0.111 0.143 0.087 0.115 0.133 0.091 0.083 C C
13 1.000 0.600 0.286 0.125 0.273 0.154 0.188 0.111 0.100 0.048 0.045 0.083 0.111 C C C
14 1.000 0.800 0.375 0.111 0.182 0.083 0.200 0.118 0.150 0.091 0.154 0.161 0.162 C C C
15 1.000 0.667 0.471 0.190 0.192 0.103 0.147 C C C C C C C C C
16 1.000 0.750 0.200 0.286 0.300 0.231 0.188 0.059 0.105 0.136 0.120 0.138 0.121 0.083 0.053 0.026
17 1.000 0.750 0.333 0.143 0.125 0.111 0.182 0.083 0.143 0.125 0.059 0.105 0.095 C C C
18 1.000 0.600 0.444 0.250 0.143 0.067 0.063 0.111 0.143 0.125 0.040 0.138 0.121 0.083 0.053 0.026
19 1.000 0.800 0.375 0.273 0.083 0.143 0.125 0.158 0.095 0.125 0.077 0.133 0.091 0.108 C C
20 1.000 0.667 0.500 0.250 0.200 0.167 0.077 0.071 0.067 0.167 0.100 0.130 0.115 0.071 0.067 0.032
r
i=A[hit/Hit] 1.000 0.680 0.385 0.196 0.213 0.156 0.160 0.084 0.114 0.107 0.099 0.110 0.094 0.077 0.064 0.035
Ri=A[Hit/Dt] 0.039 0.121 0.197 0.245 0.311 0.369 0.439 0.480 0.541 0.606 0.673 0.756 0.834 0.904 0.965 1.000
Qi=A[hit/Dt] 0.039 0.082 0.076 0.048 0.066 0.058 0.070 0.040 0.062 0.065 0.067 0.083 0.078 0.069 0.062 0.035
Figures shown in bold and italic identify constrained daily sales histories. A[.] is the average operator.
C identifies both partial or full stock-out periods. These periods do not enter the calculation of the estimate of the average ratio ri.
The ri of 0.035 for the 16th hourly interval is the average of the 7 unconstrained hit/Hit ratios observed at i =16.

---

## Page 123

Table 5.5 Cumulative Hourly Sales and Unconstrained Demand
Hourly Interval                         Un constrained
Day
12 3 4 5 6 7 8 9 1 01 1 1 21 31 41 5 1 6 Demand
1 2 6 10 12 16 18 22 23 28 32 37 40 40 40 40 40 54.97 55
2 3 7 11 16 20 25 29 31 35 40 40 40 40 40 40 40 64.66 65
3 1 4 6 8 11 17 21 23 26 29 32 36 38 40 40 40 45.54 46
4 2 5 9 10 14 17 20 21 24 27 31 33 36 38 40 40 42.05 43
5 2 7 12 15 20 25 30 32 36 40 40 40 40 40 40 40 66.51 67
61 4 7 8 1 1 1 4 1 6 1 7 1 8 2 0 2 2 2 4 2 6 2 8 3 0 3 1 3 1
7 3 7 10 12 16 21 26 29 31 35 38 40 40 40 40 40 56.46 57
81 3 5 6 7 8 1 0 1 1 1 2 1 3 1 5 1 6 1 7 1 8 1 9 2 0 2 0
91 3 6 8 1 0 1 2 1 4 1 5 1 7 1 9 2 1 2 3 2 5 2 8 3 0 3 1 3 1
10 2 8 14 17 21 23 27 29 35 40 40 40 40 40 40 40 64.66 65
11 1 3 4 5 7 8 11 12 13 14 16 18 19 20 22 23 23
12 2 5 9 11 13 14 16 18 21 23 26 30 33 36 39 39 39.84 40
13 2 5 7 8 11 13 16 18 20 21 22 24 27 31 31 31 32.36 33
14 1 5 8 9 11 12 15 17 20 22 26 31 37 40 40 40 44.35 45
15 3 9 17 21 26 29 34 40 40 40 40 40 40 40 40 40 77.39 78
16 1 4 5 7 10 13 16 17 19 22 25 29 33 36 38 39 39
17 1 4 6 7 8 9 11 12 14 16 17 19 21 23 23 23 25.17 26
18 2 5 9 12 14 15 16 18 21 24 25 29 33 36 38 39 39
19 1 5 8 11 12 14 16 19 21 24 26 30 33 37 40 40 40.95 41
20 1 3 6 8 10 12 13 14 15 18 20 23 26 28 30 31 31
R
i 0.039 0.121 0.197 0.245 0.311 0.369 0.439 0.480 0.541 0.606 0.673 0.756 0.834 0.904 0.965 1.000
Legend:  Last hourly period 100% constrained free
Figures shown in bold and italic identify constrained daily sales histories.

---

## Page 124

Table 5.6 Cumulative Demand Distribution Function
    Product-Limit Technique Unconstraining Using Ris
xj 20 23 31 39 40 41 43 45 46 55 57 65 67 78
F(xj) 0.050 0.100 0.259 0.373 0.500 0.550 0.600 0.650 0.700 0.750 0.800 0.900 0.950 1.000
See Table 5.2 =10/20 =11/20 =12/20 =13/20 =14/20 =15/20 =16/20 =18/20 =19/20 =20/20

---

## Page 125

114  Unconstraining
 
 
Fp D a b p c p
pp
T
− () == + ⋅ + ⋅+
+⋅− () ⋅ () +
12
21                     α ln β β⋅⋅ − ()pp2 1ln
 (5.1)
where a, b, c, α and β are parameters that need to be estimated from the data. Although this 
curve is not used very often in practice, it has a few characteristics worth noting. In par-
ticular, FT
–1(p) is linear in its parameters, which in turn means that its parameters can be 
easily estimated using linear regression techniques. In addition, since FT
–1(p) is specified 
through five parameters, its functional form can accommodate a large variety of demand 
distribution shapes. As a downside, however, certain combinations of parameters do 
not guarantee that F
T
–1(p) is monotonically decreasing in p, especially along its tails. Lau 
and Lau (1996) and Lau, Lau and Kottas (1999) provide extensive coverage of these and 
other related topics. For the Pain de Boulogne data shown in Table 5.6, we depict the 
parameter estimates for the Tocher’s curve in Table 5.7. We compute these parameters 
by regressing D (or, xj s) on the four independent variables that rely on p (or, F (xj)s)). 
The corresponding demand function has a mean µ T and a standard deviation σT which
can be computed as μTT Fp d p= ()−
∫
1
0
1
 and σμTT T Fp d p=− + ()()
−
∫
1
0
1 2
, respectively. 
Through numerical integration (by using, e.g., the function integrate in R), we evalu-
ate µT and σT at 41.7 and 15.1 units, respectively. Using equation (5.1), updated to reflect 
the parameter values of Table 5.7, we can compute demand threshold values that bound 
the demand from above with a certain probability  p. As an example, for a probability 
value p of 0.90, the demand is necessarily smaller than or equal to 63.6 units. We show 
this graphically in Figure 5.5.
Table 5.7 Parameter Estimates for Tocher’s Inverse Cumulative Demand Distribution Function
a b c αβ
41.88 –31.36 58.77 7.90 –1.26
0.0
40
20
80
60 FT
−1(0.90) = 56.5
F–1
G/T(p)
FT
−1(0.90) = 63.6
100
0.2
p = 0.90
µG = 41.2
µT = 41.7
0.60.4 0.8 1.0
Probability p
FG
−1(p) (Gumbel Inverse CDF) F T
−1(p) (Tocher Inverse CDF)
Actual Data
Figure 5.5 Tocher’s Inverse and Inverse Gumbel Cumulative Distribution Functions.

---

## Page 126

Unconstraining  115
As an alternative to the five-parameter Tocher’s inverse cumulative distribution func-
tion shown in equation (5.1), a Gumbel cumulative distribution function FG(x) can be 
fitted to the points (xj, F(xj)) = (Dj, pj). FG(x), expressed as
  
 , (5.2)
 
Fx xG () =−− ⋅ − ()⎛
⎝⎜
⎞
⎠⎟
⎛
⎝
⎜
⎞
⎠
⎟exp exp 1
β μ
is a function of only two parameters µ (the location parameter) and β (the scale param-
eter) that need to be estimated from the data. To compute µ and β, we first linearize FG(x) 
by taking the natural logarithm on both sides of equation (5.2) twice. This leads to
 
 
 
−− ()()() =− + ⋅log log Fx xG
μ
ββ
1
, (5.3)
 
where µ and 
β can be derived analytically as functions of the intercept a and the slope b 
of the linear regression equation that expresses –log (–log (FG(x))) as a function of x. In 
particular, µ equals – a/b and β equals 1/b. For the Pain de Boulogne data shown in Table 
5.6, we depict a, b and the parameters µ and β of the Gumbel cumulative distribution 
function in Table 5.8. Once µ and β are estimated, we can compute the mean µG and the 
standard deviation σG of the corresponding demand distribution. Using the standard 
formulas µG = µ + γ · β and σG = π · β/√6
_
, where γ /H11061 0.577 is the Euler’s constant and π /H11061 
3.142, we evaluate µG and σG for the Gumbel distribution fitted to the Pain de Boulogne 
data at 41.2 and 11.7 units, respectively. These values are comparable to those computed 
for the Tocher’s demand distribution although σG appears to be somewhat smaller than 
σT. Besides inferring µG and σG, we can use µ and β to specify the inverse FG
–1
(p) of the 
Gumbel cumulative distribution function as
 Fp pG
− () =−⋅ ()()1 μβ log log . (5.4)
For the Pain de Boulogne problem, we depict FG
–1
(p) graphically in Figure 5.5. Continu-
ing the example from the Tocher’s inverse curve, we also show in Figure 5.5 how, for a 
probability value p of 0.90, the demand as computed using equation (5.4)  (i.e., under 
the assumption of a Gumbel demand distribution) is necessarily smaller than or equal 
to 56.5 units.
AVERAGING METHOD (AM)
In contrast to how the single period items sell, many other products or services do not 
have a lifespan of just one time period. In fact, many products or services are offered to 
Table 5.8 Parameter Estimates for the Gumbel Cumulative Demand Distribution Function
a b μβ
= –a/b = 1/b 
–3.93 0.11 35.94 9.13

---

## Page 127

116  Unconstraining
customers over multiple time periods that could span several weeks or, sometimes, sev-
eral months or years. Snack foods such as potato chips, for instance, have a shelf life of 6 
to 12 weeks. Once on display, these items sell for as long as their availability lasts but not 
beyond their expiration dates. To assure product availability, these items are replenished 
using either fixed order quantity or fixed time period inventory models (for a relevant 
review of these models, see, e.g., Chopra & Meindl, 2012). Similarly, airplane tickets and 
transient hotel rooms can be typically booked up to 365 days in advance of the departure 
or check-in dates. Since these products cannot be replenished throughout the booking 
horizon (e.g., a sold-out hotel for a particular check-in date is sold-out forever), their 
availability is essentially managed by rationing the capacity made available to customers 
at various price points. In Chapter 4, we cover the aspects of how the availability of such 
perishable products is controlled. In this and the coming sections, we add to that discus-
sion and present a few popular demand unconstraining techniques that emerged and are 
routinely used in the airlines and hospitality industries. Even though these techniques 
were developed in these industries, most can be used in more general settings, which we 
illustrate by applying them to the same Pain de Boulogne data set that was used earlier.
The simplest of the demand unconstraining techniques that originated in the airlines 
industry are the averaging methods. Of their many variants, we focus here on the aver-
aging method that has been shown to perform best in industry applications (Hopper-
stad, Belobaba, & Skwarek, 1996; Queenan, Ferguson, Higbie, & Kapoor, 2007; Saleh, 
1997; Skwarek, 1996; Weatherford, 2000; Weatherford & Pölt, 2002; Zeni, 2001b). This 
method is referred to as Naïve #3 by Weatherford and Pölt (2002), or, simply as the aver-
aging method by Queenan et al. (2007). The technique requires as inputs several booking 
curves of the type shown in Figure 5.1 of which some, but not all, should be constrained. 
Based on the length of the relevant booking window, the averaging method splits the 
booking horizon into a given number of booking periods (e.g., five, ten) whose ends are 
used as demand checkpoints. For a constrained booking curve, this essentially means 
that the end of period i unconstrained cumulative demand equals the sum of the end of 
the previous period’s unconstrained cumulative demand and the maximum of (1) the 
i-th period own sales rate, and (2) the average of the i-th period unconstrained sales rates 
across all booking curves considered. In formal terms, this equates to:
 DD S R U S R
it i t it it t,, , ,max ,=+ ()()− ≠1  average && , (5.5)
where i, 1 ≤ i ≤ I, refers to the current booking period, t identifies a booking curve which 
became constrained before the end of the booking period  i , Di,t refers to the uncon-
strained cumulative demand for booking curve t and booking period  i, SRi,t provides 
the i-th period own sales rate and USRi,t¨≠t relates to the i-th period unconstrained sales 
rate associated with booking curve t¨(t¨ ≠ t). As this detail, although critical, is not always 
apparent, we stress that in equation (5.5) the USRi,t¨ s for the end of the booking horizon 
constrained booking curves t¨ do enter the calculation of the i-th period average for as 
long as the constraining happens after the booking period  i. The unconstrained cumu-
lative demand values DI,t computed for the last of the booking periods and implicitly 
assumed to be random realizations from a normal distribution are employed to esti-
mate the distributional parameters µ and σ that subsequently are to be used to set, for 
instance, the protection levels with EMSRb. The estimates for µ and σ are computed

---

## Page 128

Unconstraining  117
either directly from the sample of  DI,t’s or by maximizing the likelihood of the  DI,t’s via 
maximum-likelihood fitting techniques (by using, for example, the function fitdistr 
from the R contributed package MASS (Venables & Ripley, 2002)). The two pairs of µ  
and σ estimates are given by:
(5.6)
 
μσ μ
μ
AM
D
It
t
N
AM
D
It A M
D
t
N
A
N D N D=⋅ = − ⋅− ()
⎛
⎝
⎜⎜
⎞
⎠
⎟⎟
==
∑∑
11
11
2
1
12
,, , 
M M
MLE
It
t
N
AM
MLE
It A M
MLE
t
N
N D N D=⋅ = ⋅ − ()
⎛
⎝
⎜
⎜
⎞
⎠
⎟
⎟
==
∑∑
11
1
2
1
1
,, , σμ
2 2
,
 
where D stands for the direct approach, MLE stands for the maximum-likelihood 
approach, AM stands for averaging method and N identifies the number of DI,t observa-
tions. To make things more concrete, we illustrate how the averaging method is opera-
tionalized using data that build on the booking curves depicted in Figure 5.1.
To keep the exposition concise, we consider six business booking curves for six con-
secutive Tuesday night hotel stays. The first three of these booking curves are depicted in 
Figure 5.1. The full data set is provided in tabular form in panel A of Table 5.9. For the 
purpose of this work, we split the booking horizon into five booking periods, each of a 
length of three days. To compute, for example, the unconstrained cumulative demand 
D
3,t at the checkpoint of six days before the check-in date, we rely on the unconstrained 
cumulative demand D2,t and the sales rates experienced throughout booking period 3. 
Since none of the booking curves is constrained nine days before the check-in date, D2,t 
equal the end of booking period 2 sales. We illustrate this point in the second column 
of panel B in Table 5.9. Throughout booking period 3, booking curves 3 and 5 get con-
strained. Hence, the period 3 sales rates for these booking curves are not considered in 
the computation of the average of period 3 unconstrained sales rates. In the third column 
of panel B in Table 5.9, we label period 3 constrained sales rates with a C and provide 
the average unconstrained sales rate for the period in the last entry of the column. We 
then apply equation (5.5) to both of the already constrained booking curves and evalu-
ate D
3,t, which we present in Table 5.9 in the last column of panel B. A similar approach 
allows us to compute iteratively D 4,t and D5,t, respectively. With D5,t now estimated, we 
can calculate the estimates for the average µ and the standard deviation σ of the assumed 
underlying normal distribution using the formulae provided in equation (5.6).
Returning to the Pain de Boulogne data provided conveniently in cumulative hourly 
sales format in Table 5.5, we operationalize the averaging method by splitting the store’s 
opening hours into five sales periods with demand checkpoints at 4, 7, 10, 13 and 16 
hours after the time the store opens. To initialize the method, we assume that the avail-
able daily inventory equals the daily sales for the days that experience stock-outs and 
the daily sales plus one additional unit for the days without stock-outs. We then use 
equation (5.5) iteratively to compute the unconstrained cumulative demand D
i,t across 
all sales periods i and sales histories t. We summarize the steps of this iterative process 
in Table 5.10. The last two columns in this table show that the averaging method is less 
aggressive in its unconstraining than the technique we discussed in the previous section. 
This is not unexpected for this particular example since the absolute values of the sales

---

## Page 129

Table 5.9 Operationalization of Averaging Method for Demand Unconstraining
Protection Level: 10 units
(A) Business Booking Curves (BBC) (B) Averaging Method
Booking
Curve
Days before Check-In Date Booking Checkpoint at Time
Period 1 Period 2 Period 3   Period 4   Period 5 Curve 9 6
t 14 13 12 11 10 9 8 7 6 5 4 3 2 1 0 t D 2,t USR 3,t D 3,t 
BBC1 0 0 0 0 0 0 2 2 3 3 4 5 6 6 7 BBC 1 0.00 3.00 3.00
BBC2 0 1 1 2 2 3 3 4 4 5 6 7 8 8 10 BBC 2 3.00 1.00 4.00
BBC3 0 3 5 5 6 8 8 9 10 10 10 10 10 10 10 BBC3 8.00 C 10.50
BBC4 12 2 235 56 8 9 91 0 1 0 1 0 1 0 BBC4 5.00 3.00 8.00
BBC5 13 6 677 9 1 0 1 0 1 0 10 10 10 10 10 BBC5 7.00 C 10.00
BBC6 2 2 3 3 3 3 4 5 6 7 8 8 8 8 9 BBC 6 3.00 3.00 6.00
Average 2.50
Legend: USR: Unconstrained Sales Rate
     D: Unconstrained Cumulative Demand
Figures shown in bold and italic identify constrained booking curves.

---

## Page 130

Unconstraining  119
rates across the unconstrained and the constrained sales histories are clearly not simi-
lar. The proportionality assumption used throughout the previous section corrects for 
this shortcoming and allows the unconstraining technique that builds on the Product-
Limit method to be somehow more intrusive (and, probably, more realistic). In absolute 
terms, the average µ and the standard deviation 
σ of the assumed underlying normal 
demand distribution evaluate to µ D
AM = 39.2 and µ D
AM = 10.2 (or, alternatively, to µMLE
AM = 
39.2 and σ MLE
AM = 10.0). As a reference point, we remind the reader that the parameters of 
the demand distributions of the previous section were estimated at (µT, σT) = (41.7, 15.1) 
and (µG, σG) = (41.2, 11.7), respectively.
DOUBLE EXPONENTIAL SMOOTHING (DES)
The double exponential smoothing (DES) unconstraining technique (Queenan et al., 
2007) recognizes that the bookings or the product sales accumulate in time and could be 
effectively described in terms of the time series forecasting concepts discussed in Chap-
ter 2. At its core, the double exponential smoothing technique uses the time dependent 
Table 5.10 Demand Unconstraining via Averaging Method (AM)
Day
t 
Available
Inventory
Checkpoint at Time Unconstrained
Demand4 7 10 13 16
USR
1,t D 1,t USR 2,t D 2,t USR 3,t D 3,t USR 4,t D 4,t USR 5,t D 5,t AM Table 5.5
1 4 0 1 01 2 1 02 2 1 03 2 C 4 0 C 4 5 4 5 5 5
2 40 13 16 13 29 C 40 C 48 C 53 53 65
3 40 7 8 13 21 8 29 9 38 C 43 43 46
4 40 8 10 10 20 7 27 9 36 C 41 41 43
5 40 13 15 15 30 C 40 C 48 C 53 53 67
6 32 7 8 8 16 4 20 6 26 5 31 31 31
7 40 9 12 14 26 9 35 C 43 C 48 48 57
8 21 5 6 4 10 3 13 4 17 3 20 20 20
9 32 7 8 6 14 5 19 6 25 6 31 31 31
10 40 15 17 10 27 C 40 C 48 C 53 53 65
11 24 4 5 6 11 3 14 5 19 4 23 23 23
12 39 9 11 5 16 7 23 10 33 C 39 39 40
13 31 6 8 8 16 5 21 6 27 C 32 32 33
14 40 8 9 6 15 7 22 15 37 C 42 42 45
15 40 18 21 13 34 C 40 C 48 C 53 54 78
16 40 6 7 9 16 6 22 11 33 6 39 39 39
17 23 6 7 4 11 5 16 5 21 C 26 26 26
18 40 10 12 4 16 8 24 9 33 6 39 39 39
19 40 10 11 5 16 8 24 9 33 C 40 40 41
20 32 7 8 5 13 5 18 8 26 5 31 31 31
Average 8.90 8.40 6.25 8.00 5.00
Legend:    USR: Unconstrained Sales Rate
 D: Unconstrained Cumulative Demand 
Figures shown in bold and italic identify constrained daily sales histories.

---

## Page 131

120  Unconstraining
information available from before the stock-outs to project the unconstrained demand 
that would have been observed in the absence of any booking or inventory limits. In 
addition, the DES method is appealing because: (1) it builds on a well-known statisti-
cal forecasting technique that is not computationally intensive (see the section ‘Double 
Exponential Smoothing’ in Chapter 2); (2) it is nonparametric in that it does not impose 
any strong assumptions on the shape of the booking curves/cumulative product sales 
or the distribution of the final total demand; and (3) it can handle situations where all 
booking curves/cumulative product sales histories are constrained.
We illustrate the method’s key ideas using one of the booking curves provided in Table 
5.9. In particular, if we focus on booking curve BBC
4, we learn that the hotel gets sold-out 
three days before the corresponding Tuesday check-in date. Due to the hotel rooms being 
unavailable for the last few days of the booking horizon, no true demand information 
exists for this check-in date. However, assuming that the booking patterns before and 
after the out-of-stock event starts do not vary that much, we can forecast the end of the 
booking horizon demand using double exponential smoothing which accounts for the 
inherent cumulative sales trend and ignores the obviously missing cumulative sales sea-
sonality. Building on the concepts introduced in Chapter 2, if S
4 and T4 are the smoothed 
mean and the trend updated after the last record of the unconstrained cumulative sales is 
observed (i.e., the cumulative sales of nine units recorded four days before the check-in 
date), we can compute the demand forecast for the end of the booking horizon as F
0 = S4 
+ 4 · T4. In the expression of F0, S4 and T4 are computed recursively as S4 = α · D4+ (1 – α) · 
(S5 + T5) and T4 = β · (S4 – S5) + (1 – β) · T5, where D4 is the observed unconstrained 
cumulative sales four days before the check-in date and α and β are smoothing param-
eters estimated so as to minimize the in-sample mean square error MSE4. The apparently 
counterintuitive use of indices in F0, S4, and T4 reflects the fact that, in this example, the 
time is counted backward from 14 days before the check-in to 0 days before the check-in. 
The optimal α and β parameter values of 0.79 and 0.00 (constant trend) lead to S4 = 9.20 
and T4 = 1.00. Thus, the demand forecast for the end of the booking horizon evaluates to 
F0= 9.20 + 4.1 = 13.20 rooms. We show how this point forecast is obtained in Figure 5.6.
14
5
0
10
15
11 1012 13 9 6 587 43210
Days Before Check-In Date
Cumulative Hotel Booking/Demand
Cumulative Sales ForecastsCumulative Sales BBC4
Unconstrained Demand
Figure 5.6 Illustration of Demand Unconstraining via Double Exponential Smoothing.

---

## Page 132

Unconstraining  121
Returning to the Pain de Boulogne data shown in Table 5.1, we use for each of the 
daily sales considered the unconstrained portions of the cumulative sales histories to 
compute the smoothing parameters αt and βt so as to minimize the relevant in-sample 
mean square errors MSE i,t. The indices t and i in αt, βt, and MSE i,t refer to the current 
cumulative sales history and to the last of its hourly unconstrained cumulative sales peri-
ods, respectively. For the first of the Pain de Boulogne histories, for example, the 
α1 and 
β1 values of 0.586 and 1.000 minimize MSE11,1. For each (αt,βt) pair, we then evaluate the 
smoothed mean Si,t and trend Ti,t that characterize the end of the unconstrained portion 
of the cumulative sales histories. We use these Si,t and Ti,t values to subsequently compute 
the end-of-the-day unconstrained demand forecast Dt as Dt = F16,t= Si,t + ht · Ti,t, where ht 
= 16 – i. For the first of the cumulative sales histories depicted in Table 5.5, the S 11,1and 
T11,1 of 36.45 and 5.05, respectively, result in an end-of-the-day unconstrained demand 
D1(= F16,1) of 61.72, or, 62 units. For completeness, we show how all end-of-the-day 
unconstrained demands Dt are computed in Table 5.11. In addition, we provide a graph-
ical account of this computational process in Figure 5.7. The unconstrained Dt values in 
Figure 5.7 illustrate clearly that, in this particular application, the key source of demand 
uncertainty relates to changes in the demand levels rather than the customer purchase 
behavior (i.e., purchase earlier or later but in similar amounts).
As observed from the last columns of Table 5.11, for this particular problem, the DES 
method is similar in aggressiveness in demand unconstraining as the method discussed 
Table 5.11 Demand Unconstraining via Double Exponential Smoothing (DES)
Day
t /H9251t /H9252t iS i,t T i,t h t Dt
Unconstrained Demand
DES AM Table 5.5
1 0.586 1.000 11 36.45 5.05 5 61.72 62 45 55
2 1.000 0.000 9 35.00 4.00 7 63.00 63 53 65
3 1.000 0.000 13 38.00 3.00 3 47.00 47 43 46
4 0.277 0.345 14 38.40 2.69 2 43.79 44 41 43
5 0.290 1.000 9 36.92 3.60 7 62.09 63 53 67
6 – – – – – – 31.00 31 31 31
7 1.000 0.070 11 38.00 3.73 5 56.66 57 48 57
8 – – – – – – 20.00 20 20 20
9 – – – – – – 31.00 31 31 31
10 0.721 1.000 9 34.12 4.88 7 68.31 69 53 65
11 – – – – – – 23.00 23 23 23
12 1.000 0.507 14 36.00 3.08 2 42.16 43 39 40
13 1.000 0.292 13 27.00 2.11 3 33.32 34 32 33
14 0.887 1.000 13 36.87 6.04 3 54.99 55 42 45
15 0.893 0.433 7 33.97 4.54 9 74.80 75 54 78
16 – – – – – – 39.00 39 39 39
17 0.968 0.747 13 20.99 1.95 3 26.85 27 26 26
18 – – – – – – 39.00 39 39 39
19 0.772 1.000 14 36.87 3.84 2 44.55 45 40 41
20 – – – – – – 31.00 31 31 31
Legend:    D: Unconstrained Demand
Figures shown in bold and italic identify constrained cumulative sales histories.

---

## Page 133

122  Unconstraining
in the section ‘Estimation of Demand Distributions of Censored Single-Period Items’. In 
absolute terms, if a normal demand distribution is assumed to describe the underlying 
data, its average µ and standard deviation σ evaluate to µD
DES = 44.9 and σ D
DES = 16.0 (or, 
alternatively, to µMLE
DES = 44.9 and σ MLE
DES = 15.6).
EXPECTATION-MAXIMIZATION (EM) ALGORITHM
The Expectation-Maximization (EM) algorithm (Dempster, Laird, & Rubin, 1977) is a 
statistical-based technique which, for a variety of incomplete-data problems, computes 
maximum likelihood estimates iteratively. The use of the EM algorithm is justified by 
the fact that in many statistical applications such as those that need to deal with grouped, 
censored or truncated data, the estimation of the maximum likelihood parameters is 
made difficult by the structure of the corresponding (log) likelihood function. In such 
instances, the direct optimization over the incomplete-data (log) likelihood function is 
known to be a difficult-to-solve maximization problem. In the context of our work, the 
fact that some of the historical observations are constrained puts this estimation prob-
lem into that category.
In general, the EM algorithm computes the maximum likelihood estimates for an 
incomplete-data problem by formulating an associated complete-data problem that is 
much simpler to solve. By iteratively revising the maximum likelihood estimates for the 
simpler problem, the EM algorithm ultimately computes the maximum likelihood esti-
mates for the original incomplete-data problem. To get a sense for what the EM algorithm 
does, we discuss it in a context that builds on some of the specifics of our unconstrain-
1
20
0
40
60
80
6
Time (Hours)
1611
Cumulative Sales/Demand
Constrained/Unconstrained Cumulative Sales
Cumulative Sales Forecasts
Unconstrained Demand
Figure 5.7 Demand Unconstraining via Double Exponential Smoothing.

---

## Page 134

Unconstraining  123
ing problem. Consider that we are provided with a series of observations x = (x1,…,xn) 
which are independent and identically distributed and come from a continuous 
distribution with probability density function f (x). For this set of observations, the 
complete-data log likelihood function is given by log | logLx f xc
i
i
n
θ()() = ()
⎛
⎝
⎜⎜
⎞
⎠
⎟
⎟
=
∏
1
 
where θ = (θ1,…,θp) is a vector of unknown parameters that describe f (x). Consider 
further that y and z are vectors that consist of all uncensored (fully observed values in  
y) and censored (constrained values in z ) observations of  x. Given this separation, we 
can write the corresponding incomplete-data log likelihood function as log( L(θ | y)) = 
log(/H20848L
c
(θ | y, z)dz). Since z is not fully known but rather censored, the direct maximi-
zation of log(L(θ | y)) to estimate θ is difficult. Instead of this direct approach to com-
puting θ, the EM algorithm approaches the problem of solving the incomplete-data 
problem indirectly by iteratively employing the complete-data log likelihood function 
log (L
c
(θ | x)). In particular, during the Expectation step (or, the E-step) of each itera-
tion k of the EM algorithm, the complete-data expected conditional log likelihood 
function is computed as
(5.7)
 
QE L x y
Ly z p z y
k
c
k
c
k
θθ θ θ
θθ
|l o g | ,
log | , | ,
−−
−
() = ()(){}
= ()() ()∫
11
1 ddz,
where θk–1 are the estimates for θ revised at iteration k–1 and p(z | y, θk–1) is the probabil-
ity density function of z. In equation (5.7), we take the expectation of log (L
c
(θ | x)) given 
the fully observed data y and the previously estimated parameter estimates θk–1 (vs. log(L
c
(θ | x)) because log(L
c
(θ | x)) is unobservable. With Q(θ | θk–1) expressed analytically, the 
Maximization step (or, the M-step) of each iteration k of the EM algorithm finds esti-
mates θk such that Q(θ | θk–1) is maximized. Upon its completion, the EM algorithm is 
shown to typically converge (under fairly general conditions) to the global maximum of 
the incomplete-data log likelihood function (Boyles, 1983; Dempster et al., 1977; Redner 
& Walker, 1984; Wu, 1983).
Since the generic discussion of the E- and M-steps above may be too abstract, we 
expand on it next to provide the solution to our specific unconstraining problem exam-
ple. For clarity, we slightly alter the notations around x, n, y, z and 
θ as follows. We assume 
that the available M + N observations zi, 1≤ i ≤ M + N, are realizations of a sequence of 
independent and identically distributed normal random variables. The parameters θ = 
(µ, σ) of the underlying normal distribution are unknown and must be estimated. Of the 
M + N observations, M are constrained at random either by reaching the corresponding 
booking limits or by running out of inventory. For these observations, zi = bi, where bi, 
the booking limit or the available inventory, constrains the true value of zi. For conven-
ience only, we assume that the first M observations in zi are constrained; the other N are 
the ones exactly specified.
If the data was not constrained, the complete-data likelihood and log-likelihood func-
tions L
c
(µ, σ | zi) and log(L
c
(µ, σ | zi)) given by

---

## Page 135

124  Unconstraining
  
 
 
 
                
   
Lz ec
i
z
i
MN
i
μσ
σπ
μσ
,() =
⋅⋅
⋅
−−() ⋅()
=
+
∏
1
2
2 22
1
                                =
⋅⋅
⎛
⎝⎜
⎞
⎠⎟ ⋅
+ −⋅ ()1
2
12 2
σπ
σMN
e
(() ⋅− ()
=
+
∑
()() =− + ⋅⋅ () −
z
c
i
i
i
MN
Lz MN M
μ
μσ π
2
1
2 2
and
       log , ln + +() ⋅−
−()
⋅
=
+
∑
N
zi
i
MN
lnσ
μ
σ
2
1
22
 (5.8)
would be maximized by the closed-form parameter estimates µ andσ:
 
 
 
 
 
 (5.9)
 
 
 
 
 
μ
σ
= + ⋅= + ⋅+
⎛
⎝
⎜⎜
⎞
⎠
⎟⎟
= + ⋅
=
+
== +
+
∑∑ ∑
11
1
11 1MN z MN zz
MN z
i
i
MN
i
i
M
i
iM
MN
i − −()
⎛
⎝
⎜⎜
⎞
⎠
⎟⎟
= + ⋅− () +− ()
=
+
== +
+
∑
∑
μ
μμ
2
1
12
2
1
2
1
1
i
MN
i
i
M
i
iM
MN
MN zz
/
∑ ∑
⎛
⎝
⎜⎜
⎞
⎠
⎟⎟
⎛
⎝
⎜⎜
⎞
⎠
⎟
⎟
12/
.
 
In equation (5.9), we favor the formulation of parameter estimates in terms of two sums 
to prepare for the discussion of how the incomplete-data case should be approached.
In equation (5.8),  the zi′s that correspond to the M constrained observations are 
unobserved. Hence, we cannot use equation (5.9) to compute µ and σ for the incom-
plete-data problem directly. However, if, conditional on a current set of parameter 
estimates µk–1 and σk–1, these zi′s are replaced by their expected values Z i
(k)
 such that
EL z z M i Nc
ii k klog , | , , ,μσ μ σ()() <≤(){} −− 11  is computed analytically (the E -step), 
we could still use formulas of the type shown in equation (5.9) to suggest revised esti-
mates µk and σk for the parameters of the assumed underlying normal demand distribu-
tion (the M -step). In formal terms (see, e.g., Swan, 1969; Wolynetz, 1979), the iterative 
application of the E- and M-steps of the EM algorithm proceeds as follows:
 Initialization. Initialize µ and σ to be the sample mean and the sample standard devi-
ation (uncorrected for the degrees of freedom) of all unconstrained observations. 
 Thus, express µ and σ as μ μ== ⋅
=+
+
∑0
1
1
N iM
MN
    and σσ μ== ⋅ − ()
⎛
⎝
⎜⎜
⎞
⎠
⎟
⎟
=+
+
∑00
2
1
12
1
N zi
iM
MN /
. 
 If most observations are constrained (i.e., N ≤ 1), stop the algorithm and report a 
warning message. The EM method does not work when all observations are con-
zi

---

## Page 136

Unconstraining  125
strained so other methods, including the DES method discussed earlier, are recom-
mended to handle these extreme cases. 
 E-Step at Iteration k, k ≥  1. Replace zi, 1 ≤ i ≤ M, with their expected values  Zi
(k)
. 
The Zi
(k)
s are computed assuming that they are the expected values of the normal 
distributions N (µk–1, σ2
k–1) left truncated at bi = zi (i.e., TN(µk–1, σ 2
k–1, bi,+∞)). Spe-
cifically, if X is a normally distributed random variable with mean µk–1 and standard 
 deviation σk–1, ZE X X b X N S hi
k
ik k k k i
()
−− − −=> ()⎡
⎣
⎤
⎦ =+⋅
()|, ~ , μσ μ σ11
2
11  (or, 
 equivalently, ZE T N b S hi
k
kk i k k i
()
−− − −=+ ∞()⎡
⎣
⎤
⎦ =+⋅
()μσ μ σ11
2
11,, , ), where hi equals 
 ( bi – µk–1)/σ k–1 and S(h), or, the generic hazard function of a normal distribution, 
writes as S(h) = φ(h)/(1 – Φ(h)) (S(h)s are computed by replacing the generic ele-
ment h with the corresponding hi′s). φ and Φ in the expression of the hazard func-
tion are the standard normal density function and the standard normal cumula-
tive distribution function, respectively. Alternatively, the Zi
(k)
s can be computed 
through numerical integration (by using, for example, the function integrate 
 in R) as x f xd x f xd x
bbii
⋅ () ()
+∞ +∞
∫∫ , where f(x) is the normal probability density 
 function of  X.
 M-Step at Iteration k, k ≥  1. Revise the parameter estimates for µ  and σ by 
 maximizing the expected conditional log-likelihood function EL z c
ilog , | μσ()(){  
 zMiNik k,, , μσ<≤( ) }−− 11 .The optimal µk and σk write as:
 
μk i
k
i
M
i
iM
MN
MN Zz= + ⋅+
⎛
⎝
⎜⎜
⎞
⎠
⎟
⎟
== +
+
∑∑
1
11
() , and,
 
σμ μk
i
i
M i
k
k
i
M
ik
iMTh N
Zz=
()
⎛
⎝
⎜⎜
⎞
⎠
⎟⎟+
⋅− () +− ()
=
−
=
−
=+
∑
∑
1
1
1
2
1
1
2()
1 1
12
MN+
∑
⎛
⎝
⎜⎜
⎞
⎠
⎟⎟
⎛
⎝
⎜
⎜
⎜
⎜
⎜
⎞
⎠
⎟
⎟
⎟
⎟
⎟
/
,
respectively, where hi = (bi– µk–1)/σk–1 and T (h) = S(h) · (S(h) – h) (T (hi)s are com-
puted by replacing the generic element h with the corresponding his).
 Convergence test. If |µk – µk–1| <ε and |σk – σk–1| <ε, stop; otherwise, proceed with 
iteration k + 1 of the expectation-maximization algorithm. The tolerance ε is typi-
cally a small number such as 1e-06. If convergence is reached, µk and σk are the
 parameter estimates of µ and σ . Similarly, Zi
(k)
s (or, Z i
(k+1)
s) could be used as the 
unconstrained values of the zi s, i ≤ M.

---

## Page 137

126  Unconstraining
To illustrate how the EM algorithm works in practice, consider again the data provided 
in panel A of Table 5.9. Of the six available booking curves, three reach the booking limit 
of ten rooms before the end of the booking horizon. Hence, the corresponding observa-
tions z
i, i ≤ M = 3, are right censored at ten. The other three observations zi, M = 3 < i ≤ 
M + N = 6, are exactly specified as seven, nine and ten rooms, respectively. We initialize 
µ and σ to be µ0 = (7 + 9 + 10) / 3 = 8.667 and σμ00
2
1
12
3 1 247=− ()
⎛
⎝
⎜⎜
⎞
⎠
⎟
⎟ =
=+
+
∑ zi
iM
MN
. , 
respectively. For each of the constrained  zi, i ≤ M = 3, observations (which incidentally 
here are all ten), we evaluate next hi, S (hi) and T (hi) to be 1.069, 1.581 and 0.809, respec-
tively. This yields Zi 
(1)
 = 10.638 for all i ≤ M = 3, (the E-step) and µ1 = 9.652 and σ1 = 1.735 
(the M-step). For completeness, we provide the first two and the last of the iterations of 
the EM algorithm for this admittedly small problem in Table 5.12. As it becomes appar-
ent from the last column of this table, the unconstrained values Z i 
(20)
, i ≤ M = 3, are all 
equal irrespective of the time period within the booking horizon that the booking limit 
bi of ten rooms was reached. This stresses the fact that unlike the DES technique, which 
is time dependent, the EM algorithm is oblivious of how the booking/sales intensity 
evolves in time. To this end, all the EM algorithm requires as inputs are the end of the 
booking horizon sales and whether or not these sales are constrained.
Returning to the Pain de Boulogne data shown in Table 5.1, we apply the EM algo-
rithm to the end-of-the-day constrained and unconstrained sales values to compute 
parameters µ and 
σ of the underlying normal demand distribution. We summarize the 
EM iterations in terms of Zi
(k)
, µk and σk in Table 5.13. As for the limited example above, 
we highlight that in spite of final estimates µk and σk that are in line with those suggested 
by the other unconstraining techniques, the unconstrained demand values Zi appear 
to consistently be either over- or under-forecasted (e.g., days 4 and 13 and days 10 and 
15, respectively). As we speculated previously, this is the direct result of the EM algo-
rithm being ignorant of the time dependent mechanism that censors the data. While 
this time-indifference is usually listed as one of the major limitations of the EM algo-
rithm, we stress again that essentially all of the techniques we have discussed so far in 
this book require the parameter estimates of the unconstrained demand distributions 
and not the unconstrained demand values themselves. Thus, a method that consistently 
over estimates some demand streams but under estimates a similar number of others 
can produce reasonable estimates for the underlying demand distribution parameter 
values. This is the case of the EM results for our example problem and is true for the 
performance of the EM algorithm in many similar studies. In fact, in terms of the final 
revenue impact in revenue management settings, the EM algorithm has been shown to 
outperform all common unconstraining techniques with the exception of (for certain 
conditions) the DES and the Projection-Detruncation methods (Queenan et al., 2007; 
Weatherford & Pölt, 2002; Zeni, 2001b).
PROJECTION-DETRUNCATION (PD)
The Projection-Detruncation (PD) method (Hopperstad, 1997) is similar in spirit to 
the EM algorithm in that it iteratively replaces the constrained observations with some 
expected values and then updates the parameters of the underlying demand distribution

---

## Page 138

Table 5.12 Operationalization of the EM Algorithm for Demand Unconstraining
µ0=8.667 µ1=9.652 µ2=9.966 µ 20=10.092
σ0=1.247 σ1=1.735 σ2=1.748 σ20=1.859
i zi Iteration 1 Iteration 2 Iteration 20
hi /H9272(hi) /H9278(hi) S(hi) T(hi) zi/Zi
(1) hi /H9272(hi) /H9278(hi) S(hi) T(hi) zi/Zi
(2) T(hi) zi/Zi
(20) 
1 10* 1.069 0.225 0.857 1.581 0.809 10.638 0.200 0.391 0.579 0.930 0.678 11.265 0.626 11.517
2 10* 1.069 0.225 0.857 1.581 0.809 10.638 0.200 0.391 0.579 0.930 0.678 11.265 0.626 11.517
3 10* 1.069 0.225 0.857 1.581 0.809 10.638 0.200 0.391 0.579 0.930 0.678 11.265 0.626 11.517
4 7 –––– 1 7–––– 1 7 1 7
5 1 0 –––– 11 0–––– 11 0 11 0
6 9 –––– 1 9–––– 1 9 1 9
Legend:    * identifies constrained demand observations.

---

## Page 139

128  Unconstraining
accordingly. Provided that a demand instance z is censored at an arbitrary, yet, observed 
value b, the PD method replaces z with Z such that the likelihood of underestimating the 
unconstrained demand is bounded and known. In probabilistic terms, Z is computed 
such that the conditional probability of the demand being greater than Z given that it is 
already greater than b equals an arbitrary constant τ bounded by zero and one. Formally, 
Z, Z > b, is the solution of the following equation:
 
 
τ = () ()
= () () + ()
⎛
⎝
⎜
+∞ +∞
+∞ +∞
∫∫
∫∫ ∫
fx d x fx d x
fx d x fx d x fx d x
Zb
Zb
Z
Z
  ⎜ ⎜
⎞
⎠
⎟
⎟= +
B
AB
, (5.10)
Table 5.13 Demand Unconstraining via the EM algorithm
t zi 
zi/Zi
(k) at iteration Unconstrained Demand
1 2 3 … 40 EM(a) DES(b) AM(b) Table 5.5(c)
1 40 43.02 47.88 49.14 51.45 51.45 62 45 55
2 40 43.02 47.88 49.14 51.45 51.45 63 53 65
3 40 43.02 47.88 49.14 51.45 51.45 47 43 46
4 40 43.02 47.88 49.14 51.45 51.45 44 41 43
5 40 43.02 47.88 49.14 51.45 51.45 63 53 67
63 1 3 1 3 1 3 1 3 1 3 1 3 1 3 1 3 1
7 40 43.02 47.88 49.14 51.45 51.45 57 48 57
82 0 2 0 2 0 2 0 2 0 2 0 2 0 2 0 2 0
93 1 3 1 3 1 3 1 3 1 3 1 3 1 3 1 3 1
10 40 43.02 47.88 49.14 51.45 51.45 69 53 65
11 23 23 23 23 … 23 23 23 23 23
12 39 42.18 47.21 48.54 50.89 50.89 43 39 40
13 31 36.17 42.61 44.57 47.19 47.19 34 32 33
14 40 43.02 47.88 49.14 51.45 51.45 55 42 45
15 40 43.02 47.88 49.14 51.45 51.45 75 54 78
16 39 39 39 39 39 39 39 39 39
17 23 32.18 39.62 42.28 44.96 44.96 27 26 26
18 39 39 39 39 39 39 39 39 39
19 40 43.02 47.88 49.14 51.45 51.45 45 40 41
20 31 31 31 31 31 31 31 31 31
µ 30.57 37.73 41.11 42.04 … 43.58 43.58 44.90 39.20 41.20
σ 6.67 10.85 10.93 11.22 12.57 12.57 16.00 10.20 11.70
(a) The unconstrained demand values are not rounded up to the closest integer because µ and σ reflect the raw numeric 
values. (b) The reported standard deviation σ is corrected for the degrees of freedom. (c) µ and σ are the mean and stand-
ard deviation of the corresponding Gumbel distribution.
Figures shown in bold and italic represent constrained sales values. 
For consistency and clarity, we present the EM results ordered by t (vs. the index i which we use to describe the EM 
algorithm).

---

## Page 140

Unconstraining  129
where X is typically a normally distributed random demand variable with mean µ and 
standard deviation σ, f(x) is the probability density function of X, fx d x B
Z
() =
+∞
∫  is the 
probability that X is greater than Z, fx d x
b
()
+∞
∫  = () + () =+∫∫
+∞
fx d x fx d x A B
b
Z
Z
 is the 
probability that X is greater than b, and, τ, the conditional probability that X is greater 
than Z given that X is greater than b, is a user-specified constant that scales the aggres-
siveness of the unconstraining algorithm (similar to the smoothing constants used in 
exponential smoothing forecasting methods discussed in Chapter 2 ). Intuitively, a τ 
close to zero requires the probability that X is greater than Z be small, in which case, Z 
will likely be a very large number. A τ of zero necessarily means that Z is infinity (given 
that b is finite). Conversely, a τ that approaches 1 requires the probabilities of X being 
greater than b and Z be close, in which case, Z will likely approach b from above. A τ of 
1 necessarily means that Z = b. For convenience, we show graphically and contrast in 
Figure 5.8 how the EM algorithm (the E -step) and the DP method (in an E -like step) 
compute the corresponding unconstraining values Z. In this example, we use the index 
k, adjusted appropriately when used with Z, µ and σ, to denote that we compute at each 
iteration k the Z that corresponds to the constrained observation z based on the param-
eters of the demand distribution updated after iteration k –1.
To formalize the PD method, we begin with the same set of assumptions we used to 
describe the EM algorithm. In particular, we assume that the available M + N observa-
tions zi, 1 ≤ i ≤ M + N, are realizations of a sequence of independent and identically dis-
tributed normal random variables. The parameters θ = (µ,σ) of the underlying normal 
0
A
ZPD
KZEM
Kz=b
z=b
via PD
via EM
B
Demand (units)
Probability Density Function
TN b kk(, , , )μσ ∞−− +11
2N(μ σkk−−11
2,)
ZZ E T N bk
EM
k
kk== +−−[( , , , ) ]μσ ∞11
2
ZZ s t B A Bk
PD
k== + .. /( )τ
Figure 5.8 PD E-like Step vs. EM E-Step.

---

## Page 141

130  Unconstraining
distribution are unknown and should be estimated. Of the M + N observations, M are 
censored at random in which case zi = bi, where bi is either the booking limit or the avail-
able inventory. Finally, we assume that the first M observations in zi are constrained; the 
other N are the ones exactly specified. With these assumptions in place, the PD method 
(Gorin, 2000; Hopperstad, 1997; Zickus, 1998) proceeds as follows:
 Initialization. Initialize µ  and σ to be the sample mean and the sample stand-
ard deviation (corrected for the degrees of freedom) of all unconstrained 
 observations. T hus, express µ and σ as μμ== ⋅
=+
+
∑0
1
1
N zi
iM
MN
 and 
 σσ μ== − ⋅− ()
⎛
⎝
⎜⎜
⎞
⎠
⎟⎟=+
+
∑00
2
1
12
1
1N zi
iM
MN /
. Similar to the EM algorithm, if most obser-
vations are constrained (i.e., N ≤ 1), stop the algorithm and report a warning message. 
Assign τ a value in between zero and one (e.g., 0.30).
 E-like Step at Iteration k, k ≥ 1. Use equation (5.10) to replace zi, 1≤i≤M, with the 
corresponding Zi
(k) values. The Zi
(k)s are computed assuming that the probability 
density function f(x) in the integrals A and B describes a normally distributed ran-
dom demand variable X with mean µk–1 and standard deviation σk–1. In practice, the 
Zi
(k)s are computed solving equation (5.10) numerically (by using, e.g., the func-
tions integrate and uniroot in R), or, via some appropriate approximations. 
Zeni (2001a), for example, proposes an approach that relies on writing the integral 
B successively in terms of the standard normal cumulative distribution function
 Φ i.e., BZ i
k
kk=− − ( )⎛
⎝⎜ ⎞
⎠⎟⎛
⎝⎜ ⎞
⎠⎟()
−−1 11Φ μσ  and the Gauss error function erf 
 i.e., Φ Ze rf Zi
k
kk i
k
kk
()
−−
()
−−−( )⎛
⎝⎜ ⎞
⎠⎟=⋅ + − ( ) ⋅()μσ μ σ11 1 1
1
2 12 ⎛ ⎛
⎝⎜ ⎞
⎠⎟⎛
⎝⎜ ⎞
⎠⎟
⎛
⎝⎜
⎞
⎠⎟ , with the 
latter being approximated with an elementary function that allows Zi
(k) to be 
expressed explicitly. As an alternative to these involved approaches, we suggest a 
methodology that builds on the concepts discussed in the E -step of the EM algo-
rithm. In particular, if we rewrite equation (5.10)  in terms of the probability 
 density function of the truncated normal distribution TN b kk iμσ−− +∞() 11
2,, ,  
 vs. N kkμσ−−()( )11
2,  and solve τ = BTN/(ATN + BTN) for Zi,TN
(k), we could use the Zi,TN
(k)’s 
 as the Zi
(k)s since the two formulations are equivalent. Because fx d xTN
b
() =
+∞
∫ 1, 
 equation (5.10)  reduces to τ = ()
()
+∞
∫ fx d xTN
ZiT N
k
,
, which can be more easily solved 
 using the inverse of the cumulative truncated normal distribution function (by 
using, e.g., the function qtnorm from the R contributed package msm (Jackson, 
2011)). In this case, τ maintains its conditional probability status since the nor-
mally distributed variable X~N (µk–1, σ2
k–1) is left truncated at bi and the equivalent 
truncated normal distribution TN(µk–1, σ2
k–1) is reparameterized accordingly.

---

## Page 142

Unconstraining  131
 M-like Step at Iteration k, k /H113501. Revise the parameter estimates for µ and σ such 
that:
μk i
k
i
M
i
iM
MN
MN Zz= + ⋅+
⎛
⎝
⎜⎜
⎞
⎠
⎟⎟
== +
+
∑∑
1
11
() , and,
σμ μk i
k
k
i
M
ik
iM
MN
MN Zz= +− ⋅− () +− ()
⎛
⎝
⎜⎜
⎞
⎠
⎟⎟
⎛
⎝
−
=
−
=+
+
∑∑
1
1 1
2
1
1
2
1
()⎜ ⎜⎜
⎞
⎠
⎟
⎟
12/
 Convergence test. If |µk – µk–1| <ε and |σk – σk–1| <ε, stop; otherwise, proceed with 
iteration k + 1 of the PD method. The tolerance ε is typically a small number such 
as 1e-06. If convergence is reached, µk and σk are the parameter estimates of µ and 
σ. Similarly, Zi 
(k)
s (or, Zi
(k+1)s) could be used as the unconstrained values of zi s, i ≤ 
M.
To illustrate how the PD algorithm works in practice, reconsider the data provided 
in panel A of Table 5.9. Irrespective of how aggressive we would like the unconstrain-
ing to be, we always initialize µ and σ to be the sample mean and the sample standard 
deviation (corrected for the degrees of freedom) of all unconstrained observations. This 
means that µ0 and σ0 are always 8.667 and 1.528, respectively. For a τ of 0.50, the E-
like step at iteration 1 replaces all observations  zi, 1≤ i ≤3, constrained at bi = 10 with 
a Zi
(1) of 10.662 (for a normally distributed random demand variable X~N(µ0, σ0 
2) 
with a probability density function f(x) and a cumulative distribution function F(x),
Bf x d x F Z
Z
i
i
= () =− ( ) =
()
+∞
()
∫
1
1 0 09571 . , AB f x d x F b
b
i
i
+= () =− () =
+∞
∫ 1 0 1914 .  and, 
hence, B/(A + B) = τ= 0.50). With this imputation in place, the M -like step at iteration 
1 updates the parameter estimates for µ and σ such that µ1 = 9.664 and σ1 = 1.459. At 
iteration 2, we replace in the E-like step all the constrained observations  zi, 1 ≤ i ≤ 3, 
with a Z i
(2) of 10.869 (for X~N(µ1,σ1
2), Bf x d x F Z
Z
i
i
= () =− ( ) =
()
+∞
()
∫
2
1 0 20452 . , 
AB f x d x F b
b
i
i
+= () =− () =
+∞
∫ 1 0 4090 . , and, hence, B/(A + B) = τ = 0.50) and revise in
the M-like step the parameter estimates for µ and σ such that µ2 = 9.768 and σ2 = 1.545. 
We then repeat the E- and M-like steps several times such that upon convergence, at 
iteration 18, Zi
(18) =11.039 and µ = µ18 = 9.853 and σ = σ18 = 1.619. For convenience, we 
summarize these steps together with those undertaken for τ values of 0.40 and 0.25 in 
Table 5.14. As it is readily apparent from this table, smaller τ values guarantee a more 
aggressive unconstraining but this typically comes with a significantly higher compu-
tational effort. For example, for a τ of 0.25, the convergence is reached after 184 itera-
tions which, for a tolerance ε of 1e-06, is a tenfold increase over the number of itera-
tions required to reach convergence for a τ of 0.50. To illustrate how we computed the 
Zi
(k)'s presented in Table 5.14 , we emphasize again the fact that these figures are not 
.

---

## Page 143

132  Unconstraining
dependent on how the E-like step has been executed, that is, the numeric procedures and 
our proposed methodology suggest identical results.
Returning to our running example that builds on the Pain de Boulogne data provided 
in Table 5.1, we apply the PD method to the end-of-the-day sales values to estimate the 
parameters µ and 
σ of the underlying normal demand distribution. For a τ value of 0.35 
(which we chose at random), we summarize the PD iterations in terms of Zi
(k), µk, and σk 
in Table 5.15. The corresponding results tell a story similar to that of the EM algorithm. 
In essence, while the parameter estimates for µ and 
σ are consistent with those suggested 
by the other unconstraining techniques, the final unconstrained values Zi
(k) seem to be 
amiss. As with the EM algorithm, the fact that the PD method treats time-dependent 
information as if it were time independent leads to situations where the Z
i
(k)s appear to 
inaccurately over- or under-forecast the corresponding true demand realizations (e.g., 
days 4 and 13 and days 10 and 15, respectively). To this end, the unconstraining per-
formance of the PD method should be judged based on the requirements of each specific 
application (i.e., demand parameters vs. unconstrained demand values). In addition 
to this perceived drawback, another aspect that some authors have expressed concerns 
about relates to how one should go about setting the right 
τ values. In simulation stud-
ies for the airline industry intended to assess how well the PD method recovers the true 
parameters of some demand distributions, Weatherford and Pölt (2002), for example, 
report results specific to the degree of constraining induced in the synthetic data sets. 
For the lightly constrained regimes, the PD method with 
τ values of 0.50, 0.40, and 0.30 
seems to recover equally well the parameters of the true demand distributions. In heavily 
constrained regimes, however, some of the 
τ values underestimate (e.g., τ = 0.50) and 
some overestimate (e.g., τ = 0.30) the true hypothetical demand parameters. In a simi-
lar environment but targeting the revenue performance in competitive settings, Zickus 
(1998) investigates the effectiveness of the PD method with 
τ values of 0.35, 0.25, and 
0.15. His results are also inconclusive as the revenue performance appears to not only 
be dependent on the PD method and its 
τ values but also on the other critical compo-
nents of a revenue management system (i.e., the forecasting engine and the capacity 
controls). Given that no magic numbers for 
τ exist, we remind the reader that τ is a user-
specified “best-guess” about the conditional probability that one underestimates the 
Table 5.14 Operationalization of the PD Method for Demand Unconstraining
/H9270 = 0.50 /H9270 = 0.40 /H9270 = 0.25
i z i 
zi /Zi
(k) at iteration zi /Zi
(k) at iteration zi /Zi
(k) at iteration
1 2 … 18 1 2 … 28 1 2 … 184
1 10* 10.662 10.869 … 11.039 10.849 11.194 … 11.697 11.212 11.920 … 18.023
2 10* 10.662 10.869 11.039 10.849 11.194 11.697 11.212 11.920 18.023
3 10* 10.662 10.869 11.039 10.849 11.194 11.697 11.212 11.920 18.023
47 7 7 7 7 7 7 7 7 7
51 0 1 0 1 0 1 0 1 0 1 0 1 0 1 0 1 0 1 0
69 9 9 9 9 9 9 9 9 9
µ
k = 8.667 9.664 9.768 … 9.853 9.758 9.930 … 10.182 9.939 10.293 … 13.345
σk = 1.528 1.459 1.545 1.619 1.537 1.688 1.920 1.696 2.027 5.215
Legend:   * identifies constrained demand observations.

---

## Page 144

Unconstraining  133
unconstrained demand given that the demand is in fact constrained. To this end, some 
experimentation, common sense or both are needed to select a τ value for a sensible PD 
unconstraining performance.
SUMMARY
In this chapter, we address the important topic of demand unconstraining which 
involves the estimation of the true demand distribution parameter values from historical 
sales data that are censored due to capacity or inventory constraints. The science behind 
demand unconstraining was primarily developed for the travel and hospitality industries 
but is increasingly being used in other environments such as the retail industry. In prac-
tice, virtually all industries including retail face demand-censoring problems that one 
way or another need to be handled appropriately to avoid major business decisions being 
made based on misleading data. Some of the techniques and applications we discuss here 
are, to the best of our knowledge, still open (research) questions for which consensus 
Table 5.15 Demand Unconstraining via the PD Method τ=0.35
t z i 
zi/Zi
(k) at iteration Unconstrained Demand
1 2 3 … 68 PD(a) EM(a) DES(b) AM(b) Table 5.5(c)
1 40 43.78 46.30 48.08 … 54.22 54.22 51.45 62 45 55
2 40 43.78 46.30 48.08 54.22 54.22 51.45 63 53 65
3 40 43.78 46.30 48.08 54.22 54.22 51.45 47 43 46
4 40 43.78 46.30 48.08 54.22 54.22 51.45 44 41 43
5 40 43.78 46.30 48.08 54.22 54.22 51.45 63 53 67
63 1 3 1 3 1 3 1 3 1 3 1 3 1 3 1 3 1 3 1
7 40 43.78 46.30 48.08 54.22 54.22 51.45 57 48 57
82 0 2 0 2 0 2 0 2 0 2 0 2 0 2 0 2 0 2 0
93 1 3 1 3 1 3 1 3 1 3 1 3 1 3 1 3 1 3 1
10 40 43.78 46.30 48.08 54.22 54.22 51.45 69 53 65
11 23 23 23 23 23 23 23 23 23 23
12 39 42.99 45.71 47.57 53.83 53.83 50.89 43 39 40
13 31 37.54 42.43 44.72 51.57 51.57 47.19 34 32 33
14 40 43.78 46.30 48.08 54.22 54.22 51.45 55 42 45
15 40 43.78 46.30 48.08 54.22 54.22 51.45 75 54 78
16 39 39 39 39 39 39 39 39 39 39
17 23 34.38 41.37 43.76 50.61 50.61 44.96 27 26 26
18 39 39 39 39 39 39 39 39 39 39
19 40 43.78 46.30 48.08 54.22 54.22 51.45 45 40 41
20 31 31 31 31 31 31 31 31 31 31
µ 30.57 38.34 40.32 41.54 … 45.61 45.61 43.58 44.90 39.20 41.20
σ 7.21 7.50 8.49 9.27 12.06 12.06 12.57 16.00 10.20 11.70
(a) The unconstrained demand values are not rounded up to the closest integer because µ and σ reflect the raw numeric 
values. (b) The reported standard deviation σ is corrected for the degrees of freedom. (c) µ and σ are the mean and stand-
ard deviation of the corresponding Gumbel distribution.
Figures shown in bold and italic represent constrained sales values. 
For consistency and clarity, we present the PD results ordered by t (vs. the index i which we use to describe the PD 
algorithm).

---

## Page 145

134  Unconstraining
agreements are still unavailable. Hence, we hope that our digression will resonate with 
researchers and industry practitioners alike and build some momentum around solving 
these problems adequately.
In the second part of this chapter, we present the details of unconstraining techniques 
that apply to both single- and multi-period items. We demonstrate the Product-Limit 
technique in conjunction with hourly sales data (or, to a certain degree, subjective prob-
ability elicitation techniques) to compute the parameters of the true demand functions 
of severely censored single-period items. We further employ the averaging method, the 
double exponential smoothing technique, the expectation-maximization algorithm and 
the projection detruncation method to explore the intricacies of unconstraining sales 
data for multi-period items. Our differentiation of the unconstraining techniques based 
on the item type is a technicality; in practice, all techniques could be applied to both 
single- and multi-period items.
It is our expectation that after going through this chapter, the reader should be able to:
1. Understand why demand unconstraining is needed and how it relates to the other 
areas of revenue management and pricing.
2. Understand the intricacies of some of the most common demand unconstraining 
techniques.
3. Employ unconstraining techniques to compute the parameters of the true demand 
distributions.
REFERENCES
Agrawal, N., & Smith, S. A. (1996). Estimating negative binomial demand for retail inventory management with 
unobservable lost sales. Naval Research Logistics, 43(6), 839–861.
Anupindi, R., Dada, M., & Gupta, S. (1998). Estimation of consumer demand with stock-out based substitution: 
An application to vending machine products. Marketing Science, 17(4), 406–423.
Åžen, A. (2008). The US fashion industry: A supply chain review. International Journal of Production Economics, 
114(2), 571–593.
Boyles, R. A. (1983). On the convergence of the EM algorithm. Journal of the Royal Statistical Society. Series B 
(Methodological), 45(1), 47–50.
Chesley, G. R. (1975). Elicitation of subjective probabilities: A review. The Accounting Review, 50(2), 325–337.
Chesley, G. R. (1978). Subjective probability elicitation techniques: A performance comparison. Journal of Account-
ing Research, 16(2), 225–241.
Chopra, S., & Meindl, P. (2012). Supply chain management: Strategy, planning and operation (5th ed.). Upper 
Saddle River, NJ: Pearson/Prentice Hall.
Conlon, C., & Mortimer, J. H. (2008). Demand estimation under incomplete product availability. Working Paper. 
Cooper, W. L., Homem-de-Mello, T., & Kleywegt, A. J. (2006). Models of the spiral-down effect in revenue man-
agement. Operations Research, 54(5), 968–987.
Crowder, M. J., Kimber, A., Sweeting, T., & Smith, R. (1991). Statistical analysis of reliability data. London: Chap-
man & Hall/CRC.
Dempster, A. P., Laird, N. M., & Rubin, D. B. (1977). Maximum likelihood from incomplete data via the EM algo-
rithm. Journal of the Royal Statistical Society. Series B (Methodological), 39(1), 1–38.
Fisher, M. L., & Raman, A. (2010). The new science of retailing: How analytics are transforming the supply chain and 
improving performance. Boston, MA: Harvard Business School Press.
Gorin, T. O. (2000). Airline revenue management: Sell-up and forecasting algorithms. Unpublished MS Thesis, 
Massachusetts Institute of Technology, Cambridge, MA.
Guo, P., Xiao, B., & Li, J. (2012). Unconstraining methods in revenue management systems: Research overview 
and prospects. Advances in Operations Research, 2012 (Article ID 270910).
Hofman, M. (2012). Size level stock-outs in fashion retailing. Unpublished MS thesis (Research Proposal; 
Undefended MS thesis), University of Groningen, Faculty of Economics and Business, Groningen, the 
Netherlands.

---

## Page 146

Unconstraining  135
Hopperstad, C. (1997). Projection detruncation. Renton, WA: Boeing Company Memo.
Hopperstad, C., Belobaba, P. P., & Skwarek, D. K. (1996). Passenger O/D simulator update. AGIFORS Reservations 
and Yield Management Study Group, AGIFORS, Zurich, Switzerland.
Jackson, C. (2011). Multi-state models for panel data: The msm package for R. Journal of Statistical Software, 38(8), 
1–28.
Kahneman, D., & Tversky, A. (1979). Intuitive prediction: Biases and corrective procedures. TIMS Studies in Man-
agement Science, 12, 313–327.
Kaplan, E. L., & Meier, P. (1958). Nonparametric estimation from incomplete observations. Journal of the Ameri-
can Statistical Association, 53(282), 457–481.
Kök, A. G., & Fisher, M. L. (2007). Demand estimation and assortment optimization under substitution: Method-
ology and application. Operations Research, 55(6), 1001–1021.
Lariviere, M. A., & Porteus, E. L. (1999). Stalking information: Bayesian inventory management with unobserved 
lost sales. Management Science, 45(3), 346–363.
Lau, H., & Lau, A. H. (1996). Estimating the demand distributions of single-period items having frequent stock-
outs. European Journal of Operational Research, 92(2), 254–265.
Lau, H., Lau, A. H., & Kottas, J. F. (1999). Using Tocher’s curve to convert subjective quantile-estimates into a 
probability distribution function. IIE Transactions, 31(3), 245–254.
Lawless, J. (2003). Statistical models and methods for lifetime data  (2nd ed.). Hoboken, NJ: John Wiley & Sons, 
Inc.
Mozenda. (2012). Retrieved February 1, 2012, from www.mozenda.com/.
Nelson, W. B. (2004). Applied life data analysis. Hoboken, NJ: John Wiley & Sons, Inc.
Osika, J. (2012). Size level availability—The Achilles heel of apparel retailing. Unpublished MS thesis, University 
of Groningen, Faculty of Economics and Business, Groningen, the Netherlands.
Pezzo, M. V., Litman, J. A., & Pezzo, S. P. (2006). On the distinction between yuppies and hippies: Individual 
differences in prediction biases for planning future tasks. Personality and Individual Differences, 41(7), 
1359–1371.
Queenan, C. C., Ferguson, M., Higbie, J., & Kapoor, R. (2007). A comparison of unconstraining methods to 
improve revenue management systems. Production and Operations Management, 16(6), 729–746.
Redner, R. A., & Walker, H. F. (1984). Mixture densities, maximum likelihood and the EM algorithm. SIAM 
Review, 26(2), 195–239.
Saleh, R. (1997). Estimating lost demand with imperfect availability indicators. AGIFORS Reservations and Yield 
Management Study Group, AGIFORS, Montreal, Canada.
Skwarek, D. K. (1996). Revenue and traffic impacts of alternative detruncation methods. AGIFORS Reservations 
and Yield Management Study Group, AGIFORS, Zurich, Switzerland.
Smith, J. Q. (2010). Bayesian Decision Analysis. Cambridge, UK: Cambridge University Press.
Swan, A. V. (1969). Maximum likelihood estimation from grouped and censored normal data.  Applied Statistics, 
18(1), 110–114.
Tan, B., & Karabati, S. (2004). Can the desired service level be achieved when the demand and lost sales are unob-
served? IIE Transactions, 36(4), 345–358.
Tocher, K. D. (1963). The art of simulation. London, UK: Hodder and Stoughton.
Venables, W. N., & Ripley, B. (2002). Modern applied statistics with S (4th ed.). New York, NY: Springer.
Weatherford, L. R. (2000). Unconstraining methods. AGIFORS Reservations and Yield Management Study Group, 
AGIFORS, New York, NY.
Weatherford, L. R., & Pölt, S. (2002). Better unconstraining of airline demand data in revenue management sys-
tems for improved forecast accuracy and greater revenues.  Journal of Revenue & Pricing Management,  1(3), 
234.
Wolynetz, M. S. (1979). Algorithm AS 138: Maximum likelihood estimation from confined and censored normal 
data. Journal of the Royal Statistical Society. Series C (Applied Statistics), 28(2), 185–195.
Wright, W. F. (1988). Empirical comparison of subjective probability elicitation methods. Contemporary Account-
ing Research, 5(1), 47–57.
Wu, J. (1983). On the convergence properties of the EM algorithm. The Annals of Statistics, 11(1), 95–103.
Zeni, R. H. (2001a). Improved forecast accuracy in revenue management by unconstraining demand estimates 
from censored data. Unpublished PhD thesis, Rutgers University, Newark, NJ.
Zeni, R. H. (2001b). Improving forecast accuracy by unconstraining censored demand data. AGIFORS Reserva-
tions and Yield Management Study Group, AGIFORS, Bangkok, Thailand.
Zickus, J. S. (1998). Forecasting for airline network revenue management: Revenue and competitive impacts. 
Unpublished MS thesis, Massachusetts Institute of Technology, Cambridge, MA.

---

## Page 147

6
PRICING ANALYTICS
INTRODUCTION
How do managers in a firm decide on the prices to charge for the products or services 
they sell? For some firms, the pricing decision is made at the top level of the manage-
ment team with little flexibility for the sales force, marketing team, or supply chain part-
ners (distributors or retailers) to make adjustments. Apple’s fixed pricing for its popular 
iPhone and iPad products is a good example of this practice. For other firms, it may 
appear to the customer that pricing is left entirely up to the individual sales person. This 
happens frequently in the business-to-business (B2B) market, such as the pricing for a 
major software implementation by a software vendor or consulting company. The price 
quoted for a new car from a dealership is an example from the business-to-consumer 
(B2C) market. Even in these situations, however, there is almost always some price guid-
ance provided by a division level or corporate pricing team. Thus most large firms have 
some department or team whose primary responsibility is to determine the price, or 
price range, to charge for the firm’s products. The group may reside under many differ-
ent branches of the corporate organizational structure, such as marketing, operations, or 
finance and its members may or may not have pricing in their job titles. It is also com-
mon for this group of professionals to have access to some historical pricing and sales 
data, even if this information is not currently being used in the price-setting process.
Pricing analytics involves the use of historical data to determine the best prices to set for 
future sales. In this chapter, our focus is on both the theory and the practice of pricing ana-
lytics,
1 where we restrict our discussion to the setting of a base price for a single product. 
An example would be the regular price to charge for a nonperishable product sold through 
a retail store. We cover more specific applications of pricing analytics such as dynamic 
pricing, markdown pricing, and customized B2B pricing in later chapters. We also save 
our discussion of the important topic of behavioral responses to pricing for a later chapter. 
While it is often difficult to apply the techniques described in the introductory sections of 
this chapter directly, a good understanding of the theory behind pricing analytics is crucial 
to successful applications of the techniques described later in the book.
136

---

## Page 148

Pricing Analytics  137
THE MICROECONOMISTS’ VIEW OF CONSUMER-PURCHASING 
DECISIONS
What makes a consumer decide to purchase a product or to choose one product 
over all the other alternatives? Economists use the term ‘consumer utility’ to represent 
the value that a particular product or service provides to a customer. Utility is often 
represented in monetary values. For example, at a particular point in time, a consumer 
may derive a utility of $1 for a can of Coca-Cola and a utility of $0.90 from a can of 
Pepsi.
Willingness-to-Pay
Another term that is commonly used in the pricing field is the consumer’s maximum 
willingness-to-pay (WTP), or the maximum price at which the consumer would 
buy a good. Often, consumer utility and willingness-to-pay are terms that are used 
interchangeably. Thus if the consumer is at a store that only sells cans of Coca-Cola, 
microeconomic theory says that the consumer will purchase a can if the price is less 
than or equal to $1 (we are assuming away budget constraints in this example, i.e., 
the consumer is not prohibited from purchasing the product because of budgetary 
constraints). If the store sells cans of both Coca-Cola and Pepsi, then the consumer 
will purchase the brand that maximizes her remaining utility after subtracting the 
purchase price. For example, if a can of Coca-Cola is priced at $0.75 but a can of 
Pepsi is $0.50, then the customer purchases the can of Pepsi because ($1 – $0.75) 
< ($0.90 – $0.50).
Consumer Search Cost
In addition to a side-by-side comparison of the prices of different brands of a particular 
product, consumers are often aware that alternative brands or prices are available at 
other locations or through other channels. In the previous example, we assumed that 
the consumer will purchase one of the brands of soda from the store she is currently in. 
Suppose, however, that the consumer knows that the store across the street sells cans of 
Pepsi for $0.40. Will the consumer delay the purchase of a can of soda and cross the street 
to save an extra $0.10? To answer this question, economists have defined a “search cost” 
to represent the hassle of searching and purchasing the product from another location 
or source. Thus the consumer will still purchase the can of Pepsi from the store as long 
as ($0.90 – $0.50) > ($0.90 – $0.40 – search cost).
What makes pricing challenging is that a particular customer’s utility for products 
may change over time depending on factors such as the season, the weather, the overall 
economic climate, or the current competitive environment in the industry. In addition, 
different consumers typically have different WTPs and different search costs (termed 
‘heterogeneous customers’ in the economics literature), and we seldom have the capabil-
ity to set a personalized price for each specific consumer. Even if we did have the capabil-
ity to set customized prices for each specific consumer, they do not make it a practice to 
tell us what their utilities are for our products. This is rational; consumers recognize that 
firms that know their maximum WTP for a product could, theoretically, set a specific 
price for each consumer equal to that consumer’s maximum WTP. Thus the practice of 
pricing analytics has evolved to improve upon historical pricing performance while tak-
ing into account the realities mentioned earlier.

---

## Page 149

138  Pricing Analytics
THE PRICING ANALYTICS PROCESS
Pricing analytics is an iterative process using historical price/demand data to adjust the 
price of a product in order to maximize profits by analyzing the trade-off between price, 
volume, and cost. In general, the field has moved toward the term ‘price analytics’ and 
away from the term ‘price optimization’ because optimization implies that it is pos-
sible to analytically determine the single price that will maximize profits with a reason-
able degree of confidence. In practice, there is always uncertainty about whether a given 
price is the “right” price. Still, approximating the optimal price is the goal. Determining 
the profit-maximizing price requires a combination of analytical rigor and managerial 
judgment to understand the trade-offs among prices, costs, and customer response. An 
overview of this process is shown in Figure 6.1.
The approach behind pricing analytics is to formulate pricing problems as constrained 
optimization problems that can be solved by standard techniques. The following ele-
ments are required:
 A price-response function that describes how customers are expected to respond to 
our pricing actions.
 An objective function that specifies what we are trying to achieve (maximize prof-
its, meet a market share target, etc.).
 A set of constraints that limit what we can do (capacity, capital, margin, etc.).
The goal of pricing analytics is to provide the right price for every product, for every cus-
tomer segment, through every channel. For example, it may be better to set a different 
price for a large-revenue customer in the Northwest who orders from the firm directly 
Historical 
Price/Demand 
Data
Segment 
the Market
Estimate
Competing Price
Response Models
Choose the
Best Model
Optimize
the Price
Execute
Pricing
Monitor and 
Evaluate 
Performance
Set Objective
Function and
Constraints
Figure 6.1 The Pricing Analytics Process.

---

## Page 150

Pricing Analytics  139
than for a smaller customer in the Northeast who orders through a distributor. Some 
banks will even quote different interest rates to the same customer if she arrives via an 
online search versus in person at the local branch office. The first step before determin-
ing a profit-maximizing price, however, is to determine how customers will react to a 
price change. This involves the estimation of price-response functions from historical 
price/demand data.
Historical Price/Demand Data
The data typically used in a pricing analytics process are historical transaction data that 
show how much demand occurred for a given time period, a given location, and a given 
price. Care must be taken to ensure the accuracy of this data set before beginning the pric-
ing analytics process. For example, the data set should be tested for outliers (data points 
that appear to be statistical anomalies) and each identified outlier should be investigated 
to determine if it should remain in the data set. In addition, there is often an issue with an 
incomplete data set or missing values. There is a long history of research on how to test 
for outliers and how to handle missing values in statistical estimation projects. Finally, 
the price/demand data that most firms have available is sales data, not demand data. This 
happens when the product is out of stock and demand for the product during the time 
it is out of stock is not recorded. In such cases, the demand data must be unconstrained 
before it can be used to estimate price-response functions. Since data integrity is not a 
focus of this book, we simply offer a warning to the reader to plan on spending a signifi-
cant portion of the project duration simply extracting, cleaning, and unconstraining the 
data sets. Additional types of data used for pricing analytics are detailed in Table 6.4.
Estimating and Choosing the Best Price-Response Models
After the historical price/demand data has been extracted and evaluated as a good repre-
sentation of past consumer demand, it can be used to estimate alternative price-response 
functions. The reason for estimating alternative functions is because we do not know, 
a priori, which price-response function provides the best representation of consumer 
demand. The estimation and evaluation of price-response functions is a major compo-
nent of this book.
Set Objective Function and Constraints and Optimize the Price
Once a price-response function has been estimated and an objective function and con-
straints are set, the optimization of the price for each specific market segment is typically 
straightforward. An optimal price is defined as the price (or set of prices) that results in 
the best value of the objective function while the required resources needed to achieve 
the objective function value remain within the limits specified by the model constraints. 
A common example of an objective function with constraints is when a firm seeks to find 
the price that maximizes profits (objective function) given a specific amount of inven-
tory available (constraint).
Execute Pricing
While it may appear that price execution is a trivial piece of the pricing analytics process, 
it is often the step where pricing projects break down in practice. A firm may perform 
exceptionally well on each of the other steps in the process, but if the right prices are not 
presented to the right set of consumers in the right way, then the entire pricing analytics

---

## Page 151

140  Pricing Analytics
process will fail to deliver its projected value. While price execution is not a focus of this 
book, its importance cannot be overestimated.
Monitor and Evaluate Performance
As Figure 6.1  shows, market feedback occurs at two levels. The most immediate feed-
back is the analysis of alternatives. Here, the effects of the most recent actions should be 
monitored so that immediate action can be taken if necessary. The second level of feed-
back updates the parameters of the price-response functions. If the sales of some prod-
ucts are slower than expected, it may indicate that the market is more price responsive 
than expected and the future market-response curve for that product should be adjusted 
accordingly. 
Now that we have briefly explained each of the steps in the pricing analytics process, 
we next take a deeper look at the price-response functions that serve as the backbone of 
the price optimization endeavor.
THE PRICE-RESPONSE FUNCTION
As previously discussed, the first step in the pricing analytics process is to collect the 
historical price/demand data for the product of interest. Using this historical data, the 
price-response function can be estimated using econometric techniques such as linear or 
nonlinear regression. The price-response function specifies demand for the product of 
a single seller as a function of the price offered by that seller (Figure 6.2). This contrasts 
with the concept of a market demand curve, which specifies how an entire market will 
respond to changing prices. The distinction is critical because different firms competing 
in the same market face different price-response functions that are the result of many 
factors, such as the effectiveness of their marketing campaigns, customer-perceived dif-
ferences in quality, product differences, and location. Hence, the price-response func-
tion may be different even for the same product if the product is sold through different 
channels or outlets.
0
500
250
0
750
1000
5 10 2015
Price ($)
Demand
Figure 6.2 Linear Price-Response Function.

---

## Page 152

Pricing Analytics  141
In a perfectly competitive market, the price response faced by an individual seller is a 
vertical line at the market price. If the seller prices above the market price, her demand 
drops to zero. If the seller prices below the market price, her demand is equal to the 
entire market. In a perfectly competitive market, the seller has no pricing decision—the 
price is set by the operation of the larger market.
The price-response functions that most companies face are not necessarily linear over 
the entire price range as shown in Figure 6.2 , but they do demonstrate some degree 
of smooth price response over the entire range of possible prices. As price increases, 
demand declines until it reaches zero at some satiating price. As price decreases, the 
demand approaches the maximum market size for that product and location.
Choosing the Best Price-Response Function
When choosing a price-response function to fit to the historical price/demand data, you are 
implicitly making assumptions about customer behavior. It is worthwhile understanding 
these assumptions so that we can judge which candidate price-response function is appro-
priate for the application. The most important of these assumptions involves the distri-
bution of the consumers’ WTP. For pricing analytics, we assume that consumers’ WTP 
has a known distribution, w(x), across the entire population of consumers. Exactly how 
consumers’ WTP is distributed across the potential customer population is an important 
decision in the pricing analytics process. Figure 6.3 shows a distribution of WTP where 
consumers are evenly distributed across the entire range of possible prices. Here, P is the 
maximum price consumers are willing to pay for the product/service they are requesting.
Note that 0 ≤ w (x) ≤ 1 for all nonnegative values of the price  x. Let D = d(0) be the 
maximum demand achievable. In concrete terms, D is the demand expected to material-
ize at a price of zero and reflects the total market size. We can derive the price-response 
function, d(p), from the WTP distribution via
d(p) = the demand expected to materialize at a price p
 = the number of people who have a WTP greater than the price p
 = D* the area of the WTP distribution to the right of price p
 =  D · ∫
P
pw(x)dx.
For the uniform WTP distribution shown in Figure 6.3 , the fraction of the 
population with WTP ≥ p is ( P–p)·(1/ P), or, 1–p/P  (see Figure 6.4). In formal terms, 
0
w(x) = 1/P for 0≤x≤P
Price
w(p)
0
P
1/P
Figure 6.3 Uniform WTP Distribution.

---

## Page 153

142  Pricing Analytics
wxd x P dx P x P Pp p P
p
P
p
P
p
P
() == ⋅ = ⋅ − () =−∫∫
11 1 1 . Thus the total population with WTP 
≥ p is d(p) = D – D— P  . p.
It is important to understand what an assumption about the underlying consumer 
WTP distribution implies. For the uniform WTP distribution depicted in Figure 6.3 and 
6.4, this choice of distribution requires that an equal percentage of the total consumer 
population is willing to purchase a product at every possible price point. If we used this 
distribution for our Coca-Cola example, and the maximum that anyone is willing to pay 
for a can of Coke is $5, then a uniform distribution implies that there are just as many 
consumers who are willing to pay, but will pay no more than, $5 for a can of Coke as 
there are consumers who will pay, but will pay no more than, $1. This is probably not 
the case for the general population. Most of us would fall in some middle range of WTP 
rather than be evenly distributed over a broad range of possible prices. Thus perhaps a 
more plausible WTP distribution assumption is one that groups the largest percentage 
of the consumers around some mean value, placing very small probabilities at the low- 
and high-end extremes. Such a distribution is often called a bell-curve distribution as 
shown in Figure 6.5. The reason it is called a bell-curve distribution is because the graph 
0
Fraction of the Population with WTP ≥ p 
Price
w(p)
0
Pp
1/P
Figure 6.4 Density of Demand at Price p from a Uniform WTP Distribution.
Price
0
0
w(p)
0.05
0.1
0.15
0.2
pP
Fraction of the Population with WTP ≥ p 
Figure 6.5 Density of Demand at Price p from a Normal WTP Distribution.

---

## Page 154

Pricing Analytics  143
of its probability density function looks like a bell. The normal distribution is the most 
common of the bell-shaped distributions. If P and p were $20 and $10, respectively, one 
could interpret the WTP distribution shown in Figure 6.5 as saying that there are few 
consumers with a maximum WTP of $15 or more for the product represented. However, 
there is a large percentage of the consumer population with a maximum WTP between 
$5 and $15.
Now that we have explored a few WTP distribution assumptions, we can explain how 
the choice of a WTP distribution results in different price-response functions.
Common Price-Response Functions
Choosing and estimating the right price-response function is arguably the most difficult 
part of any pricing analytics project. In what comes next, we present four commonly 
used price-response functions. In later sections, we discuss how to estimate these func-
tions and how to judiciously select the one that serves the project’s needs best.
Linear Price-Response Function
The linear price-response function shown in Figure 6.6 can be represented by the same 
familiar equation used for linear regression:
 d (p) = D + m . p, (6.1)
where D represents the intercept term, p is the independent price variable, and m = –D/P 
< 0 is the slope for 0 ≤ p ≤ P. It is commonly used in practice mainly because it is easy to 
estimate by applying simple linear regression on the historical price/demand data.
Constant-Elasticity Price-Response Function
A second commonly used price-response function is the constant-elasticity function, 
which has a point elasticity (defined in the next section) that is the same at all prices. It is 
based on an exponential WTP distribution. The price-response function is:
D = d(0)
d(p)
Demand
Price
0
0 P = −D/m
Figure 6.6 Linear Price-Response Function.

---

## Page 155

144  Pricing Analytics
 d(p) = C . pε (6.2)
where C > 0 and ε < 0 are parameter values that are estimated by fitting equation (6.2) 
to the price/demand data. Some sample constant-elasticity price-response functions are 
shown in Figure 6.7.
Both linear and constant-elasticity price-response functions are useful for local 
demand estimation but are often not realistic global price-response models. When glo-
bal demand estimation over the entire range of prices is needed, we need a function that 
is based on the bell-curve WTP distribution shown in Figure 6.5. The price-response 
function that results from a bell-curve WTP distribution has a reverse S-shape, as shown 
in Figure 6.8.
For price-response curves with a reverse S-shape, there are diminishing returns when 
making large price decreases, as can be seen by the flatness of the curve in Figure 6.8 for prices 
on the left side of the graph. Similarly, the curve is flat for relatively high prices. Changes in 
price in the middle range, however, often results in significant changes in demand. One way 
0.2
60
30
0
90
120
1.1 2.0
Price ($)
Demand (thousands)
є = −0.5 є = −1.0 є = −2.0
Figure 6.7 Constant-Elasticity Price-Response Functions (C = 5,000).
0.0
50
25
0
75
100
0.5 1.0 2.52.01.5
Price ($)
Demand
Figure 6.8 Reverse S-Shaped Price-Response Function.

---

## Page 156

Pricing Analytics  145
to think about this is to imagine the population of Coca-Cola and Pepsi drinkers. There is 
a small segment of very loyal Pepsi or Coca-Cola drinkers that will not consider the other 
brand for any difference in price (the extreme left or right parts of the curve), while there is 
a larger segment of consumers that will change their purchase decision between the two if 
the price difference is large enough (the middle section of the curve). We will cover two of 
these reverse S-shaped functions here, the power and the logit functions.
Power Price-Response Function
The power price-response function is one function with the reverse S-shape:
 d (p) = 
α . D / (pβ + α) (6.3)
where D > 0, α > 0 and β >0 are parameter values estimated by fitting equation (6.3) to 
the price/demand data. The power price-response function is shown for different values 
of β in Figure 6.9. Higher values of β represent more price-sensitive markets. As β grows 
larger, the market approaches the perfectly competitive price-response function. Differ-
ent values of 
α, α >0, shift the curves left and right along the horizontal price-axis.
Logit Price-Response Function
The second common price-response curve that has a reverse S-shape functional form is 
the logit function:
 dp Ce
e
ab p
ab p() = ⋅
+
+⋅
+⋅1
, (6.4)
where C >0, α, and b >0 are parameter values that are estimated by fitting equation 
(6.4) to the price/demand data. The shape of the logit function is similar to the shape of 
the power functions shown in Figure 6.9. One advantage the logit function has over the 
power function is that it can be estimated using logistics regression, a methodology that 
is commonly available in most statistical software packages. Table 6.1 summarizes the 
commonly used price-response functions.
0.0
D = 100, α = 1
50
25
0
75
100
0.5 1.0 2.0 2.51.5
Price ($)
Demand
β = 2 β = 5
β = 10 β = 20
Figure 6.9 Power Price-Response Function.

---

## Page 157

146  Pricing Analytics
The most useful feature of price-response functions is that, once estimated, they can 
be used to determine the price sensitivity of a product or how demand will change in 
response to a change in price. In the next section, we look at some ways that price sensi-
tivity is measured.
MEASURES OF PRICE SENSITIVITY
Once we have some historical price and demand data, the pricing analytics process 
described in Figure 6.1 shows that the next steps are to segment the market and to esti-
mate the market response. The market response is typically estimated by measuring how 
a change in the price of a product results in a change in demand. Similarly, segmenting 
the market refers to finding different consumer attributes where consumers with similar 
attributes have the same (or similar) price/demand responses.
Estimating the market response and determining if different consumer segments 
have different responses require some measure of how demand changes with price. The 
simplest measurement is to take the slope of the price-response function at some given 
price. The slope, defined as the change in the y -axis divided by the change in the x -axis, 
measures the local rate of change of the price-response function at a particular price 
(price p in Figure 6.10). The slope of the price-response function is always negative and 
can be measured for a continuous price-response function by taking its derivative. If we 
denote the price-response function by d(p), a reasonable local estimator of the change 
in demand that would result from a small change in price (changing the price from p
1 
to p2) is
d(p2) – d(p1) ≈ d'(p1) . (p2 – p1),
Change in demand ≈ slope change in price,
where d'(p) represents the derivative of the price-response function with respect to price 
computed at price p. For example, the price-response function in Figure 6.2 can be rep-
resented by
d(p) = 10,000 – 500 . p.
Table 6.1 Price-Response Functions
Price-Response Function Formula WTP Distribution
Linear d(p) = D + m . p
(D > 0, m < 0) Uniform
Constant Elasticity d (p) = C . pε 
(C > 0, ε < 0) Variant of a Power-Law 
Distribution
Power
d (p) =  α . D
 Pβ + α
(D > 0, α > 0, β > 0 
Weibull
Logit
d (p) = C . ea+b . p
 1 + ea+b . p
(C > 0, b < 0) 
Logistic

---

## Page 158

Pricing Analytics  147
The maximum WTP in this market is $20 and the maximum market size is 10,000. The 
slope of this function is –500, which can be found by taking the derivative: d'(p) = –500. 
A slope of –500 implies that a $1 increase in the product’s price results in a decrease in 
demand of 500 units. Thus an estimate of how much demand will decrease if we raise the 
price from $5 to $10 is –500 ($10–$5) or 2,500 units.
While the slope of the price-response function provides a useful measure of price sen-
sitivity, it has a major drawback. The slope of the price-response function depends on 
the units of measurement being used for both price and demand. Thus slope expressed 
in gallons/dollar will not be the same as in liters/euro. For this reason, the most common 
measure of price sensitivity used today is price elasticity. Price elasticity is defined as the 
ratio of the percentage change in demand to a percentage change in price. Formally, we 
can write
 
ε p p dp dp dp p p p
pd p d p
12 2 1 1 2 1 1
12 1
,() = () − ()() ()⎡⎣ ⎤
⎦ −
()⎡⎣ ⎤
⎦
=⋅
() − ( ) )()⎡⎣ ⎤
⎦ −
() ⋅ ()⎡⎣ ⎤
⎦
=− ⋅
() − ()() −⋅ ()()
pp d p
pd p d p p pd p
21 1
12 1 2 11 .
  (6.5)
Here, ε(p1, p2) is called the arc elasticity as it requires two prices to calculate. Thus the 
result will depend on both the old price p1 and the new price p2. An elasticity of –2 means 
that a 10% increase in price will result in a 20% decrease in demand and an elastic-
ity of –0.6 means that a 10% decrease in price will result in a 6% increase in demand. 
We can also derive a point elasticity at price p by taking the limit of equation (6.5) as p2 
approaches p1:
 ε(p) = p . d'(p)/d(p). (6.6)
The point elasticity is useful as a local estimate of the change in demand resulting from 
a small change in price.
p0
0
Max WTP
Slope of tangent line
Max 
Market
Size
Demand
Price ($)
Figure 6.10 Nonlinear Price-Response Function.

---

## Page 159

148  Pricing Analytics
Properties of Elasticity
 Always < 0. The downward-sloping property (the slope of price-response func-
tions is always negative) guarantees that demand always changes in the opposite 
direction from price. To this end, the minus sign on the right-hand side of equa-
tions (6.5), for example, guarantees that 
ε(p1, p2) is smaller than zero. 
 Independent of units. Elasticity of gasoline will be the same measured in gallons/$ 
or liters/euro. 
 Depends on the price at which it is measured.
 Low elasticity. |
ε|<1 means consumers are price insensitive.
 High elasticity. | ε|>1 means consumers are price sensitive.
 Depends on time period of measurement. For most products, short-run elasticity 
is lower than long-run elasticity because buyers have more flexibility to adjust to 
higher prices in the long run.
 Depends on level of aggregation (see Table 6.2).
 Industry elasticity may be low but individual product elasticity is always higher.
Table 6.3 and Figure 6.11 show some elasticities that have been estimated for vari-
ous goods and services at the industry level. Some products are very inelastic—salt, for 
example, is a relatively cheap commodity-type product and customers do not change the 
amount of salt they purchase very much in response to market price changes.
Table 6.2 Estimated Price Elasticities at the Industry and Brand Level
Product Elasticity
Soft drinks (Brownell et al., 2009) –0.80 to –1.00
Coca-Cola (Ayers & Collinge, 2004) –3.80
Mountain Dew (Ayers & Collinge, 2004) –4.40
Note: We refer the reader to the original authors’ work for more details 
on the conditions under which the price elasticities were estimated.
Table 6.3 Estimated Price Elasticities for Various Goods
Product Mean Median Number of observations Length of run
Petrol (Goodwin, Dargay, & Hanly, 2004) –0.25 46 Short run
Residential Electricity (Espey & Espey, 2004) –0.35 –0.28 123 Short run
Residential water (Dalhuisen, Florax, 
Groot, & Nijkamp, 2003)
–0.41 –0.35 314
–0.51 124
Beer (Fogarty, 2005) –0.46 –0.35 139
Cigarettes (Gallet & List, 2003) –0.48 523
–0.4 368 Short run
–0.44 155 Long run
Petrol (Goodwin et al., 2004) –0.64 51 Long run
Wine (Fogarty, 2005) –0.72 –0.58 141
Spirits (Fogarty, 2005) –0.74 –0.68 136
Residential Electricity (Espey & Espey, 2004) –0.85 –0.81 125 Long run
Branded products (Tellis, 1988) –1.76 337
Note: We refer the reader to the original authors’ work for more details on the conditions under which the price elasticities 
were estimated.

---

## Page 160

Pricing Analytics  149
Price elasticities will be different for different market segments. For example, price 
elasticities are generally higher for the same type of products for coupon users than that 
for nonusers.
The elasticity of the linear price-response function is m p/(D +m . p), which ranges from 
0 at p = 0 and approaches negative infinity as p approaches P» 0. The elasticity of the con-
stant-elasticity price-response function is constant for every price within the range of the 
function. The elasticity of the logit price-response function is b p/(1+ ea+b*p).
The Impact of Elasticity on Revenue
Knowing the elasticity of a product around a certain price point tells us something about 
how the revenue from the sales of that product will change with small price changes. In 
particular, if
 |
ε|<1 (inelastic), raising price will increase revenue;
 | ε|=1, revenue is independent of price;
 | ε|>1 (elastic), raising price will decrease revenue.
Now that we have chosen a WTP distribution, estimated the corresponding price-
response function, and estimated the price elasticity, it is finally time to return to our 
original objective—to optimize the price so as to maximize profit.
PRICE OPTIMIZATION
The Objective Function
Before determining the optimal price, firms must establish their strategic goal, one that 
specifies what they are trying to accomplish in the market. Examples include maximiz-
ing the total profit, maximizing the revenue, meeting some predetermined market share 
0.50
Petrol (LR)
Cigarettes
Beer
Water
Electricity (SR)
Petrol (SR)
Branded Products
Electricity (LR)
Spirits
Wine
1.0 1.5 2.0
Elasticity
LR- Long RunSR- Short Run
Figure 6.11 Estimated Price Elasticities for Various Goods (Absolute Values).

---

## Page 161

150  Pricing Analytics
target, or some combination of these three. Normally, we assume that the objective is to 
maximize total profit:
 
Max Profit p Max p c d p
pp
  () =− () ⋅ ()  (6.7)
The total profit as a function of price is hill-shaped, with a single peak, as shown in Fig-
ure 6.12. Let p * represent the price that maximizes the total profit. Not surprisingly, the 
firm’s profit is negative when the price is below its unit cost of $5.
The Price Optimization Problem
We demonstrate how to solve a price optimization problem using an example that resem-
bles many real-life pricing initiatives. A widget-making company sells widgets through a 
single channel. The unit costs are constant at $5 per widget and the demand is governed 
by the linear price-response function represented in Figure 6.2:
d(p)=1,000 – 50 . p.
The firm’s profit as a function of price is
 Profit p p p
pp
() =−() ⋅− ⋅()
=− ⋅ + ⋅ −
5 1 000 50
50 1 250 5 0002
,
,,
 (6.8)
The profit-maximizing price is found by taking the derivative of the profit function and 
setting it to zero. To understand why this is the case, refer back to the curve in Figure 
6.12. The curve in the graph represents the profit function and the highest point in the 
curve is where the slope changes from positive to negative. The slope of the curve is 
0
−3.0
−4.5
−6.0
−1.5
1.5
0
Unit Cost p*
3.0
5 10 2015
Price ($)
Total Profit (thousand $)
Figure 6.12 Profit as a Function of Price.

---

## Page 162

Pricing Analytics  151
found by taking the derivative of the curve’s functional form with respect to price, thus 
we take the derivative of the profit function and set it equal to zero. Applying this tech-
nique to equation (6.8) gives
 –100  . p + 1,250 = 0,
 p * = $12.50.
Returning to the generic equation (6.7), p* is the price where
 Profit'(p) = d(p) + (p – c) . d'(p) = 0. (6.9)
By rearranging the terms in equation (6.9), we get the classic economics result where the 
optimal price to charge, p*, is the price where the marginal revenue equals the marginal 
cost, or:
 p . d'(p) + d(p) = c . d'(p).
Elasticity and Optimization
In the last section, we saw how elasticity can be used to determine if a price change will 
increase or decrease revenue. Elasticity can also provide guidance on when to lower or 
raise prices so as to maximize profits. By combining the equation of point elasticity with 
the condition that the derivative of the profit function should be set equal to zero, we 
find that at the optimal price p*, the following holds true
 ( p* – c)
/p* = –1/ε(p*). (6.10)
By conveniently rearranging the terms in equation (6.10), we obtain:
 
p p
p c*
*
*
= ()
+ ()
⋅ε
ε1  (6.11)
The left side of the equation is the margin per unit expressed as a fraction of price, also 
known as the gross margin ratio. To help illustrate the usefulness of this formulation, 
consider a seller seeking to maximize her total profit. Under what relative values of her 
current price p, her cost  c, and her point elasticity 
ε(p) should she raise her price to 
increase her profit? Under what conditions should she lower her price or keep her price 
the same? The answers are provided by the following set of rules:
 ( p – c)/p = –1/ε(p) → p is optimal (do not change price).
 ( p – c)/p < –1/ε(p) → p is too low—profit can be 
 increased by raising price (i.e., gain in per-unit margin > 
 loss in sales). This will always be true when |ε(p)|<1. 
 ( p – c)/p > –1/ε(p) → p is too high—contribution can be 
 increased by lowering price (i.e., gain in sales will outweigh the 
 loss in per-unit margin).
Note that all rules are local since ε(p) changes as the price changes.

---

## Page 163

152  Pricing Analytics
Examples
1. A two-liter bottle of Coca-Cola has a short-run elasticity of –3.8. The optimal price 
is one that provides a gross margin ratio of – (1/–3.8), or, 26%.
2. The short run elasticity of heroin in Norway has been estimated to be approxi-
mately –1.25. The optimal price for dealers should provide a gross margin ratio of 
–(1/–1.25), or, 80%.
Customer Segmentation and Price Optimization
Up to this point, we have assumed that the population of consumers differs in its will-
ingness-to-pay but not in its price sensitivities. This assumption is implied when we 
use only one price-response function to represent all the consumer population. The 
real value in price optimization, however, often comes from identifying microsegments 
of consumers who have different price sensitivities (coupon users versus noncoupon 
users, for example). To find these microsegments, the historical price demand data set is 
divided into possible different segments based on some customer attributes other than 
price. For example, a data set may be divided into two groups based on the attribute that 
a customer belongs to the firm’s loyalty program or not. Once the data set is divided 
into different segments, the data from each segment can then be fitted to different price-
response functions. There are various ways to test whether the resulting fits of the micro-
segments to different price-response functions are better than the fit of the entire data set 
to a single price-response function. If dividing the data set into the microsegments does 
result in better fits, then prices can be optimized for each segment using their specific 
price-response function.
One example of using price segmentation in the price analytics process has been 
applied at a grocery store chain. Previous studies have shown that consumers who shop 
at a grocery store after 5:00 p.m. on weekdays are generally less price sensitive than con-
sumers who shop on weekdays before 5:00 p.m. This finding is intuitive as the consum-
ers who are shopping after 5:00 p.m. are generally working professionals who are on their 
way home from work and do not bother to comparison shop, while consumers who shop 
before 5:00 p.m. consist of homemakers and retired individuals who, conceivably, are 
more price conscious and have more time to comparison shop. To take advantage of this 
knowledge, there is a grocery store chain in Texas that raises the prices of almost all items 
after 5:00 p.m. on weekdays and lowers them again before opening the next morning.
THE PRACTICE OF PRICING ANALYTICS
Throughout the previous sections of this chapter, we provided a brief summary of the 
theory of pricing analytics. While informative, this discussion has not provided you or 
your organization with advice on important questions such as “Am I ready to start exper-
imenting with pricing analytics? If so, how can I operationalize some of these theoretical 
concepts?” or “When should I declare myself satisfied with the progress I made?” To help 
gain an understanding of what these and other similar questions require of an organiza-
tion, we continue next with a few paragraphs on what developing organizational pricing 
capabilities entails. We then provide a few illustrative examples of how to estimate the 
price elasticity of demand in practice.
Developing and sustaining pricing capabilities is a complex task impacted by factors as 
diverse as the company market position, the vision of its leaders, and the sophistication

---

## Page 164

Pricing Analytics  153
of its execution mechanisms as reflected by the quality of its people and systems (Cudahy 
& Coleman, 2007). In what follows, we look into the issues raised by the process of devel-
oping pricing capabilities from a narrow yet practical angle. First, following our belief 
that people are an organization’s most valuable asset, we judge the organization’s pric-
ing capabilities by the pricing expertise shown by its staff. Second, as the field of pricing 
analytics is data driven, we also assess an organization’s pricing capabilities by the types 
of data available at its disposal (for relevant examples, see Table 6.4). Our latter choice 
is motivated by the fact that the types of data an organization makes use of are often a 
reflection of the sophistication of the support systems that drive the business. Stated 
otherwise, the quality of the business insights derived from the data available typically 
correlates well with the support systems in place within an organization. We illustrate 
our approach in the process roadmap shown in Figure 6.13.
In the initial stages of acquiring pricing capabilities, companies typically find themselves 
at point A in Figure 6.13. Here, they have little or no pricing expertise, since no dedicated 
personnel exist to strengthen this function. Furthermore, no data are usually available 
to support the practice of the function. Ironically, in some cases, companies at this stage 
actually collect and own the market data needed for pricing analytics, but the lack of 
pricing expertise makes it difficult to transform this latent information into actionable 
market decisions. In the evolving business environments in which most organizations 
operate, companies that stay for too long in point A are usually perceived as high-risk 
companies, since they seem to be unable to fully align with their customers’ needs.
Early attempts to adapt to the new business realities usually require organizations to 
employ high-profile external experts or industry advisors to assess and identify pricing 
Table 6.4 Types of Data Used to Make Pricing Decisions
Data Relevance Details
Basics
1. Price/demand data B2C Links prices offered to the market performance of a 
product. Helps build price-response functions.
2. Bid-price data B2B Links prices quoted to the outcome of the bid 
process. Helps build bid-response functions.
3. Pricing guidance and business rules B2C, B2B Specify constrains that apply to pricing decisions.
4. Market segmentation intelligence B2C, B2B Supports the customization of the price.
Advanced
1. Product and location hierarchies B2C Support tier pricing.
2. Special event data B2C Provides the timing of special events (e.g., email 
campaigns, Christmas, etc.) and helps unconstrain 
the demand.
3. Inventory data B2C Helps estimate the inventory effects on sales.
4. Out-of-stock data B2C Helps unconstrain the demand.
5. Promotion data B2C Provides the timing and type of promotion activities. 
Helps unconstrain the demand.
6. Competitive data B2C, B2B Helps link product performance to own and 
competitors’ prices.
7. Click data B2C Helps segment products and customers and supports 
the customization of the price.
B2C: Business-to-consumer pricing; B2B: Business-to-business pricing

---

## Page 165

154  Pricing Analytics
opportunities within the operations of the company. Through the use of some noninte-
grated price experiments or customer surveys, these outside experts often demonstrate 
the potential benefits of developing pricing capabilities. In many cases, the knowledge 
they share with the top management eventually starts to propagate throughout the 
organization and makes people at all managerial levels aware of the lost revenue oppor-
tunities. Yet companies at this stage have limited pricing expertise, as they do not pro-
duce but rather transfer relevant knowledge. A typical position for such an organization 
is point B in Figure 6.13.
Companies that do not feel comfortable knowing that they consistently miss oppor-
tunities will typically respond to this threat by heavily investing in technology. In doing 
so, they gain the edge on their slower-moving competitors. The systems that they put in 
place connect previously uncoordinated organizational functions and provide its users 
with consistent and high-quality market data. Through mutually beneficial partnerships 
and agreements with high-visibility pricing and information technology consultants, 
companies often start to feel and exploit the benefits of their investments shortly after 
the “go live” system phase. In regard to the internal pricing expertise, however, these 
D(DA): Integrated own market
data, competitive data, and
PE and CS
C(PE): Limited pricing expertise
through knowledge replication
A(PE): Little or no pricing expertise
High
Pricing Expertise (PE)
No/Unknown
Availability
Data Availability (DA)
Multisource,
Integrated Availability
Low
A
E
D
C
B
C(DA): Some own
market data
B(DA): Nonintegrated price experiments
and customer surveys (PE and CS)
A(DA): No data or irrelevant market dataB(PE): Limited pricing expertise through knowledge
transfer. External experts, industry advisors, or consultants
disseminate knowledge throughout the organization.
D(PE): Reasonable internal pricing
expertise through knowledge formulation
E(PE): Internal pricing expertise
through knowledge mastering
E(DA): Continuous
improvement of D(DA)
Low Profile, Low Impact High Profile, High Impact
Perceived Relevance and Impact of the Pricing Funciton:
Figure 6.13 Developing Pricing Capabilities: Process Roadmap.

---

## Page 166

Pricing Analytics  155
organizations are still developing, as they could not yet form their own pricing philoso-
phy to support and drive the business. At best, they now start to replicate what faster-
moving competitors have already accomplished in their industry. The lack of highly 
skilled internal pricing personnel, however, keeps them from capturing all the potential 
benefits of pricing analytics. Point C in Figure 6.13 is representative of a company at this 
stage in the development of its pricing capabilities.
Organizations that strive to be predominately analytically market oriented continue 
to invest in game-changing technology and, equally important, in building strong inter-
nal pricing expertise. The integration of their own market data with competitive and 
alternative sources data is typically complemented by hiring the right people to do the 
job. The inception of specialized pricing teams within the larger organization is just a 
normal consequence of this undertaking. As these professionals keep pushing the limits 
of the organization’s information technology (IT) systems, they are now in the position 
to discover and formulate knowledge. In Figure 6.13, the position of such an organiza-
tion is at point D.
Point D in our roadmap coincides with the last step of developing pricing capabilities 
within an organization. To sustain these capabilities and enhance intraorganizational 
learning, however, the organization needs to continuously invest in improving its mar-
ket data and data sources and in retaining its best pricing personnel. At this point, the 
personnel master the skills required in the pricing arena and can use their vast knowledge 
to run successful industry-wide pricing initiatives. This stage is identified with point E 
in Figure 6.13. Although it seems that reaching point E is the final goal of a prolonged 
organizational shaping process, this is rarely the case. In practice, point E as an ultimate 
final state does not really exist—organizations that complete phases A through D and 
want to stay ahead of the pack will always be in point E. Hence, successful market-ori-
ented organizations need to continuously fine-tune their pricing approaches and experi-
ment with innovation.
The roadmap depicted in Figure 6.13 shows two other characteristics worth discuss-
ing. First, the slight concavity of the broken line that links the developmental points A 
through E may seem odd. We associate this shape with how we believe most candidate 
organizations develop pricing capabilities. In particular, the organization’s develop-
ment of internal pricing expertise often lags behind its progress in improving the quality 
and availability of its data and the sophistication of its IT support systems. Our view 
acknowledges that quite often the innovation in pricing happens outside of organiza-
tions, which use the technology as an enabler for acquiring the needed expertise. Second, 
the relevance and business impact of the pricing function are often perceived differently 
by organizations at different stages in the development process. As opposed to organiza-
tions at the beginning of their pricing journey, which typically do not fully acknowledge 
the potential of this function, mature pricing analytics organizations consider it business 
critical and treat it accordingly. We illustrate this perspective in Figure 6.13 through the 
use of the radius-varying, color-coded circles that accompany points A through E.
We conclude our discussion of how organizations develop and sustain pricing capa-
bilities by venturing answers to the questions we posed at the beginning of this section. 
Based on our experience, we believe that it is never too early to start experimenting 
with pricing analytics. It is our hope that you will find this book illustrative of how to 
approach the practical work required by the operationalization of the theoretical con-
cepts. Last, but not least, you should never be satisfied with the progress made—pricing,

---

## Page 167

156  Pricing Analytics
and more important, successful pricing, is all about being proactive and learning how to 
identify and exploit each and every revenue opportunity.
ESTIMATING PRICE ELASTICITY
In today’s business environment, organizations must often revisit the pricing strate-
gies they put in place when they first introduced their products or services. Changes in 
the likes and dislikes of consumers, together with competitors’ actions, are some of the 
forces that call for such critical initiatives. Among the questions sellers attempt to answer 
in these situations, two are consistently at the top of their priority lists. The first relates to 
whether or not the current prices are aligned with how products or services perform in 
the marketplace. Since in many cases an unsatisfactory answer is found, the second ques-
tion focuses on what needs to be done for things to get better. We next provide guidelines 
on how to navigate the intricacies of such an involved task.
In the marketplace, sellers rarely provide their products or services at an optimized 
price. Often, offerings are either underpriced or overpriced. In the previous sections of 
this chapter we explained how to set the optimal prices but deferred the discussion of 
the details for later. In particular, we have shown how to employ the price elasticity of 
demand to achieve an optimum price, but we considered the price elasticity a known 
input into the pricing routine. In reality, however, the price elasticity of demand, as 
well as the price-response function from which it is derived, is unknown. How does one 
estimate a sensible price-response function and use it later to infer the price elasticity of 
an offering? While no definite answers exist, a few general rules apply and can be used to 
accomplish this undertaking.
Many organizations start this task by specifying a set of possible functional forms for 
their price-response functions. Usually, this set includes the linear, constant elasticity, or 
logit specifications, but other more complex forms have also been explored in the litera-
ture (e.g., attraction model, Gutenberg model) (Simon, 1989, p.30). The price-response 
functions considered are calibrated using historical data, and the form that describes 
data the best is typically employed in all subsequent steps, including the derivation of the 
price elasticity. The calibration of the price-response functions is typically approached by 
using ordinary least squares or maximum likelihood estimation techniques, which may 
involve the use of specialized statistical software packages such as R (R Core Team,2013), 
SAS (SAS Institute Inc., 2013), or Stata (Stata Corp, 2013). A short introduction to the 
software package R, an open source software environment for statistical computing and 
graphics, is included in the Appendix B. At a very high level, the ordinary least squares 
method minimizes the sum of squared errors among the observed sales and the sales pre-
dicted by the calibrated price-response functions. This is the technique used in Microsoft 
Excel’s linear regression function, for example. In contrast, maximum likelihood finds 
the parameter estimates for the price-response functions such that the probability of 
the sample data is maximized. In practice, maximum likelihood is typically preferred 
for estimating most functions, as it is perceived to be more robust and yields parameter 
estimates with superior statistical properties. Both of these estimation techniques are 
discussed in Chapter 3.
At this point, a typical newcomer to pricing analytics would express at least two points 
of concern about the feasibility of this approach. On the one hand, relevant historical 
price/demand data may not be available, as the firm may have consistently priced the

---

## Page 168

Pricing Analytics  157
product or service at the same level. Alternatively, the firm may operate in a fast-paced 
environment in which history is not representative of present or future business con-
ditions. Hence, there may be a lack of any calibration-relevant market data and data 
sources. However, it may be unclear exactly what “describes data the best” means. For-
tunately, solutions exist to address both types of concerns.
Organizations that do not have market data readily available to calibrate their candi-
date price-response functions could rely on price experiments, expert judgment, and/or 
customer surveys to do so (Lilien, Tangaswamy, & De Bruyn, 2007, Little, 1970, Simon, 
1989, Wuebker, Baumgarten, Schmidt-Gallas, & Koderisch, 2008). For example, an 
online retailer could run a split test on a few representative products in its portfolio 
to determine the likely response of its customers to various price levels. By randomly 
diverting the incoming web traffic to product web pages that differ only with respect 
to the displayed price, the retailer could get an unbiased understanding of how price 
impacts sales (consulting and software companies such as CoreMatrix LLC and Tealeaf 
Technology Inc. provide their customers with such specialized services). A word of cau-
tion is needed here, as customers who discover that others are receiving lower prices may 
react negatively against the firm. Thus it is generally better to offer different discount 
levels off the same base price during the price experiment (we discuss the psychological 
aspects of pricing in Chapter 9).
Similarly, brick-and-mortar retailers could run in-store price experiments that account 
for differences among stores to extract the same information from their visitors (Gaur 
& Fisher, 2005). If cost or other factors prevent sellers from running price experiments, 
internal or external experts with a good knowledge of the market can be involved to 
assess how changes in price could impact sales and competitors’ reactions (Little, 1970; 
Wuebker at al., 2008, pp. 51–54). The expert opinion can also be used as a means of vali-
dating the results of other pricing initiatives such as price experiments. Some organiza-
tions may prefer to estimate price responses by administering surveys to their customers 
(Wuebker et al., 2008, pp. 54–68). These surveys may be direct or indirect, paper-based 
or computer-based questionnaires.
Given the myriad of choices available, how do you choose which ones apply to your 
particular case (Simon, 1989, p. 36; Wuebker et al., 2008, p 68)? Traditionally, mar-
ket data price-response functions are considered to be cost efficient since the data are 
already available, but the range of historical prices charged may not be wide enough to 
provide accurate price-response function estimates. Expert judgments are perceived as 
being reliable, accurate, and cost efficient, but the quality is only as good as the experts 
employed. Price experiments and customer surveys, if sufficiently designed, have been 
credited with reliability and accuracy but often come at a significant cost. For our take, 
all options should be considered, and we encourage you to have an in-depth look into 
your organization’s capabilities and core competencies before you commit to any of 
these choices. Ideally, your ultimate decision should balance such things as the avail-
ability and quality of your market data; the extent of your in-house expertise; the types 
and performance of your revenue and pricing management and customer relationship 
management systems; and last, but not least, the financial health and potency of your 
organization. For the remainder of this book, we focus on estimating the price-response 
functions assuming that some price/demand data are available. 
We now proceed with explaining what we mean by choosing the price-response func-
tion that describes the data well (for some relevant references, see Chapter 3). To do so,

---

## Page 169

158  Pricing Analytics
we must be able to quantify how well the price-response functions represent the data. 
One index frequently employed to judge the quality of this fit is R2 or R-squared (Greene, 
2003). For specifications that promote a linear relationship between sales and price or 
that can be reduced to such a linear relationship (e.g., the constant-elasticity model), R
2 
represents the proportion of the variation in sales (or in a transformed measure of sales) 
that is explained by price. If sales and price were perfectly correlated, then price would 
fully explain sales, and we would experience a maximum R
2 of 1. In contrast, if sales and 
price were not related or weakly related, we would note an R2 of 0 or close to 0. This is 
equivalent to saying that sales at various price points are best predicted by the histori-
cal average sales and that the historical price offers no additional predictive capability. 
For the price-response functions for which R
2 can be computed, the ones with higher 
R2 are preferred. Functions that do not support the computation of R 2 (e.g., nonlin-
ear price-response functions such as logit) are compared against each other (or against 
specifications that do support an R
2) through the use of different indices such as the 
AIC, or Akaike Information Criterion (Greene, 2003). The AIC attempts to balance the 
accuracy and complexity of the candidate price-response functions and represents a rela-
tive measure. In a practical situation, specifications with lower AICs are preferred. Both 
measures of fit are part of the standard output of the software packages used to calibrate 
the price-response functions.
To illustrate how the points mentioned earlier support the overall objective of calculat-
ing the price elasticity of demand, in what follows, we briefly discuss case studies of several 
organizations that have gone through relevant pricing initiatives. These examples build on 
our consulting work and are used here to illustrate the concepts of pricing analytics. We 
have left out the names of the companies and adjusted some figures to protect our clients’ 
confidentiality. The first organization is a retailer with a significant online presence in the 
children’s products market. The organization has consistently sold one of its representa-
tive items in the baby care essentials category at $7. At the time of this study, it cost the 
retailer $2.50 to purchase the item from its suppliers. Customers of this product were 
believed to respond to changes in price, but the extent of the change was unknown. To 
investigate whether or not revenue opportunities existed for this product, the retailer ran 
a price experiment involving multiple price points. In particular, all online customers who 
accessed the online store during a management prespecified time window were randomly 
shown product web pages of similar content but different prices. The results of this price 
experiment are shown in Table 6.5 and graphically depicted in panel A of Figure 6.14. 
The product manager in charge of this item recommended the price differential of $0.50 
based on her experience with the product. To limit lost sales due to inconsistent pricing 
throughout the period during which the experiment was run, customers who visited the 
product web page multiple times were consistently shown the same price each time.
The results of the online price experiment were first disseminated within the organiza-
tion and feedback was requested from all interested parties (e.g., sales and product man-
agement personnel). The agreement on the intuitive character of the results was followed 
Table 6.5 Online Price Experiment Results
Price ($) 5.0 5.5 6.0 6.5 7.0 7.5 8.0 8.5 9.0
Sales  32  31  30  23  21  21  21  20  13

---

## Page 170

Pricing Analytics  159
by an internal in-depth discussion of the types of price-response functions appropri-
ate for this item. Several functional specifications were explored in connection with the 
constraints exhibited by the retailer’s information systems. The retailer eventually opted 
for a linear price-response function of the form detailed in equation (6.1). The calibra-
tion of this function, that is, the estimation of the intercept D and the slope m, was done 
using the ordinary least squares method for fitting linear models as implemented in R 
(see function
 lm). For completeness, we provide a summary of the statistical properties 
of the parameters of the price-response function and the overall model fit in Table 6.6. 
These figures suggest that price determines sales following the linear relationship d(p) = 
53.7–4.3 p, where the intercept D =d(0) = 53.7 and slope m = –4.3 are both statistically 
significant and different than 0 at a 99.9% confidence level. The high t values (or, alter-
natively, the small p values) support both these conclusions. In this situation, the model 
predicts that if the retailer prices the product at $0, then demand will be 53.7 units of the 
product. Furthermore, irrespective of the price point charged, the model predicts that 
if the retailer increases the price by $1, then sales will decline by 4.3 units. Based on this 
linear formulation, any price point above $12.49 is predicted to lead to zero sales. The 
price-response function seems to fit the data well, as the price alone appears to explain 
0
02468 1 0
Price P ($)
(A) Linear
Price-Response Function
Sales
12
0
5
10
15
20
25
10
30
20
40
50
60
0
25 30 35 40
Price P ($)
(B) Constant Elasticity
Price-Response Function
Sales
Elasticity
0
0 100 200
Price P ($)
(C) Logit
Price-Response Function
Sales
300
0
5
10
15
20
25
400
200
600
Elasticity
Elasticity
45
0
5
10
15
20
25
40
80
120
Price-Demand
Experimental Data Points
Experimental Price
Range
Price-Response
Function
Elasticity Curve
Equivalent Linear
Price-Response Function
Figure 6.14 Price-Response Functions and Elasticity Curves.

---

## Page 171

160  Pricing Analytics
89% of the variation in sales (see the multiple R2 of 0.89, which is quite close to its maxi-
mum value of 1.00). The straight line describing the assumed relationship between sales 
and price is shown in panel A of Figure 6.14 and superimposed on the experimental 
sales-price scatterplot.
The characteristics of the price-response function presented in Table 6.6 are unit 
dependent and, therefore, context specific. To generalize the knowledge and apply it to 
contexts other than the price experiment itself, the retailer computed the price elasticity 
of demand across the range of prices with nonzero expected sales. The use of the point 
elasticity formula for linear price-response functions provided in previous sections led to 
the elasticity curve depicted in panel A of Figure 2.2. At the selling price of $7, the price 
elasticity of demand is, in absolute value, about 1.28. Armed with this information, the 
retailer could easily assess the appropriateness of its pricing strategy for this product. 
Following the discussion associated with equation (6.10), it appears that the product was 
underpriced, as the contribution margin ratio (p – c)/p was less than the reciprocal of the 
point elasticity 1/
ε(p) at the selling price p of $7 (i.e., 0.64 vs. 0.78).
Our second example comes from a specialty apparel retailer who operates a small 
regional network of stores. The retailer sells clothes that target children in their preadoles-
cence stage (i.e., ages 9 to 13) and should appeal not only to the youngsters but also to their 
legal guardians who typically sponsor the purchases. In an attempt to better understand 
the likely price/demand relationship for a representative item, the retailer devised and 
executed a preseason, in-store price experiment intended to capture the price sensitivity 
of customers shopping for such an item. At the time of the experiment, it cost the retailer 
$22 to purchase the item. The intention of the product managers was to open the season 
with a product retail price of $34.95, which could later be adjusted based on how the 
market responded to this initial price. The relatively low gross margin of 37.05% ($12.95) 
is atypical of the apparel retail industry and reflects conditions relevant to this product 
only. The experiment was run for a given period of time in a few selected stores that were 
thought to be representative of the entire chain and accounted for individual store intrica-
cies. The price points at which the product was offered were chosen such that no stores in 
close proximity featured the product at conflicting prices. Across all stores, the aggregate 
sales are shown in Table 6.7 and graphically depicted in panel B of Figure 6.14.
As in the case of the retailer in the children’s products market, the results of this price 
experiment were disseminated to all internal groups with an interest in the management 
Table 6.6 Linear Price-Response Function: Summary Statistics and Model Fit
Variable Coefficient Standard Error t value p value
Intercept D 53.7 4.1 13.1 0.00
Slope m –4.3 0.6 –7.5 0.00
Residual standard error: 2.232 on 7 degrees of freedom
Multiple R-squared: 0.89, Adjusted R-squared: 0.87
F-statistic: 55.67 on 1 and 7 DF, p-value: 0.00
Table 6.7 In-Store Price Experiment Results
Price ($) 29.95 32.45 34.95 37.45 39.95
Sales  71  57  46  33  27

---

## Page 172

Pricing Analytics  161
of the item. Of these, the fashion merchandise buyers and the marketing and pricing 
personnel expressed the most opinionated points of view about the observed sales pat-
terns. In particular, while the former group believed that they were appropriately pricing 
the item, the latter thought that a price increase was needed for the organization to be 
more profitable. To investigate these claims further, the retailer considered two types of 
price-response functions to be fitted to the data—with a similar model fit in terms of R
2, 
both linear and constant-elasticity price-response functions constituted good candidate 
specifications. The linear price-response function was, however, discarded on subjective 
grounds that had to do with the difficulty of communicating the resulting elasticities to 
field employees. The retailer felt that communicating a single elasticity for an item would 
be easier for its less technical employees to grasp.
The calibration of the chosen functional form—that is, the estimation of the con-
stant C and the price elasticity 
ε (for details, revisit equation (6.2))—was done using the 
ordinary least squares method for fitting linear models as implemented in R (see func-
tion 
lm). To facilitate the calibration, a log transformation was applied to both terms of 
equation (6.2). This transformation converted the original price-response function to 
an equivalent but easier to estimate linear specification of the form log( d(p))= 
β0 +β1 
log(p), where β0 = log(C) and β1 = ε. The recovery of the original function’s param-
eter values comes from C = exp(β0) and ε = β1. A summary of the parameter estimates, 
together with the model fit, is provided in Table 6.8. The curve that describes the rela-
tionship between sales and price together with the assumed price elasticity 
ε is graphically 
depicted in panel B of Figure 6.14. The C parameter value suggests that at a retail price of 
$1, the organization could sell about 8.7 million units of the product. In the same spirit, 
the price elasticity 
ε of –3.44 implies that a 1.00% increase in price is associated with a 
3.44% decrease in sales, irrespective of the offered retail price (because it is a constant-
elasticity model). For example, by changing the price by 1%, from $34.95 to $35.30, the 
retailer should expect to see a drop in sales of about 3.44%, from 43.28 to 41.82 units (the 
apparent inconsistencies between the percent and absolute values of the figures are due 
to rounding errors). The nature of the price elasticity, which stays constant across the 
full range of prices, helps the retailer determine the quality of its current product pricing 
strategy. Referring to equation (6.10), we learn that the product seems to be overpriced, 
as the contribution margin ratio (p–c)/p is greater than the reciprocal of the point elas-
ticity 1/
ε(p) at the selling price p of $34.95 (i.e., 0.37 vs. 0.29). This result contradicted 
the expectations of both groups at the retailer, each of whom thought they had a good 
understanding of how the product was going to be received in the marketplace.
Table 6.8 Constant-Elasticity Price-Response Model: Summary Statistics and Model Fit
Variable Coefficient Standard Error t value p value
β0 15.98 0.74 21.7 0.00
β1 –3.44 0.21 –16.6 0.00
C 8,710,154
ε –3.44
Residual standard error: 0.05 on 3 degrees of freedom Multiple R-squared: 0.99, Adjusted R-squared: 0.99 F-statistic: 
274.9 on 1 and 3 DF, p-value: 0.00

---

## Page 173

162  Pricing Analytics
Over the range of experimental prices, the sales curve d(p) resembles a straight line 
(in Figure 6.14, in addition to the constant-elasticity price-response function  d(p), we 
also show for convenience the equivalent linear price-response function). Outside of it, a 
straight line departs significantly from the curvilinear geometry of the constant-elasticity 
price-response function. In layman’s terms, this means that the differences in behavior 
between the linear and constant-elasticity price-response functions are expected to be 
more significant over a larger price range than was covered in the experiment. We illus-
trate this point by discussing the extreme case of the sales expected to materialize at a 
price point of $0. For this scenario, the constant-elasticity price-response function we 
calibrated for the apparel retailer is not satiating and approaches infinity. As this may be 
too abstract to visualize properly, we reiterate that the retailer is expected to sell some 
8.7 million units of the product at a price point of $1. In contrast, had the retailer stayed 
with the linear price-response function, the model would have predicted sales of about 
204 units at a price point of $0. The lesson here is that users should be especially wary 
of using any prediction that is outside of the range of prices the price-response function 
was estimated on.
The examples we have discussed so far involve the calibration of simple price-response 
functions. In normal circumstances, any standard statistical software package, including 
Excel, can be used to complete this task. At times, however, more advanced analytical 
capabilities are needed to extract relevant insights from the data available. We illustrate 
this point with an example from a manufacturer who plays an active role in the con-
sumer electronics industry. In the United States, the manufacturer sells its personal dig-
ital assistants (PDAs) to end consumers through its own stores or through other retail-
ers such as Wal-Mart and Best Buy. Products can be purchased in the physical stores 
or ordered online. The competition in the marketplace is fierce for this product type 
but the prices of competing products have been stable and there are no indications that 
they will change soon. To prepare for the launch of a new generation model for one of 
its popular PDAs, the manufacturer ordered an extensive customer survey carried out 
by an independent, third-party intermediary. Among other things, the objective of the 
survey was to determine how the market would respond to alternative price points for 
the product. The survey was administered to existing customers known for their loyalty 
toward the brand, as well as new consumers who had not historically bought this brand. 
We present the survey results that are relevant to our discussion in Table 6.9 and panel C 
of Figure 6.14. These figures, conveniently rescaled to safeguard privacy, are the outcome 
of a demanding validation effort that required additional inputs from external industry 
experts, independent consultants, and internal stakeholders with responsibilities in the 
short-and long-term management of the product. In what follows, we restrict the expo-
sition to the calibration of the price-response function(s) and the formulation of price 
elasticities because the production and research and development (R&D) costs at this 
manufacturer cannot be disclosed.
Table 6.9 Customer Survey Results
Price ($]) 50.00 100.00 150.00 200.00 250.00
Sales  710  666  373  54  24

---

## Page 174

Pricing Analytics  163
The visual inspection of the scatterplot depicted in panel C of Figure 6.14  reveals 
that an inverse S-shaped price-response function may be appropriate for this product. 
Although both logit and power functions were considered as qualified candidates, the 
formulation of price sensitivity measures associated with the former appealed more to 
the manufacturer. Thus it opted for a logit price-response function that required the 
calibration of parameter estimates a, b, and C. We performed the calibration using the 
nonlinear weighted least squares method for fitting nonlinear models as implemented 
in R (see function 
nls). To facilitate the estimation, we rewrote the expression provided 
in equation (6.4) as
 dp Ce
e
C
e
C
e
C
e
ab p
ab p ab p bp a
bpa b
() = ⋅
+
=
+
=
+
=
=
+
+⋅
+⋅ −−⋅ −⋅ +()
−⋅ +
11 1
1 (() −−() −()=
+
=
+
A
e
A
epI s I p s11
,
where C = A, a = –I/s, and b = 1/s, and. The newly introduced parameters  A, I, and s 
are geometric elements that carry a palpable meeting. Parameter A represents an upper 
bound past which sales cannot grow irrespective of the price offered. Similarly, I identi-
fies the price point at the inflection point of the logit curve. Finally, s is a scale parameter 
on the price dimension. Using R, we first estimated the geometric parameters A, I, and s, 
from which we derived the values for a, b, and C. A summary of all parameter estimates, 
together with the model fit, is provided in Table 6.10. In panel C of Figure 6.14, we super-
imposed the resulting logit curve across the sales-price scatter plot. The A (or C) value 
of 714.56 suggests that sales cannot exceed this value irrespective of the prices offered. 
At low prices, sales are expected to approach this upper bound and change slowly as the 
price increases. For example, at a price of $0, sales of about 714.22 units are predicted. 
The rate of change accelerates as the price increases and reaches its maximum value at 
the inflection point I = –a /b of $151.70. In business terms, this translates to customers 
responding aggressively to any price changes made around the market price of $151.70. 
Thus small price changes are predicted to lead to significant sales shifts among products 
and competitors. As prices increase past the inflection point  I, the curve flattens again 
and approaches 0 units around a price of $250.00.
To compute the price elasticity of demand for the logit price-response curve of Table 
6.10, we return to equation (6.6), which we rewrite as
Table 6.10 Logit Price-Response Function: Summary Statistics and Model Fit
Estimate Std. Errors t value p value
A 714.56 13.1 54.5 0.00
I 151.70 1.7 88.1 0.00
S –19.80 1.8 –10.9 0.01
a 7.66
b –0.05
c 714.56
Residual standard error: 13.68 on 2 degrees of freedom AIC: 43.77

---

## Page 175

164  Pricing Analytics
 
ε p p
dp
d
dp dp p
dp
d
dp
Ce
e
p
d
ab p
ab p() =
()
⋅ ()() =
()
⋅ ⋅
+
⎛
⎝
⎜⎜
⎞
⎠
⎟⎟=
=
+⋅
+⋅1
p p
Cbe
e
bp
e
ab p
ab p ab p()
⋅ ⋅⋅
+()
= ⋅
+
+⋅
+⋅ +⋅
1 12
or, equivalently, as
 ε p p
e p() =− ⋅
+ −⋅
00 5
1 76 6 00 5
. ...
To help provide an understanding of the price elasticity of demand for this manufacturer, 
the elasticity is plotted in panel C of Figure 6.14. The elasticity increases continuously as the 
price increases. For example, although the slope of the price-response function at a price 
of $250.00 is only –0.25 units per dollar, the ratio of the price and the demand expected to 
materialize at this price is 50.16. Ultimately, this leads to a point elasticity of –12.54, which is 
almost two times larger than the elasticity experienced at the inflection point I of $151.70.
The examples we have discussed up to this point illustrate that the estimation of the 
price elasticity of demand in practical settings often involves as much art (i.e., subjectiv-
ity) as science (i.e., objectivity). As one should be aware of the trade-offs needed when 
undertaking such a task, we take this opportunity to relate it to the main steps of a typical 
pricing initiative.
Step 1: Motivation and Scope
Step 1 is to provide the business logic behind the pricing initiative and clearly identify 
the project’s scope. Scope creep, with a subsequent extension of the project timeline, is 
a common problem as other areas begin to discover additional business opportunities 
as the project evolves. Thus clearly defining the scope at the beginning of the project 
is particularly important. A system-wide, recurrent initiative intended to look into the 
pricing of thousands of products in real time is likely to dictate not only the technology 
to be used but also the pricing analytics embedded in the system’s back end. Hence, a bal-
ance is needed between the speed and accuracy of the latter to make sure that the system 
response times stay acceptable.
Step 2: Design
Step 2 is to look into the roles and tasks of all actors involved with the initiative. Its scope 
typically drives all decisions at this stage. The choices for technology (e.g., web based); 
data acquisition and storage (e.g., customer surveys, point of sale data, and enterprise 
data warehouse, respectively); and pricing analytics (e.g., types of price-response func-
tions) are all influenced by what the organization attempts to achieve. Domain expertise 
is critical as the links among various project components are not always clear.
Step 3: Testing
The point of this step is to make sure that the pricing initiative can go live and not experi-
ence problems before its actual execution. Few organizations that we have seen skip this

---

## Page 176

Pricing Analytics  165
step, as it is almost impossible to make things work right from the first attempt. Whether 
it is unit, integration, or system testing or just survey pretesting, organizations at this 
stage intend to anticipate, test, and remove obvious or not-so-obvious bottlenecks.
Step 4: Execution
This step coincides with the “go-live” phase of the pricing initiative. Based on how com-
plex the design is, the execution may take a few days to complete or it may seem to never 
end. Simple online price experiments focused on the performance of a single product 
are typically executed in just a few days. Initiatives that are recurrent or designed for 
continuous performance fall under the latter category.
Step 5: Control
For pricing initiatives that are recurrent or designed for continuous performance, this 
step coincides with the maintenance phase. Based on the live performance of the initia-
tive, improvements are often suggested for the original design. However, changes can be 
expensive to implement and/or can only be partially implemented after the system is in 
place. Thus it is important to get as much right the first time as possible.
SUMMARY
To summarize this chapter, we began with the ultimate goal: to be able to determine 
different segments of customers based on their price sensitivities and to optimally set a 
different price for each segment. To accomplish this objective, pricing analytics theory 
states that we use historical price/demand data to measure and test the price elasticity of 
different segments. Price elasticity is the percentage change in demand for a percentage 
change in price. Thus larger (negative) values of price elasticity represent price-sensitive 
segments while smaller (negative) values represent price-insensitive segments. Once the 
price elasticity for each customer segment is known, optimizing the price for each seg-
ment is straightforward.
To estimate price elasticities from historical price/demand data, we must make 
assumptions about how the maximum willingness-to-pay for a product is distributed 
over the entire set of potential customers. Different assumptions about the willingness-
to-pay distribution result in different price-response functions that will be estimated 
using the price/demand data. Some price-response functions are simpler and easier to 
estimate than others, but care must be taken that we are accurately modeling true buying 
behavior. Thus, it is common to evaluate several potential price-response functions on 
the same set of estimation data (a subset, but not all, of the historical price/demand data 
set) to determine which function provides the best fit for the remaining holdout sample. 
Once a price-response function has been selected, price elasticities for each segment can 
be calculated, statistical significance tests can be performed, and price optimization can 
be performed for each significant segment.
To transition from the theory to the practice of pricing analytics, we provide an over-
view of what developing pricing capabilities within an organization entails. Our graphical 
roadmap is intended to help identify where your organization is in the process of gaining 
such capabilities. In close connection to acquiring pricing competence, we stress and stand 
by the following principles: (1) it is never too early to start experimenting with pricing 
analytics; and (2) pricing analytics requires continuous refinement and improvement.

---

## Page 177

166  Pricing Analytics
Since the price elasticity of demand plays a significant role in the operationalization 
of pricing analytics concepts, we provide insights into how organizations can go about 
estimating it, both with and without historical transaction data. If data are available, we 
highlight that selecting the best functional form for the price elasticity functions involves 
as much art as science. On the art side, one must understand how the business functions 
and how sophisticated the staff and support systems are. On the science side, one must 
consider competing functional forms that are calibrated and judged against standard 
performance metrics. This resource assessment must then be tied to the science of pric-
ing analytics such that an optimal balance is achieved. We provide several examples, 
motivated by real-world pricing projects, to demonstrate the process of how firms can 
undertake their own pricing analytics projects. To provide a concrete context, we also 
discuss what a typical pricing initiative requires of an organization and link the estima-
tion of price elasticity to the corresponding upstream and downstream processes.
NOTE
1. For consistency and where appropriate, we use the same notation in this chapter as Phillips (2005).
REFERENCES 
Ayers, R., & Collinge, R. (2004). Microeconomics: Explore and apply. Upper Saddle River, NJ: Prentice Hall. 
Brownell, K. D., Farley, T., Willett, W. C., Popkin, B. M., Chaloupka, F. J., Thompson, J. W., et al. (2009). The 
public health and economic benefits of taxing sugar-sweetened beverages. The New England Journal of Medi-
cine, 361(16), 1599–1605. 
Cudahy, G., & Coleman, G. L. (2007). The price is right … Isn’t it? Outlook, 4(1), August 14, 2013. Retrieved from 
www.accenture.com/SiteCollectionDocuments/PDF/Accenture_Outlook_Jan07_Pricing.pdf. 
Dalhuisen, J. M., Florax, R. J. G. M., Groot, H. L. F. d., & Nijkamp, P. (2003). Price and income elasticities of resi-
dential water demand: A meta-analysis. Land Economics, 79(2), 292–308. 
Espey, J. A., & Espey, M. (2004). Turning on the lights: A meta-analysis of residential electricity demand elasticities. 
Journal of Agricultural and Applied Economics, 36(1), 65–81. 
Fogarty, J. J. (2005). Wine investment, pricing and substitutes. Unpublished Doctoral Dissertation, University of 
Western Australia, Crawley, Western Australia. 
Gallet, C. A., & List, J. A. (2003). Cigarette demand: A meta-analysis of elasticities. Health Economics, 12(10), 
821–835. 
Gaur, V., & Fisher, M. L. (2005). In-store experiments to determine the impact of price on sales. Production and 
Operations Management, 14(4), 377–387. 
Goodwin, P., Dargay, J., & Hanly, M. (2004). Elasticities of road traffic and fuel consumption with respect to price 
and income: A review. Transport Reviews, 24(3), 275–292. 
Greene, W. (2003). Econometric analysis. Englewood Cliffs, NJ: Prentice Hall. 
Lilien, G. L., Rangaswamy, A., & De Bruyn, A. (2007). Principles of marketing engineering (1st ed.). Bloomington, 
IN: Trafford Publishing. 
Little, J. D. C. (1970). Models and managers: The concept of a decision calculus. Management Science, 16(8), 
466–485. 
Phillips, R. (2005). Pricing and revenue optimization. Stanford, CA: Stanford University Press. 
R Core Team. (2013). R: A language and environment for statistical computing . Vienna, Austria: R Foundation for 
Statistical Computing. Retrieved from www.r-project.org/. 
SAS Institute Inc. (2013). SAS software. Cary, NC: SAS Institute. Retrieved from www.sas.com. 
Simon, H. (1989). Price management. New York, NY: North Holland. 
StataCorp. (2013). Stata statistical software. College Station, TX: StataCorp LP. Retrieved from www.stata.com. 
Tellis, G. J. (1988). The price elasticity of selective demand: A meta-analysis of econometric models of sales. Journal 
of Marketing Research, 25(4), 331–341. 
Wuebker, G., Baumgarten, J., Schmidt-Gallas, D., & Koderisch, M. (2008). Price management in financial services: 
Smart strategies for growth. Burlington, VA: Ashgate-Gower.

---

## Page 178

7
DYNAMIC AND MARKDOWN PRICING
INTRODUCTION
The last few years have witnessed a significant change in how organizations have 
approached the pricing of their products and services. Slowly but surely more and more 
companies have embraced and promoted dynamic pricing as a means of meeting the 
needs of individual customers and dealing with particular business situations. News 
reports in the popular media and articles in the scientific press have highlighted the 
potential benefits associated with dynamic pricing. A quick scan of these sources reveals 
that the concept has already crossed industry boundaries and has become the new thing 
in industries as diverse as utilities (e.g., Pacific Gas and Electric Company, a subsidiary of 
PG&E Corporation), ticketing (e.g., Digonex Technologies Inc.), sports (e.g., St. Louis 
Cardinals and Chicago White Sox), and the arts (e.g., the Arts Club Theater Company 
in Vancouver, the Saint Paul Chamber Orchestra, the Goodman Theatre in Chicago). 
These featured success stories help build excitement for the science of dynamic pricing, 
but they often lack the depth or conciseness that one needs to really understand it. In 
this chapter, we answer the questions “What is dynamic pricing?” “What are the most 
popular forms of dynamically pricing a product or service?” and “How can you imple-
ment it and exploit its benefits?” We start the chapter by providing an understanding of 
what dynamic pricing is and what it entails. We then delve into the details of markdown 
optimization, which is one the most practiced forms of dynamic pricing. Finally, we 
conclude the chapter with a discussion of a few relevant real-life examples.
DYNAMIC PRICING
Parties involved in commerce have experimented with variable pricing since the begin-
ning of commerce itself. Throughout history, most transactions between sellers and buy-
ers have involved some form of bargaining. In some Middle East cultures, bargaining 
became such a social phenomenon that not being open to negotiate was often taken as a 
great offense. Based on who had the bargaining power, buyers and sellers would typically 
167

---

## Page 179

168  Dynamic and Markdown Pricing
agree on a selling price that was perceived to be fair by both parties. Yet had the business 
circumstances or the control of power been different, the same buyers and sellers may 
have reached agreements of a different nature.
Throughout the 20th century, with the development of the modern retailing in the 
Western societies, the focus of pricing has shifted from variable to static pricing. The 
diversity of the product assortment and the variety and size of the customer base made 
it difficult for retailers to sustain any viable variable pricing initiatives. Today, the “one-
size-fits-all” approach in terms of pricing has become the norm in many business-to-
consumer (B2C) industries. Typically, the reluctance of organizations to adapt to market 
forces and adopt alternative pricing strategies has been linked to the high costs of physi-
cally changing prices and/or acquiring the required sophisticated hardware and software 
support platforms. Imagine, for example, that a Wal-Mart Supercenter had the capabil-
ity to compute daily a set of highly accurate prices for all its hundreds of thousands of 
products. In spite of its accuracy, the execution of such a price change would require an 
organizational effort that store managers could not afford. Hence, they would disregard 
most, if not all, of the price recommendations. However, if in-store electronic shelf labels 
were available, the likelihood that the same store managers would accept and implement 
the suggested price changes would be substantially increased.
In some business contexts, however, the static trends in setting and maintaining prices 
have been challenged and reversed for quite a while. In these environments organiza-
tions attempt to update the prices of their products or services continuously based on 
market forces including the foreseen demand, the supply availability, and other contex-
tual factors such as seasonality, special events, or the weather. In our view, dynamic pric-
ing refers to this process of continuously adjusting the prices to meet the evolving needs 
of the organization and its customers. Although from the outside the process seems to 
be controlled primarily by sellers, in practice, it does involve some subtle forms of bar-
gaining where, at times, buyers gain control. For example, when the needed supply is 
overestimated, sellers tend to lower prices to spur the demand for their products or serv-
ices and clear the excess inventory. In informal terms, sellers admit that they have made 
a purchasing, allocation, or replenishment mistake and intend to correct it by inviting 
buyers to purchase at discounted prices. In this case, buyers are in control as their tardy 
response may trigger other subsequent price discounts. In contrast, when the available 
supply is perceived as insufficient, smart sellers may increase the price in anticipation of 
the elevated levels of demand. Their message to the customers could very well be sum-
marized as, “We know we have a valuable asset and we are more than happy to share it 
with you as long as you are willing to pay the right price for it.” Obviously, sellers own 
the negotiation power in this case. We have brought up the discussion of who is in con-
trol of what and when simply to illustrate how dynamic pricing functions. In reality the 
shift in control, although real, happens seamlessly without any explicit reference to its 
existence. The bargaining, that is, the decisions of when to change the price and by how 
much, is typically controlled in the background by sophisticated and costly decision sup-
port systems that utilize information gathered from various sources to offer their price 
recommendations.
The answer on who exactly originated the modern form of dynamic pricing is not 
simple as the literature does not seem to share an unequivocal perspective on this issue. 
Some authors have credited airlines and hotels as being the first to engage in dynamic 
pricing (Elmaghraby & Keskinocak, 2003). Others have considered the pioneering efforts

---

## Page 180

Dynamic and Markdown Pricing  169
of these organizations as the precursors of the modern dynamic pricing (Gallego & van 
Ryzin, 1994; Talluri & van Ryzin, 2004). These differences aside, airlines and hotels in 
the late 1970s started to ration the availability of their supply in an attempt to become 
more market oriented, more responsive, and more profitable. By limiting customers’ 
access to classes of products priced distinctively, these organizations often seemed to 
be engaged in dynamic pricing. The apparent price changes, however, were exclusively 
due to the allocation of available capacity to the underlying product classes and not to 
a conscious effort of recalculating prices. Hence, sales were controlled by appropriately 
allocating the capacity and not by optimally setting the prices. This subtle difference 
sparked the debate in the literature over which firms really employ dynamic pricing. 
Nowadays, fueled by the fierce competitive environment and fickle customer base, both 
airlines and hotels seem to have moved toward operations that more closely resemble 
dynamic pricing than capacity allocation. InterContinental Hotels Group and Carlson 
Hotels Worldwide, for example, have claimed to have the capability of optimizing the 
retail rates at all participating hotels in their portfolios in real-time based on consumer 
response, competitive rates, and capacity constraints (Carlson Hotels Worldwide, 2009; 
InterContinental Hotels Group, 2009).
The encouraging results experienced by airlines and hotels prompted organizations 
in other industries to start experimenting with dynamic pricing. Retailers of style and 
seasonal goods such as Gymboree and Bloomingdale’s looked at it as an opportunity 
to better manage the demand and control the losses due to out-of-stock (OOS) events, 
lost sales, and excess inventory. Since in-season product replenishment is not a viable 
option for many fashion retailers, they have to make the most out of a fixed inventory. 
Typical dynamic pricing strategies employed by these retailers are the preseason price 
promotions and the in-season temporary and permanent price markdowns. In contrast, 
retailers of nondurable goods, such as Safeway and Walgreens, face the pressing question 
of how to manage pricing and replenishment together such that decisions in one area 
support those in the other. For example, offering a product in short supply at a low price 
could be detrimental as the corresponding sales rates would likely lead to OOS events 
and lost revenue opportunities. Based on customers’ price sensitivity, a better alternative 
could be to temporarily increase the price in anticipation of the arrival of a new product 
batch. In spite of the potential of coordinating pricing and procurement, dynamic pric-
ing by nondurable goods retailers is still rare. Instead, most retailers resort to category 
or product hierarchy-grouping pricing to frequently adjust the regular product prices in 
the absence, though, of any inventory-related information.
One would be remiss to review the field of dynamic pricing without referring to what 
it involves in e-business environments (firms selling primarily through the Internet). 
In particular, e-business seems to be the most natural host of dynamic pricing appli-
cations due primarily to two intertwined developments (Bichler, Kalagnanam, Katirci-
oglu, King, Lawrence, & Lee, 2002; Narahari, Raju, Ravikumar, & Shah, 2005). First, the 
online medium supports the seamless transfer and circulation of information through 
the entire business. Any price changes recommended by the analytics engines or sug-
gested via human interventions are now propagated instantaneously through the infor-
mation technology (IT) system network. Thus the high costs of physically changing the 
posted prices are no longer an issue in the context of e-businesses. Second, the prospects 
of an increased customer base have been associated with an increase in the uncertainty 
and composition of demand, which in itself is expected to warrant the use of dynamic

---

## Page 181

170  Dynamic and Markdown Pricing
pricing. In particular, it has been speculated that in online markets, static prices are both 
ineffective and inefficient. We refer next to a few issues that online markets promise to 
deliver on.
Technological advances exploited by service providers in the online customer rela-
tionship and experience management domains allow e-businesses to collect customer 
data at an unprecedented level of detail. Software applications such as those provided by 
CoreMatrix LLC or Tealeaf Technology Inc., among others, enable online businesses to 
find and remove inconsistencies in their virtual store designs, track customers’ interac-
tion with these stores, and last but not least, learn the search and purchase behavior of 
their customers. These features facilitate the development of customized pricing where it 
is now feasible for each online customer to be quoted her own retail price. If the current 
trends continue, it is not unrealistic to believe that these customized prices could be fur-
ther refined in real-time to dynamically account for other contextual factors including 
inventory levels, day of week, time of day, customer worthiness, and the prices at com-
petitors. A major European online retailer, for example, has recently started to explore 
the benefits of providing a select group of its unconverted customers (i.e., visitors who 
leave the retailer’s website without purchasing) with customized, e-mail delivered, e-
promotions on either the visited items or other related products (e.g., For six hours 
only, Get a 10% discount on all available cardigans). Along the same lines, serious steps 
are taken in many Western European countries to integrate the operations of disparate 
online stores with those of parcel carriers in an attempt to provide customers with cus-
tomized delivery options reflective of such things as the customer propensity to accept 
delayed deliveries (e.g., to avoid high weekend out-of-stock rates and peak workloads in 
the supplier’s warehouses on Mondays), the customers’ day-of-week and time-of-day 
availability (e.g., to avoid failed delivery attempts), the online store’s real-time inven-
tory levels, the real-time status of the carriers’ networks, and the carriers’ competitive 
landscape. Although built on different needs and principles, in the United States, Price-
line.com provides a relevant example of where dynamic/customized pricing is today 
in online environments. Among other services, the company allows its customers to 
name their own prices for opaque travel services, that is, services acquired from provid-
ers but presented to the customer with an unknown service time or provider’s identity. 
In this case, last-minute travelers looking for a deal could benefit from the distressed 
inventory of organizations that likely wouldn’t have otherwise sold it. As each offer is 
customer-specific and accepted if a minimum profit margin is guaranteed, Priceline.
com’s practices can be viewed as providing customized pricing at close to the customer’s 
willingness-to-pay.
Given the advantages of dynamic pricing mentioned previously, why have not more 
organizations and industries rushed to embrace and practice it? In addition to the reasons 
we have already hinted at, there are quite a few others that may prevent companies from 
experimenting with it. Take, for example, the case of retailers in the luxury item business. 
Although at times they may experience weak demand, they tend not to rely on any price 
discounts to accelerate sales as such an approach would diminish the value of their brands 
and anger their loyal customers. For example, a collector who invested $500,000 in a 18K 
rose Patek Philippe Minute Repeater Tourbillon wristwatch would not like to see her col-
lection item being sold for $100,000 at another time or place. Alternatively, some organiza-
tions’ missions may conflict with the for-profit concepts popularized by dynamic pricing. 
An opera house or an arts center that desires to make its product accessible may have a hard

---

## Page 182

Dynamic and Markdown Pricing  171
time explaining to its donors and supporters that dynamic pricing helps it survive. Unlike 
these not-for-profit organizations, movie theaters, for example, which need to make high 
payments on their lease agreements with the movie distributors, are often reluctant to 
employ dynamic pricing because lowering entry prices in particular may be perceived by 
potential viewers as a signal for a substandard quality motion picture, in which case the 
success of the movie would be irremediably compromised. Lastly, companies that employ 
dynamic pricing may lose their credibility as customers confronted with changing prices 
for products they perceived undifferentiated may feel cheated. To avoid such a reputation, 
airlines and hotels, for example, clear their excess inventory through online travel aggrega-
tors (e.g., Expedia.com) or opaque channels (e.g., Priceline.com) rather than through their 
own websites. In doing so, last-minute travelers adamant to catch specific flights or stay in 
particular hotels continue to be charged regular prices without feeling exploited.
Whether you need to clear your excess inventory or set up and adjust the prices for 
your products or services to reflect the changing needs of your organization and custom-
ers, dynamic pricing may help you do it more profitably (for more details, see eMarketer 
(2013)). At a high level, it intends to replace the gut feeling approach to doing business 
with fact-driven decision making. The required facts are typically derived and learned 
from customer data and updated regularly as markets evolve. From our experience with 
dynamic pricing systems, successful organizations start their implementation journeys 
small but with very aggressive deadlines. Prototypes developed in house or with external 
assistance that prove the feasibility of the concept and prepare the organization for it are 
usually followed by a fast and furious full-scale roll out. Since implementations often 
cost millions of dollars, the rush to deliver the systems is understandable—the manage-
ment team will be eager to start enjoying the benefits of its investment as quickly as pos-
sible. How the journey ends is often a reflection of: 1) how supportive of the project the 
upper management is; 2) how experienced the project management team is; and 3) how 
diligent and knowledgeable the implementation team is. To help fully understand the 
implications of these three success pillars, we paraphrase a saying from the tough world 
of mountaineers: “You can attempt to conquer Everest if you have some money, a good 
plan, and an excellent companion. Nothing else seems to work.”
MARKDOWN OPTIMIZATION
In this section, we focus on retailers of style and seasonal goods who at times may need 
to offer permanent in-season price markdowns in an attempt to spur sales, clear excess 
inventory, and maintain healthy margins. In many cases, moving the excess inventory off 
the sales floor fast and at high margins is the number one explanation for why retailers 
employ price markdowns. Judiciously planning these activities, however, is not an easy 
task as the pricing decisions made at any one stage in the lifetime of a product tend to be 
irreversible and could impact the bottom line dramatically. On the one hand, aggressive 
markdowns may clear the excess inventory fast but could hurt margins as the market-
place could accept higher prices. On the other hand, conservative markdowns may lead 
to unsold inventory that could require deep price discounts to clear at the end of the 
season. In what follows, we look into the specifics of price markdowns primarily with 
respect to how they connect to the problem of clearing the excess inventory. While such 
considerations have been often linked to why retailers are forced into offering mark-
downs, we add to this perspective by briefly referring to other alternative explanations.

---

## Page 183

172  Dynamic and Markdown Pricing
One of these builds on the fact that style and seasonal goods retailers experience long 
lead times and operate in highly uncertain environments. It is not unusual to take such 
a retailer as long as nine months to have its new products delivered in stores (an atypical 
retailer is Zara who has a cycle time of only two to five weeks (Ghemawat & Nueno, 2006)). 
In addition, during the ordering lead time, past trends in customer preferences may change 
dramatically leading to retailers bearing a high obsolescence risk. Popular quotes such as 
“In fashion apparel, there is nothing as boring as last season’s hot sellers” are illustrative of 
the seriousness of the problem (Fisher & Raman, 2010, p. 31). Hence, to manage demand 
uncertainty and stay profitable, retailers tend to introduce their products to the market 
at high margins. For example, percentage gross margins as high as 85% are customary in 
fashion apparel. Of the products on the selling floor, items perceived trendy by customers 
sell well throughout the season and do not need any special intervention. Slow-moving 
items, however, which in the eyes of the customers may appear unjustifiably overpriced, 
tend to lag behind the financial objectives and are typically considered good candidates 
for markdowns. In this situation markdowns can be looked at as mechanisms of demand 
learning (Lazear, 1986; Pashigian, 1988; Pashigian & Bowen, 1991).
Another perspective on what contributes to markdowns being offered sees an item as 
a time-dependent collection of attributes. Specifically, it suggests that the same physi-
cal item is worth more or less based on when in the season the purchase intention is 
expressed. Thus it implies that, throughout the season, such an item could appeal to cus-
tomers with different price sensitivities. A spring season Miss Cristo cork sandal featured 
on the catwalk of the New York Fashion Week in September may appear on the shopping 
list of many shoe lovers. Yet only those who perceive the item as a must-have will subject 
their wallets to the premium price of $595 to get it in the preseason. The rest, however, 
who cannot afford it or may value it at a lower price, may prefer to postpone their pur-
chasing decision, hoping to get it at a lower price. Markdown pricing is perceived in this 
context as a segmentation mechanism intended to differentiate between customers with 
different price sensitivities.
Our digression, while informative, sheds little light on the problems associated with 
price markdowns. In particular, you could ask why we should care about markdowns at 
all. In the absence of any other support material, you could even question our choosing 
to discuss this topic distinctively from the overarching theme of dynamic pricing. Well, 
it turns out that there are good reasons for us to stick to our plan. To help you get the 
feel for the types of problems markdowns may lead to, we adapt the example of the sta-
ple fashion item introduced in Chapter 3 to suit our current needs. For simplicity, let’s 
suppose that the item whose regular retail price is $135 is a seasonal item that costs $35 
to procure from the manufacturer. The retailer would practice in this case a percentage 
markup of 285.7% and a percentage gross margin of 74.1%. Now, let’s further consider 
that the item does not sell well and the retailer is tempted to mark it down to a new retail 
price of $100. The price slash means a recalculated percentage markup of 185.7% and 
a percentage gross margin of 65.0%. In this case, the 9.1% gross margin contraction 
reflects the $35 nominal markdown. Now, let’s suppose that the retailer sells ten units of 
the item at the markdown price of $100 and makes $1,000 in sales. The disturbing real-
ity is that while it has made $650 in profits, the retailer has still lost $350, or 35% of the 
actual sales, due to markdowns.
We build on this admittedly extreme example and illustrate the prevalence of mark-
downs in the modern era using the case of the U.S. department stores. Based on the

---

## Page 184

Dynamic and Markdown Pricing  173
financial and operating results published by the National Retail Federation, the U.S. 
department store markdowns more than tripled between 1971 and 1997 and reached an 
all-time high of close to 30% of sales in 1996 (Fisher, 2009). To illustrate the gravity of 
the problem further, we refer to the recent case of Sears Holdings Corporation, which 
reported a 2008 first-quarter net loss of $56 million that they attributed to the weak 
retail environment and, equally important, markdown-related gross margin contrac-
tions intended to move inventory (Jacobs, 2008). In spite of the overwhelming evidence 
that price markdowns are to be avoided, retailers do it customarily and there are no signs 
that the practice will go away any time soon. So why are markdowns offered? Are they 
really needed and, if so, how should they be handled?
In the last decade, the worrying proliferation of price markdowns has been associated 
with the product customization required by a fickle customer base. In particular, the 
product range flexibility as reflected in the styles, colors, and sizes assorted has commod-
itized and become a qualifying competitive factor rather than an order-winning one. 
This shift has forced style and seasonal goods retailers to respond to the changing market 
requirements by assorting more and more products often only marginally differentiated. 
This in turn has led to a highly uncertain environment in which retailers have been more 
susceptible to make mistakes along their entire supply chain (e.g., forecasting, product 
assortment, purchasing, store allocation, and pricing). The boost in the utilization of 
markdowns is hypothesized to be the result of retailers not being able to cope with the 
increased uncertainty prevalent in their business environments (Pashigian, 1988; Pashi-
gian & Bowen, 1991). For these reasons, in fashion apparel, for example, it is quite infre-
quent that styles perform as per their financial objectives. Some sell out before the end of 
the season while others, stocked in substantial amounts, do not sell at all or sell poorly. In 
the absence of any initiatives to stimulate demand, this slow-moving inventory is likely 
to go obsolete at the end of the season and be salvaged at no or little profit. Markdowns 
in this case are intended primarily to clear this type of inventory. They too generate cash 
to be used to assort other better-selling products. Last but not least they create store 
excitement and increase traffic and sales of complementary products.
Up to this point we have stressed the idea that markdowns are not to be practiced if 
at all possible. Along these lines, retailers able to identify slow-moving inventory early 
in the season may have the option to exchange or return the corresponding products to 
the supplier. We have also emphasized that oftentimes markdowns are to be taken as 
they are the last resort to making profit from a sunk inventory investment. In most cases, 
retailers approach this task statically. Some employ extensions of the Filene’s Basement 
automatic markdown system and offer markdowns based on the time the product spends 
on the shelf—for example, 25% off after 4 weeks, 50% off after 8 weeks, 75% off after 12 
weeks, and charity donation after 16 weeks. Others monitor product performance con-
tinuously and identify slow-moving items that do not sell as per the expectations. Items 
that consistently lag behind are typically marked down during predetermined end-of-
season clearance periods, which, in some instances, may last up to three months. In the 
markdown periods, qualified items are sold at various time-dependent price points (e.g., 
25% off, 50% off, 75% off, multiple of $5 but less than 70% off ) until all excess inventory 
is cleared. These prolonged clearance events, while effective in getting rid of the obso-
lete inventory, do tend to interfere with customers’ in-store experience as the introduc-
tion of new collections overlaps the massive clearance events. Esprit, V&D, and Zara all 
practice this markdown style in parts of Western Europe. To try not to let clearance

---

## Page 185

174  Dynamic and Markdown Pricing
activities spoil the in-store customer shopping experience, some retailers with e-pres-
ence run these events exclusively online. Others, such as Nordstrom through its Nord-
strom Rack chain of stores, prefer to consolidate the in-season leftover merchandise at 
central locations where they attempt to mark it down collectively and profitably sell it.
In recent years some retailers, including Bloomingdale’s and Gap, have started experi-
menting with dynamic in-season markdown policies. Both retailers have come to real-
ize that the static approach to marking down prices is too limiting in that it promotes 
the clearance of inventory in the absence of any sound considerations on how margins 
are impacted. Hence, they have started to rely on optimization software packages to 
compute the optimal timing and depth of the proposed markdowns with the explicit 
goal of maximizing gross margins. These systems use the up-to-date in-season product 
performance together with the continuously adjusted season forecasts to analyze com-
peting pricing scenarios and recommend appropriate markdown policies. The benefits 
of employing dynamic markdown pricing are expected to justify the high capital costs 
associated with a full-scale system implementation. For example, Oracle, one of the soft-
ware vendors with a significant footprint in the retail industry, estimates that its mark-
down optimization solution contributes to a 5%–15% increase in its customers’ gross 
margins (Polonski & Morgan-Vandome, 2009). Similarly, AMR Research, now part of 
Gartner Inc., considers that markdown optimization initiatives have the potential to add 
6%–10% to an organization’s gross margins (AMR Research, 2008).
CASE STUDIES
In this section, we provide some insights into how price markdowns are often approached 
in practice. The first case study builds on the concept of slow-moving items and illus-
trates how to identify profitable markdown opportunities. The second case study uses 
linear programming to solve a simple markdown optimization problem in which rev-
enue maximization is considered explicitly.
Price Markdowns and Slow-Moving Items
Given the significant number of products that they routinely assort, retailers tend to 
track the in-season performance of their merchandise in an attempt to identify timely 
items that are likely to over- or underperform. Often, this effort is undertaken for buy-
ers and supply chain managers to be able to react to the current market conditions. 
For style and seasonal goods retailers, an overperforming item often results in missed 
revenue opportunities as the long order lead times often impedes any effort to restock 
the item. In contrast, items that underperform the market expectations are monitored 
closely as there is a high likelihood for them to go obsolete, requiring salvaging the 
item at no or little profit. Most retailers physically review these items to get an under-
standing of what seems to cause the customer distress and then decide which items to 
mark down. Current practices require pricing managers to wait in their assessment 
until the item introductory period is considered complete. It is not uncommon in the 
fashion apparel retail industry, for example, to compute the first slow-moving indices 
after observing six weeks of demand from the time the item was first introduced. If the 
introductory period is too long, however, the markdown of an item could take place 
at times when customers’ interest for it is considerably reduced (e.g., end-of-season 
clearance events).

---

## Page 186

Dynamic and Markdown Pricing  175
We propose that either no or minimal restrictions be placed on when slow-moving 
indices are computed. If discovered fast enough, some retailers may have an opportunity 
to exchange or return these items to the supplier. For a full coverage of this and other 
related topics, we encourage the savvy reader to consult the material discussed in Walker 
(1999).
To begin our example, suppose that a retail store starts its 16-week fall season with 
1,000 pairs of seasonal Hugo Boss New Wave jeans in stock. For such items, the retailer 
usually plans for a desired maximum end-of-season percentage inventory f
n of 0.15 
(or, equivalently, 150 pairs). The season has started strong with reported sales for the 
first two weeks of 100 and 75 pairs, respectively. Based on this limited information, the 
retailer intends to assess the product performance and start thinking of alternative sell-
ing strategies if sales are not satisfactory. At first glance, it may appear that there are no 
good reasons for the retailer to worry about the sales performance of this product for the 
remaining of the season. This would be a reasonable assumption if the sales trend stays 
the same; the retailer is projected to be out of stock before the end of the twelfth week. 
But what if the trends change? What if customer excitement for this item deteriorated 
as the season progressed? How should the retailer respond to this scenario, and, equally 
important, what should the magnitude of its response be?
It turns out that in the absence of any reliable history-based forecasts, the retailer 
could still compute an end-of-the-season inventory estimate from limited in-season 
available data. In particular, one approach routinely employed by retailers of style and 
seasonal goods involves discounting the end-of-a-period inventory I
j by an inventory 
proportionality factor Fc assumed to stay constant until the end of the season. Following 
the notation in Walker (1999) for consistency, we can write the forecast for the end of the 
season inventory at the end of period j as
in I I F I F F F I Fjc j c
j
c
j
c
n
jc
nj
,,, 0
12
() =⋅ ⋅ ⋅⋅=⋅ ()
+() +() ( )
−
{{ K { ,
where Ij is the available inventory at the end of period  j, n is the length of the selling 
season (e.g., 16 weeks), and  Fc, bounded by 0 and 1, is the inventory proportionality 
factor current at time j. The proportionality factor  Fc, expressed as IIkk
k
j j
−
=
()
⎛
⎝
⎜⎜
⎞
⎠
⎟
⎟
∏ 1
1
1
, 
or, equivalently, ( Ij /I0)1/j, is the geometric mean of the period-to-period less than unit 
growth rates that accompany the move from I0 at the start of the season to Ij at the 
end of the jth time period. Stated otherwise, this forecasting method derives an average 
period-to-period inventory proportionality factor from the observed sales and uses it to 
discount the most current end-of-the-period inventory levels to account for the length 
of the remaining selling season. H. B. Wolfe conducted an extensive study of fashion 
items in several women’s clothing departments and provided the empirical basis for this 
forecasting approach (Wolfe, 1968).
Returning to the example of our retailer, we have enough information to compute the 
end-of-the-season inventory forecasts after the sales for the first and the second weeks 
are reported. Our analytical steps are summarized later and reveal that the item main-
tains a slow-moving status at the end of both weeks. If trends do not change significantly

---

## Page 187

176  Dynamic and Markdown Pricing
in the near future, the retailer may need to find alternative ways of accelerating sales, 
potentially through price markdowns. For illustration purposes only, we also refer to the 
hypothetic case when 125 pairs of jeans are sold in the second week. With only 775 units 
in inventory at the end of the second week, the item changes status to a regular selling 
product that, at least for now, does not require increased monitoring:
Assume now that the retailer takes these early warnings seriously and intends to mark 
down the price of the item to spur sales. The retailer’s intuitive decision to cut the selling 
price, however, triggers a series of subsequent decisions that are slightly more difficult 
to handle. In particular, the retailer needs to investigate if the item qualifies for a mark-
down, and, if so, when and by how much should the price be reduced. On the one hand, 
if there are no legally binding agreements with the manufacturer to preserve the image 
of the brand through consistent pricing, the retailer can attempt to lower the price. On 
the other hand, if it does so, it needs to do it in a way that the markdown is economically 
viable. In what comes next, we focus on this latter task of deciding what markdowns are 
viable at each particular moment in time.
The immediate effect of the retailer’s decision to markdown, at the end of period  j, 
the unit price from, say, P
c to Pm should be a marginal increase in the sales of period 
(j +1). If Sc
j+1 and Sm
j+1 are the expected sales at Pc and Pm, respectively, then Sm
j+1 – Sc
j+1 ≥ 0, 
or, equivalently, (Ij – Ij · (Fm)1) – (Ij – Ij · (Fc)1) ≥ 0. Fm, in this expression, is an unknown 
inventory proportionality factor associated with the unit price being marked down from 
Pc to Pm. Similarly, Ij · (Fm)1 and Ij · (Fc)1 are the end-of-period (j + 1) inventory forecasts 
in the presence of a unit price of Pc and Pm, respectively. Subsequent algebraic operations 
applied to the expression of incremental sales lead to Fc ≥ Fm, which is a necessary but 
insufficient condition to justify the markdown economic viability.
Week 0: 
Week 1: 
              
I
I
FI Ic
0
1
10
11
1 000
900
0
=
=
= () =
,,
..
..
90
900 0 90 185 31
11 5
              
         
iI F c
n
=⋅ () =⋅ () =
−
           Status: Slow Moving Item
Week 2
if n=≥ = ()185 3 150.,
  (Actual): 
              
     
I
FI I I Ic
2
2110
12
825
09 1
=
=⋅() = .
          
              
iI F
i
c
n
=⋅ () =⋅ () =
=
−
2
21 4
825 0 91 214 6
2
..
114 6 150., ≥= ()fn      Status: Slow Moving Item
Week 2 (Hypotheetical): 
              
       
I
FI I I Ic
2
2110
12
775
08 8
=
=⋅() = .
        
              
iI F
i
c
n
=⋅ () =⋅ () =
=
−
2
21 4
775 0 88 130 1
130
..
.. .1 150≤= ()fn      Status: Regular Item

---

## Page 188

Dynamic and Markdown Pricing  177
To uncover sufficient conditions that would warrant a markdown, we link the discus-
sion of the incremental sales for period ( j + 1) to the revenues expected to materialize 
during the remainder of the selling season, or (n – j) time periods. At the full price Pc, the 
retailer is expected to sell items worth Pc · (Ij – Ij · (Fc)n–j), or, Pc · Ij · (1 – (Fc)n–j). By the 
same logic, the revenues to be experienced at the markdown price Pm can be expressed as 
Pm · (Ij – Ij · (Fm)n–j), or Pm · Ij · (1 – (Fm)n–j). In these circumstances, the item is considered 
economically viable for a markdown if and only if the revenues expected to materialize at 
the markdown price Pm equal or exceed those expected to be experienced at the full price 
Pc. In formal terms, this translates into:
 PI F P I F
F F
mj m
nj
cj c
nj
m
nj c
nj
⋅⋅− ()() ≥⋅ ⋅ − ()()
− () ≥ − ()
−−
−
−
11
1 1
, o r
PPPmc
,
 (7.1)
As an aside, note that in Equation (7.1), Fm is bounded by 0 and 1. This necessarily means 
that an economically viable markdown exists if and only if Pm/Pc>1 – (Fc)n–j.
The expression in Equation (7.1) , while informative of how an appropriate mark-
down policy should be approached, is difficult to operationalize as Fm is unknown. In the 
absence of any reliable historical estimates for, the retailer can build on Equation (7.1) 
to get
 
F F
PP
m
c
nj
mc
nj
≤− − ()⎛
⎝
⎜⎜
⎞
⎠
⎟
⎟
− −()
1 1
1
. (7.2)
Using the formulation of expected sales for the end of period ( j +1) in the presence of 
both Pc and Pm, this expression can be rewritten as
 
S
S
FI
FI jnI I P P
j
m
j
c
mj
cj
jm c
+
+
= −() ⋅
−() ⋅ ≥ () =
= () =
−−
1
1
0
1
1
11
1
σ
σ
,, ,
.
− −()⎛
⎝
⎜
⎜⎜
⎞
⎠
⎟
⎟⎟
− ()
−() −()
II
PP
II
j
nj j
mc
nj
j
j
0
1
0
1
1
 (7.3)
to link the expected sales ratio Sm
j+1/Sc
j+1 to a critical ratio σ(.) that can be easily tabulated 
as a function of  j, n, Ij/I0, and Pm/Pc. We provide σ(.) values specific to our application 
in Table 7.1. Similar tables can be devised for selling seasons of different length (i.e., n), 
in-season changing sales data availability (i.e., j), and other relevant inventory and price 
ratios (i.e., Ij/I0 and Pm/Pc, respectively).
.

---

## Page 189

178  Dynamic and Markdown Pricing
To illustrate how the retailer can make use of the information provided in Table 7.1, let 
us assume that every week it can chose three possible markdown values. These correspond 
to the price ratios Pm/Pc of 0.90, 0.75, and 0.50. At the end of week 1, when an inventory 
ratio Ij/I0 of 0.90 is experienced, no economically viable markdowns can be offered at a price 
markdown of 25% or 50% off. A markdown of 10% off, however, seems to be appropriate 
if the sales ratio at the end of week 2, with and without the markdown in place, is expected 
to exceed the critical value of 1.33. As the retailer does not take a permanent price cut after 
the first week, it experiences at the end of the second week an inventory ratio I
j/I0 of 0.83. 
In this case, markdowns valued at 10% or 25% of the initial price seem to be economically 
viable. To be so, however, they must lead to projected increases in sales at the end of week 
3 as reflected by the critical ratios 
σ(.) of 1.26 and 2.52, respectively.
This procedure sheds light on how a retailer could approach the price markdown of 
its slow-moving items. The underlying concepts can be employed repeatedly to resemble 
the mechanics of a dynamic process. This means that at the time the first markdown is 
taken, the entire process is reinitialized to reflect the latest market conditions. Similarly, 
the implementation of all subsequent markdowns is followed by a mandatory model 
parameter value reestimation.
Price Markdowns and Linear Programming
Fashion retailers are often limited by the fashion designers/houses on the timing and 
range of prices they can charge for the brand name merchandise. To gain more control 
Table 7.1 Critical Ratio σ(.) for Assessing the Economic Viability of Price Markdowns
Inventory Ratio Ij /I0
                  Week 1 (j =1) Week 2 (j =2)
              Price Ratio Pm /Pc Price Ratio Pm /Pc
0.90 0.75 0.50 0.90 0.75 0.50
0.99 1.12 1.37 2.17 1.12 1.35 2.07
0.98 1.13 1.41 2.41 1.12 1.36 2.15
0.97 1.14 1.46 2.81 1.12 1.38 2.25
0.96 1.16 1.52 3.80 1.13 1.40 2.37
0.95 1.17 1.61 1.14 1.43 2.52
0.94 1.19 1.73 1.14 1.45 2.73
0.93 1.22 1.91 1.15 1.48 3.02
0.92 1.25 2.29 1.15 1.51 3.50
0.91 1.28 1.16 1.55 4.68
0.90 1.33 1.17 1.59
0.89 1.39 1.18 1.64
0.88 1.49 1.19 1.70
0.87 1.65 1.20 1.77
0.86 2.16 1.21 1.86
0.85 1.22 1.99
0.84 1.24 2.18
0.83 1.26 2.52
0.82 1.27
0.81 1.30
0.80 1.32
Note: n=16; Blank entries refer to cases where an economically viable markdown does not exist.

---

## Page 190

Dynamic and Markdown Pricing  179
over their pricing functions, many of these retailers have developed their own private 
brands (merchandise with fully developed, supported, and advertised brand profiles) 
and/or private labels (fill-in merchandise with no specific brand profiles), which are 
sold exclusively through their network of stores. Macy’s, for example, targets custom-
ers with various needs through its suite of private brands and labels including Alfani 
(men/women), Charter Club (women), Club Room (men), and Greendog (children) 
(for more details, see Macy’s Inc, 2013). Similarly, Saks Fifth Avenue’s Men’s Collection 
and Crown and Bloomingdale’s The Men’s Store attempt to appeal to sophisticated yet 
price-conscious shoppers in need of quality menswear (Palmieri, 2011; Racked Staff, 
2011). The trend has also been embraced by online fashion retailers who could not let 
such an opportunity slip away. The giant ShopBop.com, for example, has introduced its 
own brand, Bop Basics, as an alternative for its customers to the more expensive designer 
collections (Business Insider, 2013). BlueFly.com has tried to achieve similar goals by 
introducing and promoting its private label brands including Harrison, Hayden, and 
Cullen (Bloomberg Businessweek, 2013).
From an operations perspective, private brands/labels allow style and seasonal goods 
retailers to be more responsive to the markets they serve. In particular, since no bind-
ing agreements with the designer/fashion houses are in place to specify tight pricing 
terms and markdown conditions, fashion retailers can use price as an effective means to 
drive profitability. In the absence of any contractual obligations, two actions are often 
employed to immediately impact the retailer’s bottom line. First, retailers with private 
brands/labels are free to set the initial markup as low or as high as they would like as there 
is nothing in place to enforce it to be within a certain range. Second, retailers can take 
immediate actions and consider a price markdown the moment sales drop and an item 
starts to underperform. 
Motivated by the specific issues put forth by the management of private brands/labels, 
we focus on some of the recent efforts of brick-and-mortar and online retailers that 
attempt to streamline their fashion-related markdown practices. In these instances, 
retailers intend to exploit the pricing flexibility that comes with the selling of private 
brands/labels to recommend price markdown strategies that would maximize margins. 
We illustrate this approach using an example from a major online fashion retailer that 
offers collections consisting of a mix of designer and private brand/label items. Some 
conceptual ideas of our approach are present in the work of Caro & Gallien (2012).
For one of its private label items, the retailer starts the new season with 500 units in 
stock. Because the supply of the item comes from overseas, the retailer cannot restock 
the item during the selling season. A typical season at this retailer lasts about 16 weeks. 
The item’s full selling price is €60, which is anticipated to be offered for at least one week. 
If markdowns are needed, the retailer prefers fixed discrete price discounts that can be 
easily communicated to its customers. For this reason, price markdowns of 25% and 
50% off, corresponding to selling prices of €45 and €30, respectively, are considered. 
All markdowns are permanent and irreversible. While still in the preseason, the retailer 
wants to understand what its optimal markdown strategies should be based on various 
probable full-price weekly sales rates. Among these strategies, selling the item at the full 
price throughout the season is preferred. If this is not profitable because of lower-than-
originally expected sales, the retailer wants to explore alternative strategies that account 
for seasonality, inventory depletion effects, and special online events such as the timing 
of e-mail campaigns. Furthermore, once the selling season starts, the retailer wants to

---

## Page 191

180  Dynamic and Markdown Pricing
have dynamic control over its pricing function to be able to revise or implement price 
markdowns that reflect updated market conditions.
In a business environment such as this one, product demand is always difficult to 
predict. In many instances, seasonal products show sales patterns that do not repeat 
from one season to the next. To complicate things further, within the organization itself, 
opinions are typically divergent on how products will likely perform in the marketplace. 
Given the uncertainty that surrounds the demand processes, you may ask how fashion 
retailers can operationalize their markdown initiatives. Often, although individual prod-
uct histories cannot be recycled to get relevant product intelligence, histories of groups 
of similar products can be analyzed to learn the likely demand response of a typical 
group member. For the specific item introduced earlier, the results of such an under-
taking are provided in Table 7.2. To estimate the product group demand models, the 
product group the item belongs to was identified, all items in this group were selected, 
and multiplicative models of the types discussed in Chapter 3 (i.e., model types B-1 and 
B-2) were explored. The product group identification and the within-group product 
selection are inexpensive tasks that are typically driven by the product hierarchies in use 
at the retailer. Finding the preferred model specification(s) is a more involved task that 
builds on existing theory and requires extensive testing and tweaking.
The demand models depicted in Table 7.2 are exponential models of the B-2 type. We 
prefer this functional form over its B-1 counterpart because it performs marginally bet-
ter in regard to the quality of the model fit. Since seasonality within the product group 
appears weak, we do not consider it explicitly. We also prefer to provide only an excerpt 
from the full output since the product sales baselines are irrelevant to the subsequent 
markdown optimization process. In our search for the preferred model specification, 
we build on previous retail studies and find that product group sales are time dependent 
and explained by markdown values and special online events. In spite of our findings, we 
choose to show results for two competing models to subsequently illustrate the impact the 
presence of the special online events has on the expected profitability of recommended 
markdown policies. Focusing on the parameter estimates of the full model, it is obvious 
that price markdowns impact sales nonlinearly. This is an intuitive result that confirms 
to the retailer’s expectations. In addition, within the product group, we observe that sales 
tend to decline toward the end of the items’ selling season. The retailer speculates that 
this behavior is mainly a reflection of the assortment being broken, that is, the on-hand 
inventory not providing a complete selection of colors and sizes. Although more sophis-
ticated approaches can be employed, we model sales’ time dependency and, indirectly, 
the impact of the inventory level and mix using three time-related variables. As shown 
in Table 7.2, the corresponding parameter estimates are all statistically significant and 
quite large in magnitude. For example, all else being equal, the last weeks of the selling 
season are expected to experience about a tenth of the regular sales (i.e., P3 multiplier 
equals 0.13). Last but not least, we note that the special online events such as the e-mail 
campaigns tend to positively impact sales on average by a factor of 1.61.
Although specific to an average group product, the insights gained from the figures in 
Table 7.2 can be used to initialize the computation of the optimal markdown policies. In 
the absence of any sales data in the preseason, the retailer could explore the likely product 
performance using hypothetical weekly sales rates. In season, however, it can decide on the 
best course of action in regard to the pricing of the item based on actual sales rates and con-
tinuously updated product-specific demand multipliers. The differentiation of the latter

---

## Page 192

Table 7.2 Product Group Demand Analysis
Reduced Model Full Model
Coefficient Standard Error t value p value Coefficient Standard Error t value p value
(irrelevant output removed due to space constraints)
Markdown 1.83 0.2 7.5 0.00 1.56 0.2 6.6 0.00
Multiplier 0% off δ1 1.00 1.00
Multiplier 25% off δ2 1.58 1.48
Multiplier 50% off δ3 2.49 2.18
Periods in between 85% and 90% of the selling season (P1) –1.10 0.2 –5.2 0.00 –0.90 0.2 –4.4 0.00
P1 multiplier ξ1 0.33 0.41
Periods in between 90% and 95% of the selling season (P2) –1.77 0.2 –8.4 0.00 –1.53 0.2 –7.4 0.00
P2 multiplier ξ2 0.17 0.22
Periods above 95% of the selling season (P3) –2.28 0.2 –12.1 0.00 –2.04 0.2 –11.0 0.00
P3 multiplier ξ3 0.10 0.13
Special Events (SE) Indicator – – – – 0.48 0.1 4.9 0.00
SE multiplier ς – 1.61
Full Model: Multiplier 25% off 1.48=exp(0.25 × 1.56); P1 multiplier 0.41=exp(–0.90); SE multiplier 1.61=exp(0.48)
Reduced Model: Multiple R-squared: 0.58, Adjusted R-squared: 0.56
Full Model: Multiple R-squared: 0.62, Adjusted R-squared: 0.60

---

## Page 193

182  Dynamic and Markdown Pricing
happens throughout the season when relevant information becomes available. For exam-
ple, all products in a group may start the season with a special online event demand multi-
plier of 1.61 but could end the season with such multipliers in the 1.25–2.50 range, based 
on each product’s independent performance. Updating the multipliers typically requires 
the use of various weighted moving averages of which exponential moving average is the 
most frequently used. Since illustrating the dynamic character of markdown optimization 
is beyond the scope of this discussion, we show next how the retailer can structure its pre-
season markdown initiatives to prepare for more accurate in-season pricing decisions. The 
same underlying markdown mechanism, however, applies to both of these cases.
As part of how it runs its e-business, the retailer sends out customized newsletters 
intended to promote new collections, raise awareness for specific brands or item groups, 
or inform customers of imminent sales opportunities. While the effectiveness of these 
initiatives largely depends on the content of the actual message, the retailer plans to run 
recurrent e-mail campaigns directly targeting our item’s group a week after products are 
introduced to the market and every four weeks thereafter (i.e., weeks 2, 6, 10, and 14). 
These campaigns are of the same type as those we used to estimate the group-level demand 
models shown in Table 7.2. Based on discussions among several buyers at the retailer, a 
consensus has been reached on the market expectations for this important item. In the 
absence of any auxiliary activities, there are high hopes that the product will sell at full price 
at a weekly rate of 25 units. In this context, the initial inventory of 500 units is perceived as 
sufficient to serve the market requirements with a sufficient amount of leftover to create 
some end-of-the-season e-store excitement through permanent markdowns. To investi-
gate possible preseason strategies for in-season markdowns, the retailer can use the group-
level demand multipliers computed previously to adjust the expected baseline sales of 25 
units to account for product life-cycle events such as markdowns, time dependency, and 
special online initiatives. Because after purchasing the items the purchase price becomes a 
sunk cost, the retailer wishes to maximize revenues from the inventory it starts the season 
with such that several market constraints are satisfied. In formal terms, the retailer needs to 
solve the following revenue maximization problem:
max
,
,
zX p D X s
X
ti i i t t
i t
s
ti
=⋅ ⋅ ⋅ () ⋅⋅() +⋅
⋅
= =
∑ ∑ δξ ς
1
3
1
16
s.t.      DDX it t
i t
s⋅() ⋅⋅() += (
= =
∑ ∑ δξ ς
1
3
1
16
500 C1: Inventory constraint ) )
≤∀ ≤ ()
=
∑ Xt
X
ti
i
,
,
,
1
3
11
1 16 C2: Unique or no price constraint
= = ()
−≥ +
1
011 1
 C3: First period full price constraint
XXtt,, , ∀∀≤ ()
+− − +
t
XXXttt
15
12 1 1
C4: Decreasing price constraint 1
,, , XXt
X
t
ti
i
+
=
≥∀ ≤ ()12
1
3
01 5,
,
, C5: Decreasing price constraint 2
∑∑∑ −≥ ∀ ≤ ()+
=
Xtti
i
1
1
3
01 5, , C6: Decreasing price constraint 3
Alll  or  C7: Sign and value restrictionsXXti s, ,=≥ ()01 0

---

## Page 194

Dynamic and Markdown Pricing  183
where Xt,i are 0/1 decision variables that specify whether or not the discrete price pi is to 
be offered in week  t, pi is one of the possible prices in the discrete price set S ={€60.0, 
€45.0, €30.0}, D is the baseline sales of 25 units per week, δi is the demand multiplier cor-
responding to price pi (see Table 7.2 for values for δi), ξt is 1 or ξk based on the position 
of the current week t within the selling season (see Table 7.2 for time brackets and values 
for ξk), ςt is 1 or ς based on whether or not a special online event is scheduled for week t 
(see Table 7.2 for the value for ς), Xs is the inventory left over at the end of the season that 
needs to be salvaged and is the unit salvage value of €10. 
Constraints C1–C7 bound the optimal solution and enforce inventory limitations 
and other operations practices in use at the retailer. Constraint C1 limits the amount of 
inventory the retailer can sell to the initial value of 500 units. Constraints C2 enforce the 
use of a single price point in each of the 16 weeks of the selling horizon. Constraint C3 
makes sure that the item is offered at full price for at least one week. Constraints C4–C6 
implement the common retail practice that stipulates that price markdowns are irrevers-
ible. Lastly, constraint C7 imposes sign and value restrictions on all decision variables. 
Figure 7.1 shows the demand values (D · 
δi) · ξt · ςt, which enter both the objective func-
tion and the C1 constraint. These values are specific to the full model of Table 7.2. To 
repeat the task for the reduced model, we simply update the δ and ξ multipliers appro-
priately and set ς to 1. The corresponding demand profiles should be smoother than 
those depicted in Figure 7.1.
For the reduced and full demand models of Table 7.2, the solutions of the price mark-
down optimization problem are provided in Table 7.3. These results suggest that the 
ξ2 = 1.61
ξ6 = 1.61
ξ10 = 1.61
ξ14 = 1.61
ξ14 = 0.41
ξ15 = 0.22
ξ16 = 0.13
δ3 = 2.18
δ2 = 1.48
δ1 = 1.00
80
60
40
Expected Demand (units)20
0
12345678
Week
9 1 01 11 21 31 41 51 6
Demand Profile €60.0 Demand Profile €45.0
Baseline SalesDemand Profile €30.0
Figure 7.1 Price-Dependent Demand Profiles.

---

## Page 195

184  Dynamic and Markdown Pricing
demand model specifications that describe the item’s market performance lead better 
to more profitable markdown strategies. In this example, by modeling the impact of the 
special online events explicitly, the retailer is advised to markdown its full price to €45 in 
week 7, which follows the anticipated e-mail campaign of week 6. In the absence of this 
intelligence, the retailer is advised to reduce the price to €45 in week 4 or soon after the 
first e-mail campaign of week 2.
Just because the retailer possesses this type of information before the season starts does 
not mean that the retailer should stick to this plan once actual demand for the item starts 
to become available. In particular, once the season starts, the retailer should confirm the 
hypothetical baseline sales used in the preseason markdown optimization exercise. The 
actual sales, once available, could be used then to rerun the optimization procedure and 
adjust the depth and the timing of the suggested markdowns. In addition, all product 
group demand multipliers can be revised in season to reflect the item’s actual perform-
ance. By dynamically resolving the markdown optimization with updated information, 
revenues can be maximized and end-of-the-season spoilage can be minimized.
SUMMARY
Dynamic pricing is the practice of continuously adjusting prices to maximize profit by 
shaping demand (through price changes) to meet the available supply. In this chapter, 
we provide an understanding of how dynamic pricing has evolved and moved out of the 
traditional travel and hospitality industry boundaries to become the new thing in non-
traditional industries such as retailing, utilities, sports events, and the arts. One of the 
reasons for its increased adoption is the fact that it is now often technologically feasible 
for each customer to be quoted her own price. We also discuss some contextual factors 
and subjective situations that impede organizations from employing dynamic pricing 
successfully.
In light of the trends that have reshaped the style and seasonal goods retailing, we offer 
some perspectives on why permanent price markdowns—a particular form of dynamic 
pricing—are used so frequently. While their primary role involves permanent reduc-
tions in price in order to clear excess inventory off the sales floor, price markdowns 
are also sometimes used as demand learning or segmentation mechanisms. Oftentimes, 
however, the clearing of excess inventory in the absence of any other considerations can 
be detrimental to an organization. Thus we discuss a relatively newer trend of creating 
optimal price markdown policies with the explicit goal of maximizing gross margins.
We conclude the chapter with two case studies that illustrate how price markdowns 
are often dealt with in practice. In the first case study, we show how organizations can 
Table 7.3 Preseason Optimal Markdown Policies
Expected Revenue (€) Markdown Policy
Reduced Model 23,403.1 Sell at €60.0 for 3 weeks.
Switch to €45.0 in week 4.
Sell at €45.0 until the end of the season.
Full Model 25,156.1 Sell at €60.0 for 6 weeks.
Switch to €45.0 in week 7.
Sell at €45.0 until the end of the season.

---

## Page 196

Dynamic and Markdown Pricing  185
identify profitable markdown opportunities for their slow-moving items. In the second, 
we highlight how organizations can rely on more sophisticated techniques to optimize 
their markdown policies such that revenues/profits are maximized.
REFERENCES
AMR Research. (2008). Lifecycle price management—Winning in a down economy. Paper presented at the 6th 
Annual Retail Technology Summit, Berlin Germany, October 15–16.
Bichler, M., Kalagnanam, J., Katircioglu, K., King, A. J., Lawrence, R. D., Lee, H. S., et al. (2002). Applications of 
flexible pricing in business-to-business electronic commerce. IBM Systems Journal, 41(2), 287–302.
Bloomberg Businessweek. (2013). Company overview of Bluefly Inc. Accessed June 27, 2013. Retrieved from http://
investing.businessweek.com/research/stocks/private/snapshot.asp?privcapId=106427.
Business Insider. (2013). Shopbop. Accessed June 27, 2013. Retrieved from www.businessinsider.com/
blackboard/shopbop.
Carlson Hotels Worldwide. (2009). Carlson Hotels breaks the property system paradigm (press release). Accessed 
June 26, 2013. Retrieved from www.revenueanalytics.com/pdf/601_IHG_Press_Release.pdf.
Caro, F., & Gallien, J. (2012). Clearance pricing optimization for a fast-fashion retailer. Operations Research, 60(6), 
1404–1422.
Elmaghraby, W., & Keskinocak, P. (2003). Dynamic pricing in the presence of inventory considerations: Research 
overview, current practices, and future directions. Management Science, 49(10), 1287–1309.
eMarketer. (2013). Dynamic pricing: What retailers need to know about competing in real time Retrieved from www.
emarketer.com.
Fisher, M. L. (2009). Rocket science retailing: The 2006 Philip McCord Morse lecture. Operations Research, 57(3), 
527–540.
Fisher, M. L., & Raman, A. (2010). The new science of retailing: How analytics are transforming the supply chain and 
improving performance. Boston, MA: Harvard Business School Press.
Gallego, G., & van Ryzin, G. J. (1994). Optimal dynamic pricing of inventories with stochastic demand over finite 
horizons. Management Science, 40(8), 999–1020.
Ghemawat, P., & Nueno, J. L. (2006). ZARA: Fast fashion. Case Study 9-703-497, Boston, MA: Harvard Business 
School, Harvard University.
InterContinental Hotels Group. (2009). IHG launches price optimization module (press release). Accessed June 26, 
2013. Retrieved from www.revenueanalytics.com/pdf/601_IHG_Press_Release.pdf. 
Jacobs, K. (2008). Sears Holdings posts unexpected loss on markdowns. Accessed June 26, 2013. Retrieved from www.
reuters.com.
Lazear, E. P. (1986). Retail pricing and clearance sales. American Economic Review, 76(1), 14–32.
Macy’s Inc. (2013). Private brands. Accessed June 27, 2013. Retrieved from www.macysinc.com/macys/
private-brands/.
Narahari, Y., Raju, C. V. L., Ravikumar, K., & Shah, S. (2005). Dynamic pricing models for electronic business. 
Sadhana, 30(2–3), 231–256.
Palmieri, J. E. (2011). A man’s world: The men’s wear strategy evolves. Accessed June 27, 2013. Retrieved from www.
wwd.com/images/processed/newsletters_ads/wwd/2012/01/Articlewwd-2011-12-05.pdf.
Pashigian, B. P. (1988). Demand uncertainty and sales: A study of fashion and markdown pricing. The American 
Economic Review, 78(5), 936–953.
Pashigian, B. P., & Bowen, B. (1991). Why are products sold on sale? Explanations of pricing regularities.  The 
Quarterly Journal of Economics, 106(4), 1015–1038.
Polonski, J., & Morgan-Vandome, A. (2009). Oracle retail solution: Retail application footprint. Paper presented 
at the North American Retail Partner Summit, January 28.
Racked Staff. (2011). Sneak peek: Saks Fifth Avenue Men’s Collection for Pre-Fall & Fall. Accessed June 27, 2013. 
Retrieved from http://racked.com/archives/2011/05/13/sneak-peek-saks-fifth-avenue-mens-collection-for-
prefall-fall.php.
Talluri, K. T., & van Ryzin, G. J. (2004). The theory and practice of revenue management. New York, NY: Springer 
Science + Business Media Inc.
Walker, J. (1999). A model for determining price markdowns of seasonal merchandise. Journal of Product & Brand 
Management, 8(4), 352–361.
Wolfe, H. B. (1968). A model for control of style merchandise. Industrial Management Review, 9(2), 69–82.

---

## Page 197

8
PRICING IN BUSINESS-TO-BUSINESS ENVIRONMENTS
INTRODUCTION
In contrast to the pricing decisions discussed in the previous chapters, which involve 
estimating a price-quantity relationship, business-to-business (B2B) environments 
often involve a single bid opportunity where the entire bid is either won or lost. In such 
business environments, companies are often required to respond to a potential client’s 
requests-for-proposal (RFPs) with a personalized offer. The customized response to 
these RFPs reflects the unique customer-company trade conditions and is frequently 
accompanied by customer-tailored prices that try to balance decreasing margins with 
increasing bid success probabilities. While customized pricing has always been a com-
mon practice in such environments, the actual task of determining the customized price 
has historically been based purely on the experience and judgment of the salesperson 
responsible for the customer’s account.
More recently, analytical models for customized pricing have been successfully imple-
mented in industries as diverse as package delivery (Kniple, 2006), building products dis-
tribution (Dudziak, 2006), and hotel event space (Hormby & Morrison, 2008; Hormby, 
Morrison, Dave, Meyers, & Tenca, 2010). The models have also been used in the busi-
ness-to-consumer (B2C) market in the financial services industry to help banks deter-
mine what interest rate to offer when responding to requests for mortgages, credit cards, 
and car loans (Kadet, 2008; Phillips, 2005b). The financial improvement from using 
customized pricing models can be significant. UPS, for example, reported an increase in 
profits of more than $100 million per year by optimizing its price offerings using cus-
tomized pricing models (Boyd et al., 2005).
In a typical B2B environment, price optimization relies on models that incorporate 
insights gained from the bidding history into the current pricing decisions. Specifi-
cally, by using the information on past wins and losses, models are estimated to express 
the probability of winning the bid as a function of the offered price. These probability 
curves are commonly termed bid-response functions. The two bid-response probability 
186

---

## Page 198

Pricing in Business-to-Business Environments  187
functions previously introduced in Chapter 6 are the logit and power models (Agrawal 
& Ferguson, 2007; Boyd et al., 2005; Ferguson, 2010; Phillips, 2005a). Both are inverse 
S-shaped and approach one and zero at low and high prices, respectively. The latter of 
these points holds true if and only if the scale parameters D and C are set to 1.0 (for 
details on this issue see Chapter 6). If all firms were homogeneous in their probability 
of accepting a bid for a given price, the bid-response functions would be the same for all 
potential firms and the result of the price optimization would be a single price quoted 
for every bid opportunity.
In practice, however, firms are often heterogeneous in their price sensitivity as pre-
dicted by certain customer attributes such as size, location, or the length of time a cus-
tomer has had a relationship with the bidding firm. Not surprisingly, determining which 
of the many possible customer attributes are good predictors of a potential firm’s price 
sensitivity is often a difficult task for a salesperson who may respond to hundreds or even 
thousands of RFPs per year. Thus the fact that bid-response functions can include, and 
in some cases test the significance of, these different customer attributes makes them 
attractive tools for firms that desire a more standardized (and analytical) approach to 
B2B pricing. More specifically, bid-response functions use customers’ attribute data 
along with the firm’s historical win/loss data from past bid opportunities to test which 
attributes are most useful in segmenting customers. Furthermore, they also support the 
analytical optimization of the price for future bid opportunities based on the significant 
segmentation groups that were determined using the model-fitting procedures.
Price segments are defined as sets of transactions, classified by customer, product, 
and transaction attributes, which exhibit similar price sensitivities. Customer attributes 
may include customer location, size of the market the customer is in, type of business 
the customer is in, the way the customer uses the product, customer purchase frequency, 
customer size, and customer purchasing sophistication. Product attributes may include 
product type, life-cycle stage, and the degree of commoditization. Transaction attributes 
may include order size, other products on the order, channel (the potential buyer is 
reached through), specific competitors, when the order is placed, and the urgency of the 
bidder. In addition, some models assume knowledge of the historical and current bid 
price of competing firms participating in the bid opportunity.
A common characteristic of environments where companies employ customized pric-
ing models occurs when the bidder with the lowest price does not always win the bid. 
Thus markets are characterized by product differentiation where a given firm may com-
mand a positive price premium over its competitors, dependent on the particular cus-
tomer requesting the bid response. Sometimes even bids from the same customer may 
contain some inherent amount of uncertainty in the bid-winning probability because the 
bid-requesting firm randomly allocates its business to different competitors to ensure a 
competitive market for future bids. Because of these practices, a firm will never be able to 
remove all uncertainty from the bid-price response process and must work with proba-
bilistic models.
A second common characteristic of an appropriate customized pricing environment 
occurs when the size of the bid opportunities is not large enough to justify a sales person 
dedicated to each customer. Instead, a single sales person may respond to multiple bid 
opportunities from a variety of potential customers each day. The most common alterna-
tives to using customized pricing models are either to charge a fixed price to all custom-
ers or to have a sales agent respond to each separate bid opportunity with a customized

---

## Page 199

188  Pricing in Business-to-Business Environments
price. Charging a fixed price leads to missed opportunities to price discriminate among 
different customer segments—a practice that has been well publicized for significantly 
increasing a firm’s profit in many different industries. The other alternative, relying on a 
sales agent to respond to multiple bid opportunities, is also problematic. Theoretically, 
the sales agent should have knowledge of the market, based on the customer’s history of 
former bid responses, allowing the sales agent to customize a price that optimizes this 
inherent trade-off between decreasing margins, due to lowering the price, and increasing 
probabilities of winning the bid. In reality, sales agents often do not make good trade-off 
decisions in these situations because of a lack of historical knowledge, the inability to 
process this historical knowledge into probability distributions, or misaligned incen-
tives (Garrow, Ferguson, Keskinocak, & Swann, 2006). The judicious use of customized 
pricing models allows firms to capture historical bid information, analyze it, and present 
nonbiased price recommendations for future bidding opportunities. If there is addi-
tional information available regarding the bidding opportunity that cannot be captured 
in the model, the model’s recommended price may serve as one of many possible inputs 
to the person responsible for making the bid-response decision. Additional background 
and information on where customized pricing models are best applied can be found in 
Phillips (2005a).
RELATION TO TRADITIONAL PRICE OPTIMIZATION
The practice of price optimization is well known for applications where the demand for a 
product over a certain period of time is correlated with the price charged for the product 
over the same time period. In such a situation, a firm can measure the demand at dif-
ferent price points for a product and use this data to estimate a price-response function. 
This traditional application to price optimization works well in environments where 
there are a large number of potential customers who each may buy a small quantity of 
the product (e.g., consumer retail stores) or where a small number of potential custom-
ers purchase large quantities of a product but spread their purchases over many suppli-
ers (e.g., commodity spot markets such as grain, steel, or oil). It is less helpful, however, 
in winner-takes-all bidding situations that are common in B2B transactions, where the 
customer commits to purchase a given quantity of goods or services and solicits bids 
from a set of firms capable of providing that quantity. In these situations, the decision 
a providing firm is concerned about is not if (or how much) the customer will buy but 
rather will the customer buy from the firm as opposed to one of its competitors. Thus 
the provider firm does not face a decision of what price to place on a product to attract 
demand but instead what price to quote to this particular customer to win this particular 
bid opportunity (customized pricing).
Panel A in Figure 8.1 shows a historical demand plot for a customized pricing sce-
nario. Notice that the wins (jittered and shown around the horizontal line positioned at 
the y-value of one) are more common for the lower prices while the losses (jittered and 
shown around the horizontal line positioned at the y-value of zero) are more common 
for the higher prices.
The data captured in panel A in Figure 8.1 is the historical win/loss data for a firm 
over 140 past bid opportunities for the same product. Judging from the data, it appears 
that the average price offered has been around $10 per unit but the firm has historically 
priced as low as $8 and as high as a little over $12. It also appears that a lower-than-

---

## Page 200

Pricing in Business-to-Business Environments  189
average price does not guarantee a win, nor does a higher-than-average price guarantee a 
loss—there is some uncertainty in how the prospective demand responds to the offered 
price. Therefore, we will focus on maximizing the firm’s expected profit, consisting of 
the total profit assuming the firm wins the bid (margin multiplied by the quantity Q) 
times the probability of winning a bid for a given price, which we label 
ρ (P) ∈ [0,1]. 
Thus the firm’s expected profit is π (P) = ρ (P) (P – C) Q, where P is the price offered, C 
is the unit cost and Q is the quantity requested.
ESTIMATING THE PROBABILITY FUNCTION
Once ρ (P) is estimated, the actual price optimization part for the problem is straight-
forward and differs little from the traditional linear demand problem. The difficulty, of 
course, lies in estimating ρ (P). Before we discuss some various methods of doing so, it 
is helpful to define some properties that any estimated function should possess. First, 
the function should decrease monotonically as the price increases. Second, the function 
should be bounded by 0 and 1 (see panel B in Figure 8.1).
While there are several models that provide a reverse S-shaped probability function, 
the most common model used in practice is the logit model, a model similar in spirit to 
the one described in Chapter 6. This model is described in Boyd et al. (2005) and Phillips 
(2005a) and is compared against a competing model in Agrawal and Ferguson (2007). As 
a review, the logit model is represented by
 
ρ P Ce
e
ab P
ab P() = ⋅
+
+⋅
+⋅1
, (8.1)
where C = 1 and a and b are parameters that must be estimated to fit the historical win/
loss data. The parameter estimation is performed by minimizing the squared errors of 
the residuals or by using maximum-likelihood estimates. Before computing the parame-
ter estimates of the models, however, it is important to divide the historical win/loss data 
1.0
0.8
0.6
Win = 1, Loss = 0
0.4
0.2
0.0
89
Price ($)
(A)
10 11 12
1.0
0.8
0.6
Win Probability
0.4
0.2
0.0
89
Price ($)
(B)
10 11 12
Figure 8.1 (A) Historical Demand Data for Customized Pricing, (B) Fitted Reverse S-Shaped Probability Function to Win/
Loss Data

---

## Page 201

190  Pricing in Business-to-Business Environments
set into two segments: one for estimating the parameter values and the other for measur-
ing the fit. Similar to time series forecasting models, measuring the goodness-of-fit on 
the same data as the parameter values may result in a misleadingly close fit as compared 
to testing the model on a holdout sample. Phillips (2005a) describes how each estimation 
method is applied to the logit function (8.1). In general, if we define each historical bid 
opportunity with the subscript i (with W
i representing the indicator response variable, 1 
= win and 0 = loss, and Pi representing the firm’s price response for bid opportunity i), 
the most common estimation method is to choose parameter values (a, b) that maximize 
the likelihood of the observed values, that is, the likelihood function provided below:
 ρρPa b Pa bi
W
i
W
i
i i
,,() ⋅− ()()⎛
⎝⎜
⎞
⎠⎟
−()
∏ 1
1
. (8.2)
PRICE OPTIMIZATION FOR CUSTOMIZED PRICING
We now look at how customized pricing probability models are used in price optimi-
zation. For the discussion that follows, our objective is to maximize expected profits. 
However, other strategic or operational objectives can be easily accommodated such as 
increasing market share or including constraints on capacity, inventory, price, or mar-
gin. In addition, the firm is assumed to be risk-neutral in this example. A risk-averse 
firm may prefer to optimize expected revenue with a concave utility function so as to 
mitigate the chances of bad individual outcomes. The price optimization problem for a 
prospective bid opportunity i (with Q
i now representing the quantity that is requested 
in bid i) becomes:
 Max P P P C Q
P ii ii
i
 πρ() = () ⋅−() ⋅ . (8.3)
Note that in equation (8.3) the margin (Pi – C) is strictly increasing in price (see panel 
A in Figure 8.2) but the probability of winning the bid is strictly decreasing in price (see 
panel B in Figure 8.2 ). Therefore, the expected profit is often a unimodal function as 
shown in panel C in Figure 8.2.
Determining the optimal price involves finding a global maximum for the expected 
profit shown in equation (8.3). Since the profit function is unimodal, any search-based 
optimization algorithm can be used to solve for the price that maximizes profit, includ-
ing the solver package available in Microsoft Excel. The profit-maximizing price can also 
be found by solving for the price where the elasticity of the expected profit function is 
equal to the inverse of the marginal contribution ratio.
SEGMENTING CUSTOMERS BASED ON HISTORICAL 
PRICE BEHAVIOR
The basic logit model described in equations (8.1) and (8.2) only includes the price as 
a predictor of the probability of winning a bid. This model is appropriate if there are 
no discernable differences in the price sensitivity of a firm’s customer set; for every bid 
opportunity, every customer has the same probability of accepting the firm’s bid at a 
given price. In this situation, the customized price optimization equation (8.3) will rec-
ommend the same optimal price for every future bid opportunity. In practice, this is

---

## Page 202

Pricing in Business-to-Business Environments  191
rarely the case—if it was, then why would the firm be applying customized pricing to 
begin with? A more common scenario is one where a firm’s sales force has historically set 
different prices for each bid opportunity based on certain characteristics of the bid or of 
the customer requesting the bid. The characteristics driving the different prices, which 
may even differ by salespersons within a firm, may include such things as the size of the 
customer (annual revenue), the length of time a firm has been a customer, the quantity 
requested by the bid, or the number of firms invited to submit to this particular bidding 
opportunity. Thus a bid opportunity from a small customer who has had a long-term 
relationship with the firm and typically involves only two additional firms in the bidding 
process may receive a higher price quote than a large customer with little sales history 
who includes at least five competitive quotes in every bid opportunity. In an interest-
ing example of customized pricing in the banking industry, Kadet (2008) describes how 
some banks place consumers into pricing segments and quote customized interest rates 
each time a potential customer shops for a loan. It is exactly this case, when customers 
can be segmented based on their price sensitivities, that customized pricing models pro-
vide the largest benefit.
The logit model in equation (8.1) can be expanded to include segmentation variables. 
Figure 8.2 (A) Marginal Deal Contribution vs. Unit Price, (B) Win Probability vs. Unit Price, (C) Expected Profit vs. Unit Price
5
4
3
Margin ($) (Cost = $7.0)
2
1
89
Price ($)
(A)
10 11 12
1.0
0.8
0.6
Win Probability
0.4
0.2
0.0
89
Price ($)
(B)
10 11 12
160
120
80
Expected Profit ($)
40
89
Price ($)
(C)
10 11 12

---

## Page 203

192  Pricing in Business-to-Business Environments
To show how this can be done, we use an example from an application of customized 
pricing at a major credit bureau, which is a real company that we will call Alpha Com-
pany because of the sensitive nature of the data set. Alpha sells credit scores of individu-
als to businesses that extend credit to their customers, such as car dealerships and jewelry 
stores. If an individual purchases his or her credit score, there is a list price of around 
$10. Businesses that purchase multiple credit scores annually often send out bids to the 
three largest credit bureaus, promising a minimum volume of score requests per year in 
exchange for a discounted price. Alpha is typically included in these bid opportunities, so 
it has a substantial historical database that includes each past bid opportunity, the size of 
the minimum quantity promised in each contract, and the length of time in months that 
the business requesting the bid has been a customer of Alpha. We denote the quantity of 
each bid by Q and the length of the relationship with Alpha in months by M. In addition, 
we define c as the coefficient for the quantity parameter and d as the coefficient for the 
length of the relationship. Including these new variables and coefficients into equation 
(8.1) results in:
 
ρ PQ M e
e
ab Pc Qd M
ab Pc Qd M|,() =
+
+⋅ +⋅ +⋅
+⋅ +⋅ +⋅1
. (8.4)
The estimation of the set of coefficients ( a, b, c, d) is performed through a maximum 
likelihood fit. It still remains, however, to determine what segmentation variables should 
be included in the model. Just because a firm has historical data for a segmentation vari-
able does not mean that it should be included in the model. Next, we will explain how to 
determine whether a segmentation variable should be included.
Many different approaches to segment data exist. The number and type of segments 
can be determined in advance (a priori), by asking, for example, the sales team what 
customer characteristics they use when determining the price to respond to a bid. While 
this knowledge (perhaps based on years of experience) should not be discounted, it 
should, however, be statistically tested. There are many cases where a firm implement-
ing a customized pricing model finds, when doing so, that many of the characteristics it 
has historically used to segment customers are not statistically significant based on the 
historical sales data. Thus it is also useful to determine (or confirm) customer segments 
based on data analyses (post hoc). Some methods for determining customer segments 
include nonoverlapping and overlapping clustering methods, classification and regres-
sion trees, and mixture (latent class) regression models. A detailed analysis of these meth-
ods is beyond the scope of this chapter, but we refer the reader to Wedel and Kamakura 
(2000) for a detailed overview. In most situations, the easiest and most popular method, 
however, is to estimate a multivariate logistic regression model (Hosmer & Lemeshow, 
2000; Kutner, Nachtsheim, & Neter, 2004). This technique is available in most statistical 
software packages and, similar to linear regression, a statistical significance test can be 
applied to the predictor variables. Estimating the win/loss probability as a function of 
price, quantity and active months by running a logistic regression on Alpha’s data results 
in the output shown in Table 8.1.
Observing the p values in the logistic regression output table shows that only the inter-
cept, the price, and the active months are significant at the 95% level ( p value less than 
0.05). Thus the quantity variable is dropped from the model and a second regression is 
run using only the significant variables. The estimated coefficients of the variables from

---

## Page 204

Pricing in Business-to-Business Environments  193
the second logistic regression are shown in Table 8.2. Substituting the estimated coef-
ficient values into equation (8.4) leaves
 ρ PM e
e
e
e
ab Pd M
ab Pd M
PM
|
.. .
.() =
+
=
+
+⋅ +⋅
+⋅ +⋅
−⋅ +⋅
11
2 716 1 180 0 140
27 116 1 180 0 140−⋅ +⋅.. PM . (8.5)
The fact that quantity was not a significant segmentation variable was a surprise to the 
sales team at Alpha. Prior to this study, the team members felt that the quantity requested 
in a bid was a better indicator of the price sensitivity of the customer than the length of 
time the customer had been doing business with Alpha. Of course, there may be other 
significant segmentation variables that were not included in the model, such as geo-
graphic location, company size, and so on. Moving forward, Alpha plans on collecting 
additional information on each bidding opportunity so that other possible segmentation 
variables can be tested. In general, the number of customer attributes (segments) that 
can be accurately estimated depends on the amount of historical bid information avail-
able. If extensive historical data are available, greater degrees of segmentation can be 
achieved without compromising the accuracy and robustness of the statistical estimation 
of the parameter values.
While building statistically significant probability models is important, what firms 
really care about are improvements in profits. In the next section, we show how to test 
the performance of a customized pricing model.
MEASURING PERFORMANCE
We alluded to the point earlier that the historical win/loss data should be divided into an 
estimation set and a holdout sample set. A holdout set is critical for obtaining a realistic 
measure of the model’s performance; it is misleading to measure performance on the 
Table 8.2 Output From Logistic Regression After Removing Quantity
Variable Coefficient Standard Error z value p value
Intercept 2.716 1.018 2.669 0.008
Price -1.180 0.425 –2.774 0.006
Active Months 0.140 0.041 3.377 0.001
Descriptive statistics Price ($):
min = 0.58; Q1 = 2.00; Q2 = 2.24; mean = 2.33; Q3 = 2.52; max = 4.19
Table 8.1 Output From Logistic Regression on Alpha’s Historical Win/Loss Data
Variable Coefficient Standard Error z value p value
Intercept 3.124 1.095 2.852 0.004
Price –1.253 0.433 –2.896 0.004
Quantity 0.000 0.000 –1.075 0.282
Active Months 0.141 0.042 3.381 0.001
Descriptive statistics Price ($): 
min = 0.58; Q1 = 2.00; Q2 = 2.24; mean = 2.33; Q3 = 2.52; max = 4.19

---

## Page 205

194  Pricing in Business-to-Business Environments
same data that was used to estimate the logistic regression model’s coefficients. There are 
two performance metrics available: percent improvement in profits over unoptimized 
actual profits and percent improvement in profits over unoptimized expected profits. 
To understand the difference between the two performance metrics, consider the bid 
opportunity from Alpha’s historical win/loss data in Table 8.3.
Applying the logit model from equation (8.5) to the bid opportunity and optimizing 
results in an optimal price of $2.62 for this particular bid opportunity. Substituting the 
original bid price of $2.00 into equation (8.5) results in the probability of winning for 
the unoptimized bid of 0.814 or 81.4%. Substituting the optimal price results in a prob-
ability of winning for the optimized bid of 0.677 or 67.7%.
Since Alpha’s marginal cost of providing a credit score is essentially zero, the actual 
profit from this bid opportunity is (Original Bid Price – Marginal Cost) Quantity 
Requested Win/Loss Indicator Variable = $(2.00 – 0.00) 4,800 1 = $9,600. If the origi-
nal bid had resulted in a loss, the actual profit would be zero. The original bid expected 
profit is (Original Bid Price – Marginal Cost) Quantity Requested Win Probability at 
the Original Bid Price = $(2.00 – 0.00)* 4,800* 0.814 = $7,814.40. Note that the expected 
profit is always smaller than the actual profit when the bid was won, and is always larger 
when the bid was lost. The optimized bid expected profit is (Optimized Bid Price – Mar-
ginal Cost) Quantity Requested Win Probability at the Optimized Bid Price = $(2.62 
– 0.00)* 4,800* 0.677 = $8,513.95. These expected profits can then be used to calculate 
the two performance measure for this bid opportunity as follows:
 Percent improvement in optimized bid expected profits over unoptimized bid 
actual profits = ($8,513.95 – $ 9,600.00) / $9,600.00* 100 = –11.31%.
 Percent improvement in optimized bid expected profits over unoptimized bid 
expected profits = ($8,513.95 – $7,814.40) / $7,814.40* 100 = 8.95%.
The actual and expected profit calculations should be performed for every bid opportu-
nity in the holdout set and the sum of each of these profits (over all bid opportunities in 
the holdout set) can then be used to compute the performance measures for the model. 
For this data set (holdout sample equal to 146 historical bids), the total percent improve-
ment in optimized bid expected profits over unoptimized actual profits was 19%. The 
percent improvement in optimized bid expected profits over unoptimized bid expected 
profits was 13.4%.
Table 8.3 Bid Characteristics
Bid Identifier 78
Win (Won=1; Loss=0) 1
Quantity Requested 4,800
Active Months 8
Original Bid Price ($) 2.00
Optimal Bid Price ($) 2.62
Win Probability at Original Bid Price 0.814
Win Probability at Optimized Bid Price 0.677

---

## Page 206

Pricing in Business-to-Business Environments  195
IMPLEMENTING A CUSTOMIZED PRICING 
OPTIMIZATION PACKAGE
Thus far, we have focused on the technical aspects of customized pricing optimization. 
What is clearly evident, however, from the presentations by individuals whose firms have 
implemented customized pricing models is that the most difficult part of an implemen-
tation is not the proof of the value of the system, nor is it building the models and per-
forming the price optimizations. Instead, the most quoted difficulty involves the accept-
ance of the system’s price recommendations by the existing sales team. The removal of 
some decision-making authority away from individuals to a more automated system is 
problematic in any environment, but it is particularly difficult for pricing, since the sales 
team may feel that the ability to generate customized price quotes is a large part of the 
value its members bring to the firm and the incentive system (often a commission based 
on total revenue) may not match the profit maximization objective of a customized pric-
ing optimization system.
Are there best practices that may be applied to help mitigate these problems given 
the almost certain cultural issues and expected resistance to a system implementation? 
It turns out that there are some practices that seem to help, based on the same panel 
discussions referenced earlier. The most frequently suggested technique is to treat the 
customized price optimizer as a decision support tool for the sales team rather than a 
system that will automatically set prices for all future bid opportunities. No automated 
pricing system will ever completely replace the ability of humans to factor in extenuating 
circumstances or information that is not captured in the historical sales data. Of course, 
sales personnel often overemphasize the value of human judgment so there needs to be 
some incentive to follow the recommendations of the pricing models. One such incen-
tive that has worked for several firms is to track the frequency that a sales person sets a 
price within the recommended range from the pricing model and then publish these 
results along with the monthly profits made by each sales person. If, as expected, the 
sales personnel ranked the highest for pricing within the recommended price ranges are 
also ranked the highest for monthly profits, then the rest of the sales team will copy this 
practice to improve their own performance.
CASE STUDY: INTEREST RATE OPTIMIZATION AT A U.S. 
ONLINE AUTO LENDER
In this section, we provide a case study of how to implement a customized pricing deci-
sion support system. Although the case study explores the specifics of a business-to-con-
sumer (B2C) environment, the discussion and the approach are relevant to both B2B 
and B2C environments. For convenience, we look into the example of a U.S. online auto 
lender for which data is available upon request from the Center for Pricing and Revenue 
Management (CPRM) at Columbia University (www7.gsb.columbia.edu/cprm/). The 
CPRM data set consists of all applications that an online auto lender approved during 
the time period between July 2002 and November 2004.
Although the auto lender focuses exclusively on serving the online market, its busi-
ness model follows closely the procedures routinely employed by the traditional offline 
financial institutions. Specifically, a prospective customer who intends to acquire a new/
used automobile and would like to finance her purchase could apply for a loan by sub-
mitting an online application via the auto lender’s website. The website receives both

---

## Page 207

196  Pricing in Business-to-Business Environments
direct and referral traffic. Upon the receipt of the application, the auto lender evaluates 
the credit worthiness of the applicant (i.e., the likelihood of the applicant’s defaulting 
on her debt obligations) and provides her with an approval notice if an approval deci-
sion is granted. An approved loan application is accompanied by a customized annual 
percent rate (APR) that reflects such things as the amount requested, the term of the 
loan or the loan’s perceived risk of default. Upon the receipt of the approval notice, the 
prospective borrower evaluates the competitiveness of the offer and decides whether or 
not to take up the loan during a grace period of 45 days. If the loan is not taken up dur-
ing this period, the prospective customer is recorded as lost in regard to this particular 
loan application.
As it is readily apparent from the exposition above, one of the critical profit decisions 
the auto lender needs to make relates to what APR to quote the prospective borrower. 
In the case where the applicant accepts the offer, a high APR leads to high profits; in 
general, however, a high APR is typically associated with a relatively low win probability. 
Conversely, a low APR may easily win business for the auto lender but the corresponding 
profits are small and may turn into significant losses if the borrower defaults. To satisfy 
this high (low) profit—low (high) win probability trade-off, the auto lender can opti-
mize how it computes the quoted APRs so as to maximize its expected profits. Following 
the discussion before equation (8.3), the auto lender should quote a loan application i 
with a customized APR that maximizes the expected profit:
 
πρAPR APR X APR PR Amount Term PoP LGDik i i i() = () ⋅ ()∏|, , , , ,, , (8.6)
where Xi,k are some k attributes that intrinsically describe loan application i (e.g., Amounti, 
Termi); ρ (APR | Xi,k) is the take up probability conditional on the loan attributes Xi,k (i.e., 
the bid-response function discussed extensively throughout this chapter); Π (APR, …) 
is the auto lender’s expected profit assuming that the applicant accepts the loan; PRi is 
the prime rate in effect at the time loan application i is approved; Amounti and Termi are 
the amount approved and the term approved, respectively; PoP (or, POPi) is the prob-
ability of payment; and, LGD (or, LGDi) is the loss given default expressed as a probabil-
ity. For a typical financial institution, Π (APR, …) is often expressed as:
 APR PoP Amount Term
APR
APR
PR
ii
Term
i
i
,K() =⋅ ⋅ ⋅
−+()
−
−
∏
−
12
11 1 2
12
11 + +()
⎛
⎝
⎜
⎜
⎞
⎠
⎟
⎟−
−() ⋅⋅
−PR
PoP LGD Amount
i
Term
i
i
12
1,
 (8.7)
where Amounti Termi (APR/12)/H20862/H208981–(1+ APR/12)–Termi/H20899 provides the borrower’s total pay-
ment over the full term Termi (expressed in months) of the loan amounting to Amounti ; 
Amounti Termi (PR/12)/H20862/H208981–(1+ PR/12)–Termi/H20899 provides the lender’s total payment over the 
full term Termi toward the financial institution (e.g., a commercial bank) that extended 
the line of credit for the amount Amounti (optional term); and, 1–PoP /H20898or, 1– POPi/H20899 s the 
probability of default. For the subprime auto-loan industry, realistic average values for 
the probability of default (1–PoP) and the loss given default LGD are 15.0% and 55.0%, 
respectively (Elghanayan, 2008).

---

## Page 208

Pricing in Business-to-Business Environments  197
For any approved loan application i characterized by PR_i, Amounti and Termi (and, 
possibly, PoPi and LGDi), the profit Π (APR, …) shown in equations (8.6) and (8.7) is a 
known function of the APR. The take up probability ρ (APR | Xi,k), however, is unknown 
at the level of the individual loan application i but could be inferred at the customer seg-
ment level that loan application i belongs to. These segment-level bid-response functions 
are estimated from historic win/loss data and typically modeled as logit bid-response 
functions. Before discussing how we compute these probability functions, we briefly 
describe the content of the CPRM auto lender data set. For more details on this topic, we 
refer the interested reader to the data dictionary that accompanies the data set and the 
work of Phillips, Simsek & van Ryzin (2013).
The CPRM data set consists of a total of 208,085 approved applications of which 
47,210 applications requested the refinancing of an existing auto loan and were thus 
excluded from the analysis. Of the remaining approved auto loan applications, 7,912 
were removed because they were still in the grace period of 45 days when the data col-
lection ended (7,910 applications) or had inconsistent or missing entries on some of the 
data set attributes (two applications). Of the resulting 152,963 valid approved auto loans, 
26,322 were funded for an overall win rate (or, equivalently, take up rate) of 17.21%. 
Each of the qualified auto loans showed valid entries along the data attributes depicted 
in Table 8.4. We randomly split the working data set into an estimation sample and a 
holdout sample consisting of 122,371 and 30,592 approved loan applications, respec-
tively. The win rates in the two samples were 17.31% (i.e., 21,179 funded applications) 
and 16.81% (i.e., 5,143 funded applications), respectively.
Table 8.4 Online Auto Lender—Data Dictionary
Variable Description
Funded Dichotomous response variable equal to 1 if the approved application was funded 
(i.e., the applicant took up the loan) and 0 otherwise.
Tier Risk based classification of applicants. Four level categorical variable: Tier 1 (most 
creditworthy applicants), Tier 2, Tier 3 and Tier 7 (least creditworthy applicants).
Partner Source of the application. Three level categorical variable: 1 (own website), 2 
(referrals from Partner A’s website) and 3 (referrals from all other websites).
Term Term of the approved loan (months). Four level categorical variable: 36, 48, 60 and 
66+ (66 and 72) months.
Vehicle Type Type of vehicle. Two level categorical variable: New and Used.
FICO Applicant’s FICO score. Numeric variable that covers the range [594, 854].
FICOH Applicant’s FICO score relative to the mean FICO score for the applicant’s tier group 
(/100). Numeric variable that covers the range [–1.72, 1.53].
Log Amount Natural logarithm of the approved loan amount. Numeric variable that covers the 
range [8.47, 11.51] (or, alternatively, [$4,770, $100,000]).
APR Online lender’s quoted APR (fractional). Numeric variable that covers the range 
[0.0245, 0.1390] (or, equivalently, [2.45%, 13.90%]).
Prime Rate 1-month LIBOR benchmark interest rate. Numeric variable that covers the range 
[0.0102, 0.0210] (or, equivalently, [1.02%, 2.10%]).
ΔRate Difference between APR and Prime Rate.
Region Region where the applicant resides. Four level categorical variable defined as per the 
US Census Bureau’s regional classification: Region 1 – Northeast (9 states), Region 2 
– Midwest (12 states), Region 3 – South (17 states) and Region 4 – West (13 states).

---

## Page 209

198  Pricing in Business-to-Business Environments
We now focus on the details of the techniques routinely used to compute the segment-
level bid-response probability functions ρ (APR | Xi,k). We examine these techniques 
in the increasing order of their complexity and provide critical yet often overlooked 
insights into what their use entails.
The simplest of the extant techniques requires one to first segment customers using a 
priori or post-hoc segmentation methods and then estimate the corresponding simple 
APR/price-only bid-response functions. While the latter of these tasks follows closely the 
procedure introduced in the section ‘Estimating the Probability Function’, the former 
is typically accomplished through the use of tree-based classification algorithms such as 
CART (Breiman, Friedman, Stone, & Olsen, 1984) and CHAID (Kass, 1980) which seg-
ment customers recursively so as to achieve the best predictive accuracy with respect to a 
categorical response variable. The use of these algorithms is appealing because—through 
perpendicular splits on the values or the levels of the available covariates  X
k—they can 
deal with complex interactions and nonlinear and nonmonotone patterns in the data 
which can be intuitively presented graphically via decision trees. For the U.S. online auto 
lender, we depict the CHAID decision tree structure in Figure 8.3; the stacked bar plots at 
its terminal nodes show the corresponding fractions of funded and nonfunded applica-
tions. The CART decision tree is not shown because it is a more parsimonious variant of 
the CHAID decision tree.
We computed the CHAID decision tree on the estimation sample using a variant of the 
CHAID algorithm (Hothorn, Hornik, & Zeileis, 2006) that is more flexible and implements 
unbiased recursive partitioning while growing the tree. We used Funded as the response 
variable and Log Amount, FICO, Term, Partner, Region and Vehicle Type as potential cov-
ariates. Of these covariates, Vehicle Type showed the highest association to the response 
1
0.8
n = 13436Funded  Non-Funded
0.6
0.4
0.2
0
1
FICO
p < 0.001
Term
p < 0.001
Log Amount
p < 0.001
Log Amount
p < 0.001
Log Amount
p < 0.001
Log Amount
p < 0.001
Vehicle Type
p < 0.001
n = 11909Funded  Non-Funded
0.6
0.4
0.2
0
1
0.80.8
n = 15823Funded  Non-Funded
0.6
0.4
0.2
0
1
0.8
n = 8912Funded  Non-Funded
0.6
0.4
0.2
0
1
0.8
n = 9976Funded  Non-Funded
0.6
0.4
0.2
0
1
0.8
n = 17941Funded  Non-Funded
0.6
0.4
0.2
0
1
0.8
n = 14318Funded  Non-Funded
0.6
0.4
0.2
0
1
0.8
n = 13713Funded  Non-Funded
0.6
0.4
0.2
0
1
0.8
n = 16343Funded  Non-Funded
0.6
0.4
0.2
0
Partner
p < 0.001
New
66+ {36, 48, 60}
> 729≤ 729
≤ 10.127 > 10.127
{2,3}1
> 10.372≤ 10.37 ≤ 10.46 > 10.461
> 9.903≤ 9.903
Used
3
2
6
9
8
12
1
15
Figure 8.3 Online Auto Lender—CHAID Decision Tree.
Note: From left to right the terminal nodes should read: Node 4, 5, 7, 10, 11, 13, 14, 16 and 17.

---

## Page 210

Pricing in Business-to-Business Environments  199
variable. Hence, Vehicle Type was chosen to split the data set first. The 92,315 approved 
applications that requested a loan for a new vehicle (shown on the branch departing the 
root node 1 on the left) were thus separated from the other 30,056 applications with an 
approved loan for a used car (shown on the branch departing the root node 1 on the 
right). In the next step of the recursive partitioning, the group of the new vehicle loans was 
further diversified based on the natural logarithm of the amount approved. According 
to the implied splitting rule, the 25,345 approved loans requesting up to $25,010 for the 
purchase of a new vehicle (or, equivalently, the approved new vehicle applications with 
a Log Amount of up to 10.127) were separated from the approved loans requesting more 
than this amount. The growing of the tree continued then recursively in a similar fashion 
until either no more association between any of the potential covariates and the response 
variable was detected or other stopping criteria were met (e.g., a minimum threshold 
size of 8,500 approved applications for the terminal nodes was reached). Upon comple-
tion, the CHAID algorithm recommended nine nonoverlapping segments (i.e., terminal 
nodes) identified by all of the potential covariates with the exception of Region. For these 
segments, we depict the corresponding APR-only logit bid-response functions in Table 
8.5 and Figure 8.4. To assess the classification accuracy of the CHAID algorithm in terms 
of whether or not an approved application is eventually funded, all approved applica-
tions in the holdout sample were mapped to the matching segments and had their take 
up probabilities computed as per the corresponding bid-response functions. With these 
probabilities as a reference, the classification error rate on the holdout sample amounted 
to 12.84%. In absolute terms, this means that 3,928 of the approved applications in the 
holdout sample were misclassified as either Funded or NonFunded when in reality they 
Table 8.5 Online Auto Lender—CHAID Logit Bid-Response Functions
Node
Variables
# 
Observations
Log 
Likelihood AIC BIC(Intercept) APR
Coef.a) S.E.b) Sig.c) Coef. S.E. Sig.
4 –0.812 0.121 *** –22.094 1.999 *** 13,436 –4,401.4 8,806.8 8,821.8
5 –1.246 0.193 *** –1.723 4.428 11,909 –6,132.7 12,269.4 12,284.1
7 –1.559 0.151 *** –13.857 2.538 *** 15,823 –4,583.2 9,170.4 9,185.7
10 –1.398 0.238 *** –28.228 5.002 *** 8,912 –2,001.3 4,006.6 4,020.7
11 –2.257 0.281 *** –21.368 5.814 *** 9,976 –1,534.8 3,073.7 3,088.1
13 –1.839 0.219 *** –30.901 4.612 *** 17,941 –2,674.1 5,352.1 5,367.7
14 –3.177 0.337 *** –18.621 6.992 *** 14,318 –1,211.1 2,426.2 2,441.4
16 3.415 0.071 *** –41.524 1.073 *** 13,713 –7,595.8 15,195.6 15,210.7
17 1.313 0.079 *** –36.993 1.321 *** 16,343 –9,291.5 18,587.1 18,602.5
# Observations 122,371
Log Likelihood –39,425.9
AIC 78,887.8
BIC 79,022.7
Error Rate
d) 12.84%
a) Coef. = Coefficient b) S.E. = Standard Error
c) Significance codes: 0 ‘***’ 0.001 ‘**’ 0.01 ‘*’ 0.05 ‘.’ 0.1
d) Classification error rates are computed on the holdout sample (30,592 approved applications of which 5,143 were 
funded).

---

## Page 211

200  Pricing in Business-to-Business Environments
were NonFunded or Funded, respectively. In practice, the value of the classification 
error rate suggests that with any new approved auto application there is a likelihood of 
12.84% to misjudge its final outcome. To put this number in perspective, the reference 
misclassification rate is 16.81% when all funded applications in the holdout sample are 
misclassified as nonfunded applications. Thus, independent of any other financial incen-
tives/considerations, the CHAID approach improves the auto lender’s ability to predict 
whether or not an application is going to be funded by about four percentage points.
As stated throughout the previous paragraphs, the procedures that require the use of 
the tree-based classification algorithms to compute the segment-level bid-response func-
tions are appealing because all complexities are shared between two disjoint tasks (i.e., 
the estimation of the bid-response functions commences only after the segmentation step 
completes). While this sharing leads to intuitive decision trees and simple APR/price-only 
bid-response functions, the approach still leaves something to be desired. First, the earlier 
variants of the CART and CHAID algorithms (many of which are coded in commercial 
customer segmentation applications) are known to suffer severe methodological short-
comings including over-fitting and variable selection bias (Chan & Loh, 2004; Hothorn et 
al., 2006; Loh, 2011). Second, these algorithms differentiate among customers in a purely 
data-driven and exploratory way (Berk, 2006); they attempt to achieve the best predictive 
accuracy with respect to a categorical response variable but do little to uncover the under-
lying patterns of the association between this response variable and the other available cov-
ariates. Hence, the simple APR/price-only bid-response functions built on the segments 
recommended by the tree-based classification algorithms are indicative of the true cus-
tomer response to various stimuli by chance only (for an illustrative example, see Hormby 
et al., 2010). This is apparent in Table 8.5 where the customers’ price sensitivity (as reflected 
by the APR coefficients) is difficult to justify across the CHAID-recommended segments. 
Finally, the fact that the segmentation and the subsequent estimation of the bid-response 
functions are asynchronous can ultimately lead to situations where the latter of these tasks 
cannot be operationalized or trusted. In particular, the conflict emerges when CART and 
1.0
0.8
0.6
Vehicle Type: New
Take Up Probability
0.4
4
5
10
713
11
14
0.2
0.0
0.00 0.05 0.10 0.20 0.15
APR
1.0
0.8
0.6
Vehicle Type: Used
Take Up Probability
0.4
16
17
0.2
0.0
0.00 0.05 0.10 0.20 0.15
APR
Node 4 Node 5
Node 7 Node 10
Node 11 Node 13
Node 14
Node 16 Node 17
Figure 8.4 Online Auto Lender—CHAID Logit Bid-Response Functions.

---

## Page 212

Pricing in Business-to-Business Environments  201
CHAID algorithms lead to either pure nodes (i.e., the segmentation is successful but the 
estimation of the bid-response functions is impossible because the segments contain all 
funded or all nonfunded applications) or nodes where the expected relation between the 
take up probabilities and the offered APR/price is insignificant or reversed (i.e., the implied 
APR/price-only bid-response functions are flat or increasing over the range of observed 
APRs/prices). Node 14, which is almost pure (see Figure 8.3), comes close to fitting well 
the first of the cases above. With its insignificant APR coefficient (see Table 8.5 and Figure 
8.4), Node 5 in turn illustrates well the problems that accompany the second of these situ-
ations. Formally, both of the difficulties above have been used to motivate the need for 
the development of alternative techniques capable of computing better logit bid-response 
functions. Chan and Loh (2004, p. 829), for example, refer to this issue to conclude that 
“a possible difficulty is the conflicting aims of classification and logistic regression—
classification trees prefer splits that cleanly separate the [categorical response variable’s] 
classes but such splits yield data sets that cannot be fitted by logistic regression.”
While the tree-based classification approach considers the segmentation and the esti-
mation of the bid-response functions as separate steps, the two can be combined into 
a single task by simply including the possible segmentation variables in a multivariate 
logistic regression model (Agrawal & Ferguson, 2007; Ferguson, 2010). This approach 
treats segmentation as a by-product and derives it directly from the functional form 
of the bid-response probability functions. Thus, the two previously asynchronous tasks 
become contemporaneous and, supposedly, they fit better the requirements of custom-
ized pricing. The logistic regression model M
1 in Table 8.6 illustrates this approach. Here, 
we modeled the win probability (i.e., the probability that the response variable Funded 
equals 1) as a nonlinear logistic function of the loan attributes Tier, Partner , Term , Vehi-
cle Type, Region (all five categorical variables), FICOH, Log Amount and APR (all three 
continuous numeric variables). As it is readily apparent from this model specification, 
the levels of the categorical variables are used to group customers into segments with 
distinct bid-response functions which can be further personalized through the use of the 
individual values for the continuous numeric variables; in this context, personalization 
leads to bid-response functions specific to groups of customers with similar attributes  
X
i,k. For example, for the most credit worthy applicants (Tier = 1) who reside in the south 
(Region = 3) and apply through the lender’s own website ( Partner = 1) to request a 60 
month loan ( Term = 60 mths) for a used car ( Vehicle Type = Used), the bid-response 
function is:
 ρ APR FICOH Log Amount|, ,   
                               
K() =
  
 
=
+
−⋅ −⋅ − ⋅
−⋅
e
e
FICOH Log Amount APR
FI
α
α
0 295 2 646 77 189
0 2951
.. .
. CCOH Log Amount APR−⋅ − ⋅2 646 77 189..  
, (8.8)
where the intercept α is adjusted to incorporate the entire information on the categorical 
loan attributes. In particular, α is expressed as
 α =+ ⋅ + ⋅ + ⋅26 774 0 1 0 1 1 130.. Tier Partner Term   60 mths
                Used   South+⋅ () +⋅ ()
=
2 313 0 665 3
26 7
..
.
Vehicle Type Region
774 1 130 1 2 313 1 0 665 1 30 882+⋅ +⋅ +⋅ =... . .
 (8.9)

---

## Page 213

202  Pricing in Business-to-Business Environments
In equation (8.9), Tier 1 and Partner 1 are zero because they both form the reference lev-
els in the corresponding dummy coded variables. If we were to continue the exercise that 
led to equation (8.8)  and discussed the particular case of applicants with a FICO score 
100 units below the mean FICO score for the Tier 1 risk group (FICOH = –100/100 = –1) 
who request an approved amount of $30,000 ( Log Amount = 10.309), we could rewrite 
the bid-response function (8.8) as:
 ρ APR e
e
APR
|
.. .. .
.K() =
+
−⋅ − () −⋅ − ⋅30 882 0 295 1 2 646 10 309 77 189
30 81 882 0 295 1 2 646 10 309 77 189
3 899 77 189
1
−⋅ − () −⋅ − ⋅
−⋅
=
+
.. . .
..
APR
APRe
e e APR3 899 77 189.. .−⋅
 (8.10)
The auto lender could then plug in the revised bid-response function (8.10) into the 
expected profit formulation (8.6) to compute the optimal APR to quote a request 
received from a loan applicant that fits the full customer profile introduced above (i.e., 
Tier 1, Region = 3, Partner 1, etc.).
While the multivariate logistic regression models avoid some of the shortcomings 
associated with the use of the tree-based classification algorithms, they too raise their 
own set of problems. In particular, when simple, no-interaction models such as model 
M
1 or the slightly altered model M2 are estimated, these imply that all applicants show 
an identical APR/price sensitivity. Given that one of the main objectives of customer 
segmentation in the first place is to identify segments with varying price sensitivities, this 
result may be unsatisfactory. For the U.S. auto lender, for example, the equal APR/price 
sensitivity requirement (for model M
1, see the constant βAPR coefficient of –77.189 in 
Table 8.6) implies that an APR increase of 1% would reduce the odds of the applicant’s 
taking up an approved loan by a factor of 2.16 (= 1/exp (βAPR . 0.01)) irrespective of who 
the applicant might be. 1 When such simple models are employed to offer customized 
APRs/prices, the customization comes solely from arbitrarily changing the APR/price 
reference points through an appropriate intercept adjustment. In practical terms, this 
means, for instance, that in bivariate plots (APR, ρ (APR |…)), the derived bid-response 
functions of the type shown in equation (8.10) are all parallel and shifted left or right 
along the APR -axis as per the values suggested by the adjusted intercepts.
The equal APR/price sensitivity problem may be addressed by fitting interaction mod-
els to the win/loss historical data in which case the model complexity increases signifi-
cantly and the implied customer behavior becomes more difficult to interpret. Model M3 
in Table 8.6 is an example of such a model. In model M3 (which builds on the specifica-
tion of the simpler model M2), the effect of the offered APR on the take up probability 
was split into two distinct components where the first is intended to capture, through the 
use of Prime Rate, the effect of the industry costs on the likelihood of an auto loan being 
funded. Since these costs are likely impacting the customers’ take up decisions undif-
ferentiated, the Prime Rate effect was estimated such that it stayed constant across all 
customer segments. The second component is intended to assess the impact of the auto 
lender’s pricing/profit decisions on the win probabilities and was estimated through the 
use of ΔRate (= APR – Prime Rate). Since it is quite likely that the margin the auto lender 
placed on top of the Prime Rate to set the offered APR correlated well with the applicants’ 
risk of default, the effect of ΔRate was estimated differentiated based on the risk tier the

---

## Page 214

Pricing in Business-to-Business Environments  203
applicants belonged to. Hence, we evaluated four Δ Rate effects, one for each of the risk 
tier segments. These effects, together with their behavioral interpretation, are provided 
in Table 8.7. The effects of all other explanatory variables were modeled as in models M1 
and M2.
Model M3 helps shed some light on the differential effect of ΔRate on the win prob-
abilities. While this effort adds to the explanatory and predictive power of our sequential 
model building (see the statistics shown at the bottom of Table 8.6), our approach is 
limiting in that it only explores some of the underlying interaction effects that govern 
borrowers’ behavior and are present in the historical data. As previously acknowledged, 
while alternative behavioral hypotheses could be tested using several other pairwise or 
higher order interactions, in practice such a task is made difficult by the correspond-
ing model complexity and the inherent difficulty of interpreting the results. In addi-
tion, while building relevant interaction terms using categorical/quantitative variables 
is straightforward (e.g., Tier, Δ Rate and Tier × Δ Rate as in Table 8.6), the same does 
Table 8.6 Online Auto Lender—Logistic Regression Results
Variable
Model M1 Model M2 Model M3
Coef.a) S.E. b) Sig. c) Coef. S.E Sig. Coef. S.E. Sig.
(Intercept) 26.774 0.286 *** 26.105 0.288 *** 27.752 0.304 ***
Tier 2 0.191 0.027 *** 0.282 0.028 *** –1.040 0.143 ***
Tier 3 0.556 0.034 *** 0.759 0.035 *** –1.586 0.147 ***
Tier 7 1.362 0.062 *** 1.795 0.064 *** –1.139 0.212 ***
Partner 2 –0.709 0.037 *** –0.657 0.038 *** –0.681 0.038 ***
Partner 3 –0.410 0.020 *** –0.423 0.020 *** –0.431 0.020 ***
Term 48 mths 0.322 0.041 *** 0.358 0.041 *** 0.547 0.042 ***
Term 60 mths 1.130 0.034 *** 1.155 0.034 *** 1.336 0.036 ***
Term 66+ mths 2.302 0.040 *** 2.430 0.041 *** 2.785 0.046 ***
Vehicle Type (Used) 2.313 0.022 *** 2.403 0.023 *** 2.514 0.024 ***
FICOH –0.295 0.045 *** –0.402 0.046 *** –0.483 0.046 ***
Log Amount –2.646 0.028 *** –2.675 0.028 *** –2.676 0.028 ***
APR –77.189 1.449 *** – – – – – –
Prime Rate- – – – 18.471 3.788 *** 13.428 3.821 ***
ΔRate – – – –89.428 1.539 *** –145.012 3.478 ***
Region 2 (Midwest) 0.019 0.034 0.035 0.035 0.044 0.035
Region 3 (South) 0.665 0.027 *** 0.674 0.027 *** 0.672 0.027 ***
Region 4 (West) 0.396 0.031 *** 0.394 0.031 *** 0.403 0.031 ***
Tier 2 
× ΔRate – – – – – – 43.005 3.904 ***
Tier 3 × ΔRate – – – – – – 65.488 3.770 ***
Tier 7 × ΔRate – – – – – – 70.331 4.103 ***
# Observations 122,371
Log Likelihood –36,211.6 –35,850.2 –35,665.8
AIC 72,455.2 71,734.3 71,371.6
BIC 72,610.6 71,899.5 71,565.9
Error Rate
d) 10.96% 10.94% 10.83%
a) Coef. = Coefficient b) S.E. = Standard Error
c) Significance codes: 0 ‘***’ 0.001 ‘**’ 0.01 ‘*’ 0.05 ‘.’ 0.1 ‘ ’ 1
d) Classification error rates are computed on the holdout sample (30,592 approved applications of which 5,143 were 
funded).

---

## Page 215

204  Pricing in Business-to-Business Environments
not apply when quantitative variables are required to be binned as a prerequisite for 
running an interaction term model (e.g., transform  FICO, a continuous quantitative 
variable, into a FICO0 ordinal variable and build the interaction terms FICO0 × ΔRate). 
In this case, determining the optimal break points for the focus variable(s) could easily 
become an intractable exercise. Finally, a reality check should be applied to any model 
results. In this application, one needs to make sure that the estimated model results in a 
constant decrease in the take-up odds when the APR/price increases. If it does not, then 
models with functional forms other than the logistic function may need to be explored 
and operationalized.
As an alternative to the individual use of the tree-based classification algorithms or the 
multivariate logistic regression models, we next describe a technique that combines the 
visually appealing structure of trees with the power of logistic regression to grow logistic 
regression trees (Chan & Loh, 2004). This technique recursively partitions a data set by 
fitting logistic regression models in each of the resulting partitions. Since they employ 
perpendicular splits, the logistic regression trees avoid some of the difficulties associated 
with the interpretability of the multivariate logistic regression models that are due to 
complex interactions and nonlinear and/or nonmonotone patterns present in the data. 
In addition, since model complexity is shared between the tree structure and the logistic 
regression models in the nodes, the resulting logistic regression models are typically less 
complex than are the multivariate regression models with interaction terms. Also, unlike 
other tree-based classification algorithms such as CART and CHAID, logistic regres-
sion trees avoid the variable selection bias by approaching the task of split selection as 
a two-stage disjoint process: the identification of the variable on which to partition the 
data is followed by the selection of the appropriate variable split points. For the U.S. auto 
lender, we depict the logistic regression tree in Figure 8.5 and the corresponding bid-
response functions in Table 8.8.
We built the logistic regression tree on the estimation sample using the LOTUS algo-
rithm (Chan & Loh, 2004) assuming the following roles for the available covariates: 
Table 8.7 Online Auto Lender—Behavioral Interpretation of the ΔRate Interaction Effects
Risk Tier /H9004RateSource from Table 8.6 Implied Customer Behavior
Tier 1 –145.012 ΔRate Most creditworthy applicants are the most APR sensitive 
of all applicants. (Irrespective of the reference level) A 1% 
increases in the APR above the prime rate in effect at the 
time of a possible approval reduces the take-up odds by a 
factor of 4.26 (=1/exp(–145.012 
× 0.01)).
Tier 2 –102.007 ΔRate + Tier 2 × ΔRate (Irrespective of the reference level) A 1% increases in the 
APR above the prime rate in effect at the time of a possible 
approval reduces the take-up odds by a factor of 2.77.
Tier 3 –79.524 ΔRate + Tier 3 
× ΔRate (Irrespective of the reference level) A 1% increases in the 
APR above the prime rate in effect at the time of a possible 
approval reduces the take-up odds by a factor of 2.21.
Tier 7 –74.681 ΔRate + Tier 7 
× ΔRate Least creditworthy applicants are the least APR sensitive 
of all applicants. (Irrespective of the reference level) A 1% 
increases in the APR above the prime rate in effect at the 
time of a possible approval reduces the take-up odds by a 
factor of 2.11 (=1/exp(–74.681 
× 0.01))

---

## Page 216

Pricing in Business-to-Business Environments  205
Funded was the dependent variable (i.e., d-variable); APR and Log Amount were treated 
as quantitative variables and used only for fitting the logistic regression models in the 
tree nodes (i.e., f-variables); FICO was treated as a quantitative variable and used both 
for fitting the logistic regression models in the tree nodes and for splitting the nodes (i.e., 
n-variable); Term was treated as an ordinal categorical variable and used exclusively for 
splitting the nodes (i.e., o-variable); and Partner, Region and Vehicle Type were treated 
as nominal categorical variables and used exclusively for splitting the nodes (i.e., c -vari-
ables). The grouping of variables in d-, f-, n-, o- or c -variables is LOTUS specific and 
provided here just to allow the interested readers to replicate our set of results. As general 
remarks, note that of the five possible segmentation variables (i.e., n-, o- and c-variables), 
only three (i.e., Vehicle Type, Partner and Region) contributed to the growing of the tree. 
Furthermore, owing to the variable stepwise selection routine implemented in LOTUS, 
FICO entered as a significant explanatory variable in only four of the six terminal node 
logistic regression models.
As apparent from Figure 8.5 and Table 8.8, the LOTUS algorithm identified six dis-
tinct customer segments in the data for which it contemporaneously estimated the cor-
responding logit bid-response functions. Unlike the multivariate logistic regression 
models shown in Table 8.6, LOTUS allowed for the constraint-free estimation of the 
parameter estimates of all explanatory variables that entered the logistic models in the 
inner or terminal nodes. Hence, no two other segments showed identical parameter esti-
mates for any of the covariates APR, Log Amount or FICO. For convenience, we provide 
the behavioral interpretation of the segment-level APR coefficients in Table 8.9.
In our introductory statements to the logistic regression trees, we highlighted some of 
the benefits of employing this technique to compute the bid-response functions 
ρ (APR 
|…) (or, some close variants ρ (ΔRate|…)) required in the expected profit formulation 
shown in equation (8.6). To avoid giving the logistic regression trees an advantage over 
the alternative approaches in terms of the model performance, we discuss next some of 
4
8
1829/35252 1554/21400 1860/21329 1754/14334
6310/15314
Partner
є {2, 3}
Vehicle
є {New}
Partner
є {2, 3}
Region
є {1, 2, 4}
Region
є {1, 2, 4}
7872/14742
5
1
91 0 11
2 3
6 7
Figure 8.5 Online Auto Lender—Logistic Regression Tree.
Note: The inner and terminal nodes are represented by circles and squares, respectively. The number inside a node is the node label and 
the splitting rule of an inner node is provided beside it. If a case satisfies the rule, it goes to the left child node; otherwise, the right child 
node. The ratio of cases with Y=1 (i.e., funded applications) to the node sample size is given beneath each terminal node. Minimum node 
size is set to 8,500 observations.

---

## Page 217

Table 8.8 Online Auto Lender—Logistic Regression Tree Bid-Response Functions
Node
Variables
# 
Observations
Log 
Likelihood AIC BIC(Intercept) APR Log Amount FICO
Coef.
a) S.E.b) Sig.c) Coef. S.E. Sig. Coef. S.E. Sig. Coef. S.E. Sig.
8 19.751 0.668 *** –27.570 2.160 *** –2.091 0.064 *** – – – 35,252 –6,617.5 13,241.0 13,266.4
9 20.466 0.764 *** –22.216 2.085 *** –2.143 0.073 *** – – – 21,400 –5,107.5 10,221.0 10,244.9
10 14.667 0.950 *** –11.614 2.949 *** –1.856 0.068 *** 0.003 0.001 *** 21,329 –5,891.0 11,790.0 11,821.9
11 16.401 1.025 *** –9.336 2.864 ** –1.891 0.074 *** 0.002 0.001 * 14,334 –4,961.6 9,931.1 9,961.4
6 33.050 0.772 *** –65.962 1.927 *** –2.289 0.047 *** –0.009 0.001 *** 15,314 –7,893.5 15,795.0 15,825.5
7 32.284 0.749 *** –55.638 1.765 *** –2.169 0.048 *** –0.010 0.001 *** 14,742 –8,147.5 16,303.0 16,333.4
# Observations 122,371
Log Likelihood –38,618.6
AIC
d) 77,291.1
BICd) 77,553.4
Error Ratee) 12.02%
a) Coef. = Coefficient
b) S.E. = Standard Error 
c) Significance codes: 0 ‘***’ 0.001 ‘**’ 0.01 ‘*’ 0.05 ‘.’ 0.1 ‘ ’ 1
d) The values of the model AIC and BIC reflect the contemporaneous estimation of all model parameter estimates including the split points
e) Classification error rates are computed on the holdout sample (30,592 approved applications of which 5,143 were funded).

---

## Page 218

Pricing in Business-to-Business Environments  207
the issues that their use commands. In terms of the split variable selection, for example, 
LOTUS tests at each node through ordinary or trend-adjusted Chi Square tests (Armit-
age, 1955; Cochran, 1954; Pearson, 1900) the independence between the dependent vari-
able and any of the possible segmentation variables and then picks for splitting the one 
covariate for which the statistical association is the most significant. As in the case of 
CART and CHAID, this approach seeks to identify and exploit the patterns in a categori-
cal response variable according to the available segmentation variables but does little to 
provide any realistic insights into the underlying patterns of the association between this 
response variable and the other available covariates. This means that although a logistic 
regression model is present in each node of a LOTUS tree, the segmentation variable 
selection is oblivious to everything that surrounds the estimation of this model, and, in 
particular, to how its parameter estimates may change as a result of splitting the node. 
In terms of the specification of the logistic regression models fitted in the nodes, LOTUS 
does not allow categorical variables such as Term, Partner or Region to be used as model 
regressors due to concerns that revolve around the following points: “The traditional 
method of dealing with nominal variables is to convert them to vectors of indicator 
variables and then use the latter as predictors in a logistic regression model. Because this 
can greatly increase the number of parameters in the node models, LOTUS only allows 
categorical variables to participate in the split selection; they are not used as regressors in 
the logistic regression models” (Chan & Loh, 2004, p. 831).
Table 8.9 Online Auto Lender—Behavioral Interpretation of the APR Effects
Node Customer Segment APR 
Coefficients 
(see Table 8.8)
Implied Customer Behavior
8 Applicants referred by the auto 
lender’s partners who live in any 
region of the US except the South 
and seek to purchase a new car.
–27.570 (Irrespective of the reference level) A 1% 
increase in the APR reduces the take-up odds 
by a factor of 1.32 (=1/exp(–27.570 
× 0.01)).
9 Applicants referred by the auto 
lender’s partners who live in 
the South of the US and seek to 
purchase a new car.
–22.216 (Irrespective of the reference level) A 1% 
increase in the APR reduces the take-up odds 
by a factor of 1.25 (=1/exp(–22.216 
× 0.01)).
10 Auto lender’s direct applicants 
who live in any region of the 
US except the South and seek to 
purchase a new car.
–11.614 (Irrespective of the reference level) A 1% 
increase in the APR reduces the take-up odds 
by a factor of 1.12 (=1/exp(–11.614 
× 0.01)).
11 Auto lender’s direct applicants 
who live in the South of the US 
and seek to purchase a new car.
–9.336 This is the least APR sensitivite customer 
segment. (Irrespective of the reference level) 
A 1% increase in the APR reduces the take-up 
odds by a factor of 1.10 (=1/exp(–9.336 
× 0.01)).
6 Applicants referred by the auto 
lender’s partners who seek to 
purchase a used car.
–65.962 This is the most APR sensitive customer 
segment. (Irrespective of the reference level) A 
1% increase in the APR reduces the take-up odds 
by a factor of 1.93 (=1/exp(–65.962 
× 0.01)).
7 Auto lender’s direct applicants 
who seek to purchase a used car.
–55.638 (Irrespective of the reference level) A 1% 
increase in the APR reduces the take-up odds 
by a factor of 1.74 (=1/exp(–55.638 
× 0.01)).

---

## Page 219

208  Pricing in Business-to-Business Environments
Up to this point, we have focused on discussing how one can compute alternative logit 
bid-response functions ρ (APR |…) for the APR optimization problem formulated in 
equation (8.6). We illustrate next the various APR/profit decisions one can make by using 
any of these ρ (APR |…) functions to the detriment of the others. Consider, for example, 
the holdout sample approved application shown in Table 8.10 where a tier 2 borrower 
applied for and subsequently took up a $24,275, 60 month loan to purchase a used car. 
If the CHAID bid-response functions are believed to be representative of customers’ 
take-up behavior, the online auto lender should quote this borrower an optimal APR of 
6.55% for an expected profit of $546.6. Alternatively, if the multivariate logistic regres-
sion or the LOTUS bid-response functions are deemed more appropriate, optimal APRs 
of 5.61% or 6.05% should be extended to this borrower, resulting in expected profits of 
$1,036.3 or $802.3, respectively. The significant differences in the expected profits are 
emphasized further by the differences in the maximum achievable profits attributable to 
borrowers who take-up the loan and stay in good standing throughout the entire agreed 
upon loan term. For the three competing 
ρ (APR |…) functions, the maximum achiev-
able profits total $3,123.9, $2,486.6, and $2,783.8, respectively. We show the optimal 
APRs and the corresponding profit figures together with the borrower’s segment-level 
bid-response functions in Table 8.11 and Figure 8.6. These somehow puzzling results 
emphasize just how critical capturing the true underlying customers’ take-up behavior 
is. In practice, competing bid-response functions are typically judged based on model 
fit statistics on the estimation sample and the model predictive accuracy on the holdout 
sample. For the online auto lender data set, the multivariate logistic regression seems to 
be superior in all regards to the other alternative modeling techniques (for relevant sta-
tistics, see the bottom of Table 8.5, Table 8.6 and Table 8.8). For other applications, we 
recommend a similar comparison to evaluate alternative estimation techniques.
SUMMARY
To summarize this chapter, the following steps are involved in building a customized 
pricing optimization model:
1. Start with a historical data set of the firm’s previous bid opportunities for the prod-
uct of interest. This data set should include both wins and losses along with the 
price submitted for each bid opportunity and any other segmentation data avail-
able on the customer or bid. The historical data set should be randomly divided 
into two distinct sets: the first for estimating the parameters of the bid-response 
models and the second for performance evaluation (the holdout data set).
Table 8.10 Online Auto Lender—Characteristics of a Holdout Sample Auto Loan Application
Application ID 142,381
Funded 1 FICOH 0.0595
Tier 2 Log Amount 10.0972
Partner 1 APR (%) 5.69%
Term (mths) 60 Prime Rate (%) 1.81%
Vehicle Type Used ΔRate (%) 3.88%
FICO 719 Region 3

---

## Page 220

Pricing in Business-to-Business Environments  209
2. A win/loss probability model, such as the logit model, should be developed that 
includes coefficients for any segmentation variables.
3. Using the estimation set from the historical data, the parameter values for the prob-
ability model should be estimated using maximum likelihood estimators. This can 
CHAID Logistic Regression
LOTUS
CHAID Logistic Regression
LOTUS
Bid-Response Functions
1.0
0.0
0.02 0.100.080.06
APR
0.04
0.2
0.4
0.6
0.8
Expected Profit Functions ($)
1000
(5.61%, $1036.3)
(6.05%, $802.2)
(6.55%, $546.6)
500
0
−500
0.02 0.100.080.06
APR
0.04
Figure 8.6 Auto Online Lender—Bid-Response Functions and Expected Profit Functions for a Holdout Sample Auto Loan 
Application.
Table 8.11 Online Auto Lender—Bid-Response Functions and Expected Proﬁ  t Functions for a Holdout Sample Auto Loan 
Application
Application ID 142,381
1. Profit Function (see Equation 8.7)
Probability of Payment PoPi = 0.90 Term Termi = 60 mths
Probability of Default 1-PoPi = 0.10 Amount Amounti = $24,275
Loss Given Default LGDi = 0.25 Prime Rate PRi = 1.81%
2. Bid-Response Functions & Optimal APRs (see Equation 8.6 and Figure 8.6)
Segmentation/Estimation Technique Bid-Response Functions Optimal 
APR (%)
Expected 
Profit ($)
Profit 
($)
a)
CHAID (see Node 17 in Figure 8.3 and 
Table 8.5) ρ APR e
e
APR
APR| ...
..
..() =
+
−⋅
−⋅
1 313 36 993
1 313 36 9931
 
 
 
 
6.55% $546.6 $3,123.9
Logistic Regression (see Model M3 
in Table 8.6and Table 8.7) ρ APR e
e
APR
APR| ...
..
..() =
+
−⋅
−⋅
6 278 102 007
6 278 102 0071
 
 
 
 
5.61% $1,036.3 $2,486.6
LOTUS Logistic Regression Trees 
(see Node 7in Figure 8.5 and 
Table 8.8)
ρ APR e
e
APR
APR| ...
..
..() =
+
−⋅
−⋅
3 054 55 638
3 054 55 6381
 
 
 
 
6.05% $802.2 $2,783.8
a) The profit values reflect the actual profit the auto lender makes if the borrower takes-up the loan and does not default 
(i.e., ρ(APR|…) = 1.0 and PoPi = 1.0).

---

## Page 221

210  Pricing in Business-to-Business Environments
be done by running a logistic regression if a logit model is used for the probability 
model. The output from the regression will help identify potential segmentation 
variables.
4. After selecting the win/loss probability model that provides the best fit for the 
holdout sample data, use this model to optimize the bid prices for all the bids in 
the holdout set from the historic data.
5. Percent improvements over expected profits and over actual profits can then be 
calculated using the holdout data to measure the model’s performance.
While customized pricing models hold great potential for substantially increasing prof-
its, any firm considering adopting them should be aware of their limitations. The mod-
els behind customized pricing assume the bid opportunities are exogenous and are not 
affected by the bid responses suggested through the optimization. In reality, a firm’s 
pricing strategy may have a significant impact on customer retention, especially if the 
optimization model recommends consistently pricing higher than the competition for 
a particular customer class. Also, the optimization models do not assume any strategic 
response from the firm’s competitors. Instead, they assume the actions of competitors 
will stay the same as it was during the time period covered by the historical data set. In 
reality, competitors may react to a firm’s new pricing strategy causing the historical bid 
opportunity data to be unrepresentative of future bid price responses. To help detect 
these possibilities, mechanisms should be put in place to monitor and evaluate the per-
formance of the models over time. If competitors change their bid-pricing behavior due 
to the implementation of a customized pricing solution, more involved models using 
concepts from game theory should be employed.
NOTE
1. If ρ (APR |…) is the take up probability, the ratio ρ (APR |…)/(1 – ρ (APR |…)) gives the odds of the appli-
cant’s taking up an approved loan. For the bid-response function shown in equation (8.10), an APR of 3% 
leads to a take up probability of 82.97% and take up odds of 4.872 (i.e., an applicant is 4.872 times more likely 
to take up the loan than to dismiss it). An APR increase of 1% changes the take up probability and take up odds 
to 69.24% and 2.251, respectively. Thus, an APR increase of 1% (all else held constant) reduces the take up 
odds by a factor of 2.16 (= 1/exp (
βAPR 0.01) = 1/exp (–77.189 0.01)). Since βAPR accompanies all bid-response 
functions derived from model M 1 depicted in Table 8.6, the odds reduction factor of 2.16 does not change 
from one applicant to another.
REFERENCES
Agrawal, V., & Ferguson, M. (2007). Bid-response models for customized pricing. Journal of Revenue & Pricing 
Management, 6(3), 212–228.
Armitage, P. (1955). Tests for linear trends in proportions and frequencies. Biometrics, 11(3), 375–386.
Berk, R. A. (2006). An introduction to ensemble methods for data analysis. Sociological Methods & Research, 34(3), 
263–295.
Boyd, D., Gordon, M., Andersson, J., Tai, C. C., Yang, F., Kolamala, A., et al. (2005). In Manugistics I. (ed.), Target 
pricing system (705/37, 705/35, 705/400, 705/1.1 ed.) G06Q30/00.
Breiman, L., Friedman, J., Stone, C. J., & Olsen, R. A. (1984). Classification and regression trees. New York, NY: 
Chapman & Hall.
Chan, K., & Loh, W. (2004). LOTUS: An algorithm for building accurate and comprehensible logistic regression 
trees. Journal of Computational and Graphical Statistics, 13(4), 826–852.
Cochran, W. G. (1954). Some methods for strengthening the common chi-squared tests.  Biometrics, 10(4), 
417–451.

---

## Page 222

Pricing in Business-to-Business Environments  211
Dudziak, B. (2006). Senior manager in the planning and analysis group at BlueLinx. Panelist in NonTraditional 
Industries Workshop. Georgia Institute of Technology and Revenue Analytics 2nd Annual Conference on 
Price Optimization and Revenue Management, Atlanta, GA, May 18, 2006.
Elghanayan, S. (2008). Does subprime deserve more than 20:20 hindsight?  Sungard Ambit Risk Management and 
Compliance, 
Ferguson, M. (2010). Customized price response to bid opportunities in competitive markets. In J. J. Cochran, L. 
A. Cox, P. Keskinocak, J. P. Kharoufeh & J. C. Smith (eds.), Wiley Encyclopedia of Operations Research and 
Management Sciences (1st ed., p. 9). New York, NY: John Wiley & Sons.
Garrow, L., Ferguson, M., Keskinocak, P., & Swann, J. (2006). Expert opinions: Current pricing and revenue man-
agement practice across U.S. industries. Journal of Revenue & Pricing Management, 5(3), 237–247.
Hormby, S., & Morrison, J. (2008). Marriott International. Instructors for workshop: Is bigger really better? Bulk 
pricing and negotiated deals. Georgia Institute of Technology and Revenue Analytics 4th Annual Conference 
on Price Optimization and Revenue Management, Atlanta, GA, November 11, 2008.
Hormby, S., Morrison, J., Dave, P., Meyers, M., & Tenca, T. (2010). Marriott International increases revenue by 
implementing a group pricing optimizer. Interfaces, 40(1), 47–57.
Hosmer, D. W., & Lemeshow, S. (2000). Applied logistic regression (2nd ed.). New York, NY: John Wiley & Sons.
Hothorn, T., Hornik, K., & Zeileis, A. (2006). Unbiased recursive partitioning: A conditional inference framework. 
Journal of Computational and Graphical Statistics, 15(3), 651–674.
Kadet, A. (2008). Price profiling. Smart Money: The Wall Street Journal Magazine, 17(5), 81–85.
Kass, G. V. (1980). An exploratory technique for investigating large quantities of categorical data. Journal of the 
Royal Statistical Society.Series C (Applied Statistics), 29(2), 119–127.
Kniple, J. (2006). Director of pricing strategy and solutions at UPS. Panelist in NonTraditional Industries Work-
shop. Georgia Institute of Technology and Revenue Analytics 2nd Annual Conference on Price Optimization 
and Revenue Management, Atlanta, GA, May 18, 2006.
Kutner, M., Nachtsheim, C., & Neter, J. (2004). Applied linear regression models (4th ed.). Boston, MA: 
McGraw-Hill/Irwin.
Loh, W. (2011). Classification and regression trees. WIREs Data Mining and Knowledge Discovery, 1(1), 14–23.
Pearson, K. (1900). On the criterion that a given system of deviations from the probable in the case of a correlated 
system of variables is such that it can be reasonably supposed to have arisen from random sampling. Philo-
sophical Magazine Series 5, 50(302), 157–175.
Phillips, R. (2005a). Pricing and revenue optimization. Stanford, CA: Stanford University Press.
Phillips, R. (2005b). Pricing Optimization in consumer credit. Presentation at the 2005 INFORMS Annual Meet-
ing, San Francisco, CA.
Phillips, R., Simsek, S., & van Ryzin, G. (2013). Does field price-discretion improve profits? Evidence from auto 
lending. Working Paper. 
Wedel, M., & Kamakura, W. A. (2000). Market segmentation: Conceptual and methodological foundations (Inter-
national Series in Quantitative Marketing) (2nd ed.). Dordrecht, The Netherlands: Kluwer Academic 
Publishers.

---

## Page 223

9
CUSTOMER BEHAVIOR ASPECTS OF PRICING
INTRODUCTION
Thus far, we have mainly focused on observing how customers respond to different 
prices and then using this data to estimate models so that price can be optimized. A 
purely analytical approach to price optimization does not guarantee success, however. 
What is also needed is to understand why customers react the way they do to promotions 
and price changes so the changes and promotions can be framed in a way that maximizes 
customer acceptance. To do so, we now venture into the psychology of pricing.
Before getting into specifics, let us first try a simple mental exercise. Imagine that you 
are trying out a new restaurant for dinner with a friend or significant other. You decide 
that a Merlot will provide a nice pairing with your meal choice so you ask for the wine 
menu. The waiter then hands you a wine menu that has the following two options for 
Merlot wines:
Dan River Vineyards Merlot $25
Dan River Vineyards Merlot Reserve $35
Which bottle do you choose? Let’s repeat the exact same exercise with the only differ-
ence being that, when you open the wine menu, you observe the following options for 
Merlot wines:
Dan River Vineyards Merlot $25
Dan River Vineyards Merlot Reserve $35
Dan River Vineyards Merlot Limited $45
Now, which bottle did you choose? It is doubtful that you recognize the brand of the 
wine (in fact, it is a made-up name), so you cannot rely on past experience of the brand’s 
quality to aid in your selection. In similar experiments of settings such as this, the major-
ity of customers faced with the $25 and $35 bottles of wine have chosen the $25 bottle. 
212

---

## Page 224

Customer Behavior Aspects of Pricing  213
The main reason provided after the choice is made is that they do not recognize the 
brand so they chose the least expensive option so as to limit their risk if the wine is not 
good. What is interesting is that the majority of customers provided with the three dif-
ferent wine choices (the $25, $35, and $45 bottles) have chosen the $35 bottle.
If the restaurant follows the common convention of increasing the markups with the 
cost of the product, then it is reasonable to assume that the $35 bottle provides around 
$15 in profit, while the $25 bottle provides around $10. If we also assume the common 
convention that the restaurant basically breaks even on sales of its meals and makes all its 
profit from the sale of beverages, then the restaurant could increase its per-seating profit 
by 33% simply by adding the third wine bottle option to its menu.
While this example is intentionally oversimplified, it demonstrates a commonly 
observed phenomenon in pricing-related experiments that cannot be explained by the 
microeconomics-based theory of pricing that was discussed in Chapter 6. If we assume 
away budget constraints, basic microeconomic theory states that each customer derives 
a distinct utility from every possible product. In this context, the customer chooses to 
purchase if the product utility (expressed as a monetary value) is greater than the selling 
price and selects the product that maximizes her remaining utility. There is nothing in 
microeconomic “utility” theory that explains why a customer would change her deci-
sion from purchasing the $25 bottle to purchasing the $35 bottle simply because a third 
option (the $45 bottle) was added to the menu. To better understand this decision mak-
ing, we have to venture into the psychological aspects of pricing and to something called 
a reference price.
REFERENCE PRICING
The wine selection experiment is an example of reference pricing, sometimes called 
anchoring. In the wine example, the consumers’ price sensitivity appears to change sim-
ply by changing the assortment of products that are available. In other experiments, 
their price sensitivity changes based on the order that an offer is presented. For example, 
an oceanfront hotel at a popular tourist destination ran an experiment in which half 
of its reservation center operators presented the most expensive room in the hotel first 
(oceanfront room), then offered the less expensive room (parking lot-view room) while 
emphasizing the discount from the more expensive option. The other half of the opera-
tors presented the room options in the opposite order. After running the experiment 
for several days, the reservation operators who presented the more expensive room first 
had a significantly higher percentage of customers who booked a room, as well as signifi-
cantly higher total revenue from the bookings they accepted.
Another aspect of reference pricing describes how a buyer’s price sensitivity increases 
with a higher price compared to perceived alternatives. The key word in this definition 
is perceived. As an example, during the recession in the travel and hospitality industry 
in the early 2000s, many hotel chains dramatically lowered their room rates in order 
to keep occupancy at a reasonable level. Thus a hotel that normally charged $300 per 
night would lower the rack rate to $150 per night. After the economy started to recover, 
the hotel chains tried to raise their rack rates back to their original amounts. Doing so, 
however, initially resulted in significant decreases in demand—much below the base-
line demand that occurred for the same room rates before the recession, even though 
the overall economy had returned to its prerecession levels. A generally accepted reason

---

## Page 225

214  Customer Behavior Aspects of Pricing
within the industry for this increase in price sensitivity was that customers had formed 
new reference prices for the value of the hotel rooms. Thus if a customer began to value 
a particular hotel room at $150, then an increase in the price to $300 is perceived to be 
unfair. The hotel chains learned from this experience, however. When the next recession 
occurred in the latter 2000s, the hotel chains were very careful about lowering the actual 
room rates to stimulate demand. Instead, they offered deals such as the fourth night free 
or free breakfasts with a room stay. These offers often accomplished the same result of 
stimulating additional demand but without the negative effect of changing the perceived 
reference prices of their customers for the value of a hotel stay.
Retailers also have to be aware of changing their customers’ reference price for an 
item during promotions or when practicing dynamic pricing. If the price for an item is 
lowered for too long of a time period, customers will change the perceived value they 
associate with the product and will be reluctant to purchase the product again at the 
former baseline price. Thus sales should be announced and the time period should be set 
for reasonably short duration.
It should also be noted in this discussion that certain items can form a reference price 
for an entire store. Consumers are more aware of the “market” price of some items more 
than others. For grocery stores, an item that consumers frequently use to determine the 
price competitiveness of a store is the price for a gallon of milk. Since most consumers 
buy milk every week, they tend to be very aware of its price. Thus if they enter a particular 
store for the first time and notice that the store prices a gallon of milk significantly higher 
than what they are used to paying (above their reference price), they will form an impres-
sion of the entire store as being a high-cost location. If, by comparison, the store prices 
an item such as nail clippers significantly higher than its competitors, consumers may 
not even notice this price difference since they tend to buy nail clippers infrequently. For 
this reason, the price range for a gallon of milk is fairly small among competing stores, 
while the price range for items bought less frequently may exhibit a wide range of prices. 
One of the hottest topics in retailing is the science of determining the items and catego-
ries for which consumers have a more knowledgeable understanding of market prices.
A final topic on reference pricing is how market prices, or some surrogate of them, 
are increasingly used in the pricing analytics models employed by some of the pricing 
software firms. As an example, a major hotel chain implemented a price optimization 
software that uses, as a reference price in the model, the average daily room rate of a 
hotel’s closest five competitors. For example, a hotel property in a downtown location 
that caters mostly to business clients uses, as a reference price, the average daily room 
rate of five competing hotel properties near the same downtown location. You may won-
der how the hotel collects the prices from the competitive hotels daily. Since most rates 
in the hospitality industry are published on the internet, there are several companies that 
specialize in designing web bots, programs that automatically capture the prices quoted 
on other firms’ web pages. These professional “screen-scraping” firms assemble a vast 
database of rates for each hotel property, by date and by room type, and send updated 
reports, listing the rates of a set number of their competitors, daily. These competitor 
prices are then fed into a firm’s pricing optimization software where they often form the 
basis for a reference price.
There is still a lot that is unknown about how consumers develop their reference 
prices. To illustrate just how arbitrary reference pricing can be, Dan Ariely (a profes-
sor at MIT and now Duke University) ran a series of behavioral experiments to see how

---

## Page 226

Customer Behavior Aspects of Pricing  215
memory of an unrelated set of numbers influenced how consumers bid for items. Ariely 
and his coauthors chose items such as an unknown brand of wine, cordless keyboards, 
and Belgian chocolates, because they represent items that most people have no strong 
priors for prices. They began the experiment by asking the participants (in this case, MIT 
students) to write the last two digits of their Social Security numbers on a sheet of paper. 
The participants were then divided into five groups based on a ranked order of these two 
digits (00–19, 20–39, etc.). Each subgroup was presented with the same items and asked 
to provide a bid for each item. While one would expect that five random groups (the last 
two numbers of each participant’s Social Security number should be random) have the 
same average bids, the average bids showed a consistent positive correlation with the last 
two Social Security numbers. That is, the bids from the group that wrote down the last 
two numbers of 00–19 bid consistently lower for all the items than did the group with 
the last two numbers 80–99.
The main implication of reference prices to pricing decisions is that when a firm 
decides to offer a temporary price promotion, care must be taken to ensure that the pro-
motional price does not change the consumers’ reference price for the product. While 
reference prices have a significant impact on how consumers respond to price changes, 
exactly how they respond depends on whether the observed price is higher or lower than 
the reference price. Their response also depends on how much higher or lower the price 
is. This leads to our next discussion on prospect theory.
PROSPECT THEORY
Prospect theory describes a behavioral approach to human decision making developed 
by Daniel Kahneman and Amos Tversky (1979) to help explain deviations from eco-
nomic models of rationality. Most of their results relate to the treatment of uncertainty 
and are not directly relevant to pricing, but one specific finding has important implica-
tions for pricing: the asymmetric, and nonlinear, treatment of how people view gains 
and losses.
To explain, let’s try another thought experiment. Imagine that you put on a coat that 
you had not worn for a while and found a $5 bill in the pocket that you did not know that 
you had. This experience will typically raise your happiness level by a certain amount. 
Now imagine that you just realized that you mistakenly left a $5 bill on a table in the 
library, and it is not there when you return. This experience will typically lower your level 
of happiness. One of the interesting findings from prospect theory is that the loss of the 
money lowers your happiness more than you gain in happiness from finding the money. 
Thus changes in utility are asymmetric between gains and losses—losses are experienced 
more intensely than gains.
Another important finding is that there is a nonlinear and decreasing return to gains. 
Think of the coat example again, but imagine that you found $10 in the pocket rather 
than $5. Finding the $5 increased your state of happiness by 20%, but finding $10 will 
not necessarily increase your state of happiness by 40%, or twice the amount that finding 
the $5 did. Thus increases in our gains result in an increase in our utility, but there are 
diminishing returns. There is a similar relationship with losses. Discovering that you left 
$10 on the table instead of $5 does not necessarily mean that you will be twice as upset.
The graph in Figure 9.1 illustrates both aspects of prospect theory. The loss in value 
from the 10% loss is greater than the gain in value from the 10% gain. The graph also

---

## Page 227

216  Customer Behavior Aspects of Pricing
illustrates the nonlinear relationship for both gains and losses. Extending prospect theory 
to pricing results in two general rules of thumb: (a) offer a discount rather than charge 
a premium whenever possible; and (b) small discounts have disproportionate effects, 
larger discounts proportionately less effect. The first rule reflects the asymmetry between 
gains and losses. Consumers view price increases or surcharges as a loss and view price 
discounts or promotions as a gain. Thus it is better to start with a higher base price and 
offer discounts than start with a lower base price and charge surcharges. The second rule 
implies that firms can delight their customers with even small discounts, but they should 
expect diminishing returns from the value their customers perceive as the discount 
increases. Note that this relationship is different from the shape of the price-response 
functions that we discussed in Chapter 6 (i.e., prospect theory does not discredit the use 
of a linear demand curve, for example). Prospect theory pertains to how an individual 
customer’s utility changes with a gain or loss, while the price-response curves reflect how 
the total market will react to price changes.
The main implications of prospect theory for pricing decisions are that discounts are 
more acceptable than surcharges, and small discounts can often capture a large percent-
age of the benefit of large discounts. Thus far, we have focused on how some behavioral 
aspects affect whether consumers decide to make a purchase or not. We have yet to say 
much about how consumers feel after making a purchase, that is, customer satisfac-
tion. In the next section, we address this important topic with a discussion on perceived 
fairness.
Value (+)
Value (−)
10% Loss
10% Gain
Reference Point
Gains ($)Losses ($)
Figure 9.1 Changes in Consumer Utility as Explained by Prospect Theory.

---

## Page 228

Customer Behavior Aspects of Pricing  217
PERCEIVED FAIRNESS OF PRICING
Have you ever purchased an item, feeling pleased with the transaction, only to discover 
a short time period later that the same item has been marked down or that someone you 
know purchased the same item for a much lower price? If so, how did you feel about 
your purchase after this new revelation? If you are like most people, your satisfaction 
from making the purchase will change from positive to negative. The first example is 
termed “buyer regret,” while the second example is termed “interpersonal comparisons,” 
because it often results when two customers of the same product discuss their purchase 
transaction and one person discovers that the other person paid a lower price.
Some industries are more susceptible to the influence of interpersonal comparisons 
than others. For example, it is common for airlines or hotels to charge very different 
prices to customers for the same flight or the same room on the same date at the same 
hotel. Consumers in these industries rarely interact with each other, so they suffer from 
a minimum amount of loss of customer satisfaction from these practices. The cruise line 
industry, by comparison, groups their customers together for social events and meals 
during a multiday cruise, where the topic of conversation frequently turns to what each 
party paid for their cruise. Thus the cruise line industry must be diligent about managing 
interpersonal comparisons, lest its customers leave the cruise with a diminished satisfac-
tion level.
Firms also have to be aware of how price changes are perceived by consumers. In gen-
eral, most consumers believe that they are entitled to a reasonable price and that firms 
are entitled to a reasonable profit. They also feel that it is unfair for a firm to make what 
are perceived to be abnormally high profits, even when customers are willing to buy the 
product at a high price. Examples of this principle abound, whenever there is a system-
atic shortage of a hot-selling product or when there is a demand/supply imbalance due 
to things such as natural disasters. This idea, called dual entitlement, was presented by 
Kahneman, Knetsch, and Thaler (1986). The implications of this principle for pricing 
decisions are as follows: (a) raising price to recoup costs is usually viewed as fair, while 
raising prices just to increase profits is often viewed as unfair; and (b) it generally helps 
to provide reasons when implementing price increases.
Finally, consumers tend to view differentiable pricing between customers more favo-
rably when they feel that the lower price is at least theoretically achievable by them. The 
early booking discount for airfares is a good example of this principle. Most consumers 
today accept the fact that different people will pay different prices for the same quality of 
coach-class seat on a particular flight. One explanation for why this is an accepted prac-
tice is that airfares tend to increase in price as the time of departure approaches. Thus 
customers who buy late and pay the higher price realize that they could have gotten a 
lower price if they had made their travel plans further in advance. Another example of an 
“achievable by me” price discount is product rebates, which are commonly used in the 
consumer electronics industry. Firms offering product rebates typically know that only a 
fraction of the buyers will follow through and take the time to send in the rebate request. 
By offering the rebate, however, the firm is able to advertise a lower price (selling price 
minus the rebate) and induce additional demand from some of the lower willingness-to-
pay consumers. In this example, customers who do not follow through by sending in the 
rebate form still feel that they had the opportunity to get the lower price, even though 
they ended up paying the full price.

---

## Page 229

218  Customer Behavior Aspects of Pricing
Compare these examples to a retailer or restaurant that offers an unannounced sale, 
that is, a sale price that is not widely advertised and requires the customer to specifically 
request it. These types of sales are common in tourist destinations, as some restaurants 
have special “local resident” menus that have much lower prices but must be specifically 
asked for. Imagine how your opinion about a restaurant would change if you were a 
frequent patron that just found out about this policy after paying the higher prices for 
years.
In summary, consumer responses to a price, or changes in the price, are based on 
more than just the utility theory discussed in Chapter 6. Indeed, there are a number of 
behavioral factors that also play a role, such as reference prices, prospect theory, and the 
perceived fairness. Thus firms considering how to set a price, or a price change, should 
also factor in how customer satisfaction will be impacted by the price change. A change 
in customer satisfaction depends on:
 how the price is presented and packaged
 perceived fairness in terms of the seller’s profit
 perceived fairness in terms of past and future prices
 perceived fairness relative to what other customers get.
SUMMARY
A purely analytical approach to price optimization is rarely successful because consum-
ers do not always react in the “rational” way that traditional microeconomics predicts. 
Thus it is just as important to understand the psychological aspects of pricing so that 
price changes and promotions can be framed in a way that maximizes the probability of 
customer acceptance. Some of the psychological aspects of pricing that have been proven 
through behavioral research include the following:
 reference pricing
 prospect theory—the asymmetric and nonlinear treatment of gains and losses
 perceptions of fairness (interpersonal comparisons, entitlement. achievability).
Reference pricing refers to how consumers form a “reference price” for a particular 
product or service. The reference price can be set based on the consumers’ experience 
with the prices set by other firms for similar products or services (market effect) or by the 
price set over a certain amount of time for your firm’s product  or service (time effect). 
One key implication of this science to pricing analytics is that firms must be careful not 
to offer promotion prices for too long a period, less the consumers will form a new refer-
ence price for the product.
Prospect theory applies to pricing analytics through the finding that consumers 
respond unfavorably to price increases in a disproportionate manner to which they 
respond favorably to price discounts. Thus it is typically better to frame price changes as 
discounts whenever possible. There is also a diminishing return to price discounts, such 
that a small discount may provide a favorable response that is more than twice the favo-
rable response that a price discount of twice the dollar amount may provide.
Finally, consumers’ happiness about a purchase may change based on their perceived 
fairness of the offer. If they feel that the company is making abnormal profits at their

---

## Page 230

Customer Behavior Aspects of Pricing  219
expense, they are less likely to be satisfied with a purchase even though their utility from 
owning the product is more than the purchase price they paid. Their perceptions may 
even change over time, especially if they find out that other consumers were able to 
purchase the product at a lower price and that they were excluded somehow from this 
offer. Thus it is generally better to design promotions such that they can be achieved by 
everyone, even if some consumer segments will self-select not to meet the requirements 
for the lower price.
REFERENCES
Kahneman, D., Knetsch, J., & Thaler, R. (1986). Fairness as a constraint on profit seeking: Entitlements in the 
market.  The American Economic Review,  76(4), 728–741. 
Kahneman, D., & Tversky, A. (1979). Prospect theory: An analysis of decision under risk.   Econometrica,  47(2), 
263–291.

---

## Page 231

Appendix A
DICHOTOMOUS LOGISTIC REGRESSION
Throughout this book we referred extensively to the logistic regression methodology 
as a means to either calibrate the logit price-response functions of Chapter 6 or esti-
mate the logit bid-response probability functions introduced in Chapter 8. While the 
two contexts exhibit many similarities in terms of their final outcome (e.g., both func-
tions are inverse S-shaped and approach zero at some high prices), from a methodo-
logical standpoint, they often require two distinct sets of statistical tools. First, the logit 
price-response functions are typically estimated using nonlinear regression models 
that attempt to minimize the sum of squared errors between the observed demand and 
the demand expected to materialize at the observed price points. This method, termed 
“nonlinear least square estimation,” requires a numeric response variable (e.g., demand) 
and at least one explanatory variable (e.g., price) which are assumed to be associated 
through a nonlinear relationship. Whenever used, this method requires the error terms 
to follow a normal distribution. The second method is usually used to estimate the logit 
bid-response probability functions using generalized linear regression models that max-
imize the likelihood of the sample data. In this case, the maximum likelihood estimation 
requires a dichotomous response variable (e.g., won/lost bids) and one or more numeric 
and/or categorical explanatory variables (e.g., price or quantity requested). We term the 
second method dichotomous logistic regression. Since the first method builds on the 
well-established class of linear regression models, we devote this appendix to exploring 
some of the intricacies associated with dichotomous logistic regression models. For a 
comprehensive discussion of nonlinear regression models, including the logistic model, 
we refer the reader to Bates and Watts (1988) and Fox (2002).
THE DICHOTOMOUS LOGISTIC REGRESSION MODEL
In the general case, the dichotomous logistic model (for details, see McCullagh and 
Nelder (1989), Nelder and Wedderburn (1972), and Neter, Kutner, Nachtsheim, and 
Wasserman (1999)) is of the form:
220

---

## Page 232

Dichotomous Logistic Regression  221
 YE Y= [] + ε , (A.1)
where
 
EY Y X
X
X
k
kk
k
K
kk
k
K[] == () =
+⋅
⎛
⎝
⎜⎜
⎞
⎠
⎟⎟
++ ⋅
⎛
⎝
⎜
=
=
∑
∑
ρ
αβ
αβ
1
1
1
1
|
exp
exp⎜ ⎜
⎞
⎠
⎟
⎟
. (A.2)
In equations (A.1) and (A.2), the variable Y, which takes on the values 0 and 1, is a Ber-
noulli random variable. E[Y] is the expected value of Y; 
ε is an error term with a distribu-
tion dependent on the Bernoulli distribution of  Y; ρ(Y = 1|Xk), or, equivalently, ρ(Xk), 
is, by construction, the probability of an event happening, that is, the probability that 
the response variable Y takes on the value 1; Xk are the explanatory variables; α and βk 
are parameters that must be estimated by fitting the model to some historical data; and 
k = 1,…,K  refers to the variables that specify the model. The response function 
ρ(Y = 1|Xk) is not linear in parameters α and βk. If we return to one of the examples of 
Chapter 8 and consider that the price quoted P is the only predictor variable that explains 
the outcome of Alpha Company’s bids, the dichotomous logistic model reduces to:
 
 
YE Y
EY Y P P
P
= [] +
[] == () = +⋅()
++ ⋅ ()
ε
ρ αβ
αβ1 1| exp
exp
,
where Y, coded as 1 for a win and 0 for a loss, refers to the outcome of the bid, 
ρ(Y = 1|P), or, equivalently, ρ(P), provides the probability of winning the bid at a current 
price P, and α and β are parameters that are to be computed using the historical win/loss 
data available.
LINEAR AND LOGISTIC REGRESSION MODELS FOR 
DICHOTOMOUS RESPONSE VARIABLES
The formulation of dichotomous logistic models in terms of probability functions ρ(Xk) 
provides support for why these models are typically preferred over the more simple 
linear regression models of the form EY Xkk
k
K
[] =+ ⋅
=
∑αβ
1
. In particular, since the 
response variable Y involves two event states that negate/exclude each other—in prac-
tice, a bid is either won or lost—it appears appropriate to predict the closeness of an 
event to these extreme 0/1 states through the means of 0/1-bounded probabilities. In this 
context, probabilities ρ(Xk) close to 1 or 0 refer to events that are likely to happen (e.g., 
a bid is won) or not happen (e.g., a bid is lost), respectively. In contrast, the use of linear 
models to compute the likely state of 0/1 events typically leads to predicted values that 
are outside of the admissible 0/1 range such as probabilities less than 0 or greater than 
1. This is particularly true when probabilities are predicted at the extreme values of the

---

## Page 233

222  Dichotomous Logistic Regression
range of Xks. Since predicted values below 0 or above 1 cannot be meaningfully justified, 
the use of linear regression models for these situations is typically deemed inappropri-
ate. We illustrate this problem in Figure A.1 where we employ some of the historical 
win/loss data from the Alpha Company and show the geometric elements recommended 
by comparable specifications of the linear and logistic regression models. Both models 
rely only on price to explain the 0/1 outcome of the bidding process. Panel A of Figure 
A.1 shows that if Alpha decided to quote a bid at the price of $7, the linear model on the 
dichotomous 0/1 bid outcome would predict a probability close to 1.2, which carries no 
palpable meaning. In contrast, panel B shows that at the same bid price of $7, the logistic 
regression model predicts a win probability close to 0.97.
Another reason logistic regression may be preferred over the simpler linear regres-
sion when the dependent variable is dichotomous relates to how the latter violates 
critical assumptions of the linear models. In particular, linear models of the form
EY X
kk
k
K
[] =+ ⋅
=
∑αβ
1
 require E[Y] to exhibit constant variance across the entire range
of the Xks. This is certainly not the case when Y is a Bernoulli random variable. We illus-
trate this point in Figure A.2, whose panel A replicates the geometric elements shown in 
panel A of Figure A.1 but limits prices to the price range $7.80 to $12.16 within which 
the corresponding predicted values are bounded by 0 and 1. Within this price interval, 
the predicted values E[Y] provide information on the likelihood of Alpha winning the 
bids. Thus E[Y] serves as the probability of winning the bid (i.e., the success probabil-
ity). A quoted price of $9.98, for example, appears to lead to a win probability of 0.50. 
At this price, the variance of a Bernoulli variable with a success probability p of 0.50 is 
p · (1 – p), or, 0.25. Using similar judgment, we compute the implied variance of all Ber-
noulli variables Y and chart it against the price in panel B of Figure A.2. This plot is not 
linear, peaks at $9.98, and decreases symmetrically toward 0 as the price slides toward 
$7.80 and $12.16, respectively.
Lastly, the linear regression model is not used with dichotomous response variables 
because the robustness of the significance testing of parameters α and βk largely depends 
(A) Linear Regression Model
1.25
1.00
0.75
0.50
0.25
0.00
6 8 10 12
Won Bids: Y = 1
Lost Bids: Y = 0p = $7.0
14
−0.25
(B) Logistic Regression Model
Price ($)
Predicted Values
Probability of Winning
Price ($)
1.25
1.00
0.75
0.50
0.25
0.00
6 8 10 12
Won Bids: Y = 1
Lost Bids: Y = 0p = $7.0
14
−0.25
Figure A.1 (A) Fitted Line for the Linear Regression Model (B) Fitted Curve for the Logistic Regression Model.

---

## Page 234

Dichotomous Logistic Regression  223
on the assumption that the residuals ( Y – E[Y]) are normally distributed. Since Y takes 
on only the values 0 and 1, this assumption is hard to justify, even approximately. Thus 
all tests of the parameter estimates α and βk computed on dichotomous responses using 
linear regression are questionable. Using the sample data from the Alpha Company, 
we show a representative residual plot in Figure A.3. In this plot, the residuals, charted 
against the fitted values E[Y], are anything but normally distributed.
(A) Linear Regression Model
(B) Variance Plot
1.00
0.50
0.75
0.25
0.00
0.00
0.05
0.10
0.15
0.20
0.25
8 9 10 11 12
Price ($)
Predicted Values
(Win Probability)Variance
8 9 10 11 12
Price ($)
Figure A.2 (A) Fitted Line for the Linear Regression Model (B) Variance Plot.
0.0 0.2
−1.0
1.0
0.5
0.0
−0.5
Fitted Values
Residuals
1.00.4 0.6 0.8
Figure A.3 Residual Plot.

---

## Page 235

224  Dichotomous Logistic Regression
 THE ESTIMATION OF DICHOTOMOUS LOGISTIC 
REGRESSION MODELS
One of the most popular techniques of estimating a logistic regression model involves 
the maximization of the likelihood of the observed data. For a data sample of size n with 
a response variable Y = {Yi = 0/1}i=1,n, the likelihood function can be expressed as
 
LP X P X ik k
Yi
ik k
Yi
i
n
= () ⋅− ()()()
−
=
∏ αβ αβ,, ,,1
1
1
, (A.3)
where Yi is the observed 0/1 outcome for the ith observation, α and βk are the parameter 
estimates that need to be computed, Xk refers to the kth explanatory variable, and Pi (α,β, 
Xk) is the probability ρi(Xk) computed for the ith observation at the current values of α 
and βk. Since the product form of the likelihood function leads to numerical instabilities 
even for small sample sizes, in practice it is generally preferred to maximize the log-
likelihood function that yields the same parameter estimates but is numerically more 
stable. Taking the natural logarithm on both sides of the likelihood function (A.3) results 
in the following expression for the log-likelihood function:
 
LL L
YP X Y P X
i i kk i i kk
= () =
=⋅ ()() +−() ⋅− ()()()
log
log , , log , ,αβ αβ11
i i
n
=
∑
1
.  (A.4)
The maximum likelihood estimators of α and βk are typically obtained by evaluating the 
gradient of the log-likelihood function (A.4) at the current values of the parameters and 
iteratively improving them using the information in the gradient.1 The iterative process 
stops when the gradient is sufficiently close to zero. Due to the complexities involved, 
the iterative procedure requires the use of a general-purpose optimizer to complete the 
task.
Other techniques used to estimate maximum likelihood estimates rely on pure itera-
tive methods to compute the parameters 
α and βk. At each iteration, the coefficients 
computed in the previous step are revised until corrections sufficiently close to zero are 
recommended. The Newton-Raphson method is a representative example of the itera-
tive techniques commonly used in practice.
For the example depicted in panel B of Figure A.1, the maximum likelihood estimates 
are given in Table A.1 . The price, with its highly statistically significant parameter  β 
(p value of 0.00), appears to indeed impact the outcome of the bid process. The negative 
sign of β suggests that increases in the price quoted are to be expected to lower Alpha’s 
probability of winning the bid. In addition, the probability plot in Figure A.1 shows that 
the middle part of the probability range ρ(P) is almost linear in the price. This indicates 
that a change in the price quoted leads to approximately the same change in the prob-
ability of winning the bid, irrespective of the reference price at which the change hap-
pens. As 
ρ(P) approaches 1 and 0, at the extreme values of the price quoted, the curve is, 
however, no longer linear.

---

## Page 236

Dichotomous Logistic Regression  225
 THE LOGIT LINK FUNCTION AND THE ODDS RATIO
Unlike linear regression, the logistic model formulated in terms of the probability ρ(Xk) 
does not provide for an intuitive interpretation of the parameter estimates α and βk. 
The logit transformation linearizes the response function ρ(Xk) and helps in getting an 
understanding of what these coefficients mean. This transformation, which calls for the 
natural logarithm of the ratio between ρ(Xk) and its complement (1 – ρ(Xk)), leads to
log ρ
ρ αβX
X Xk
k
kk
()
− ()
⎛
⎝
⎜⎜
⎞
⎠
⎟⎟=+ ⋅1 ,
where the ratio ρ(Xk)/(1 – ρ(Xk)), referred to as the odds, describes the relative likelihood 
of an event happening (e.g., the relative likelihood of winning a bid). In mathematical 
terms, the left-hand side of the equation is called the logit link function. The existence 
of such a link function places the dichotomous logistic regression models among the 
generalized linear models (Fox, 2008; Nelder & Wedderburn, 1972).
Since in many applications we are interested in quantifying the change in the odds 
associated with a unit change in an explanatory variable X
j, we can write
log odds , log odds ,,,XX X Xj k kj j k kj+()() − ()() =≠≠1
                                           =
+() ≠
log
odds ,
odds ,
,XX
XX
jk k j
j
1
kkk j
j
, ≠()
⎛
⎝
⎜
⎜
⎞
⎠
⎟
⎟=
β
or, equivalently,
OR
XX
XX
e
jk k j
jk k j
j=
+()
()
=
≠
≠
odds ,
odds ,
,
,
1 β
to compute the odds ratio OR that corresponds to a unit change in the predictor variable 
Xj (all other explanatory variables being held constant). The odds ratio OR intrinsically 
characterizes the logistic model in that it stays constant over the entire range of any vari-
able Xj. For the price-only model summarized in Table A.1, this means that a $1 increase 
in the quoted price P results in the likelihood of the firm winning the bid drop by a fac-
tor of 1/exp(–1.16), or 3.19 (irrespective of what the reference price is). In this context, 
the price coefficient β can be interpreted as specifying the customer price sensitivity. A 
Table A.1 Dichotomous Logistic Regression Model
Variable Coefficient Standard Error z value p value
Intercept α 11.58 1.98 5.86 0.00
Price β –1.16 0.20 –5.96 0.00
Null deviance: 193.05 on 139 degrees of freedom
Residual deviance: 142.46 on 138 degrees of freedom
AIC: 146.46

---

## Page 237

226  Dichotomous Logistic Regression
large negative coefficient leads to a more price sensitive customer. The interpretation 
of the price coefficient can be extrapolated to apply to all other predictor variables Xk 
(if any are present). Since the task is context specific, we restrict our discussion to pro-
viding insights only for the price quoted  P. In addition, we should warn the interested 
reader that the interpretation of parameter estimates βk changes when logistic regression 
models with interaction terms are estimated (for a relevant monograph on this topic, see 
Jaccard, 2001). 
In the logit link function, 
α, through the antilog transformation, describes the odds 
of an event happening (e.g., the odds of winning the bid) when all independent variables 
X
k are set to 0, or
odds | | |XX XX XX ekk kk kk=() == () −= ()() =00 1 0ρρ α .
Although for the price-only model the odds are irrelevant at a price P of 0, it is worth 
noting that α positions the probability function along the x -axis, that is, the price axis. 
Thus for the same value of the β coefficient, or, equivalently, the same customer price 
sensitivity, the α values shift the probability functions to the left or to the right along 
the price axis such that the resulting curves are parallel to each other in their middle 
sections. This becomes relevant when variables other than the price enter the specifi-
cation of the logistic model and are used for segmentation purposes as their presence 
typically impacts the value of 
α but not that of β. In this case, the recommended cus-
tomer segments show an identical price sensitivity that may or may not be a reasonable 
assumption.
 THE QUALITY OF THE FIT OF A DICHOTOMOUS 
LOGISTIC REGRESSION MODEL
To assess the relative performance of competing model specifications, some perform-
ance measure is needed. A standard statistical test employed in all model-fitting exercises 
asks whether a logistic regression model that includes explanatory variables (i.e., the full 
model) fits the data significantly better than a constant-only model (i.e., the null model). 
Similar judgment can be employed to compare logistic regression models that are nested. 
In this case, the null model is replaced by a reduced model that exhibits a subset of the 
explanatory variables of the full model.
The test statistic used to measure the relative model performance relies on the dif-
ference between the residual deviance for the full and null (or reduced) models. Since 
the residual deviance is a reflection of how well the log-likelihood function of a model 
approaches the maximum of the observed (zero value) log-likelihood function, the test 
statistic can be expressed as
dD e v D e v L L L L
LL L
Null Full Null Full
Null
=− = ⋅ − () −⋅ −() =
=− ⋅ + ⋅
20 20
22 L LFull
where d is the test statistic;  Dev Null, DevFull, LLNull and LLFull are the deviances and the 
log-likelihood functions for the null (or reduced) and full models, respectively; 0 is 
the observed log-likelihood function; and 2 is a convenience, scale-parameter. The test

---

## Page 238

Dichotomous Logistic Regression  227
statistic d is distributed χ2 (i.e., chi-squared) with degrees of freedom provided by the 
difference in the number of parameters between the full and null (or reduced) models.
For the logistic regression model summarized in Table A.1, the test statistic d equals 
50.59 (=193.05 – 142.46) and is chi-squared distributed with one degree of freedom. 
With an associated p value of less than 0.001, this statistic tells us that our model as a 
whole fits significantly better than a constant-only model.
NOTE 
1. In this context, the gradient refers to the vector of partial derivatives of the log-likelihood function taken with 
respect to α and βΚ. Finding the parameter estimates that make the gradient zero (and the matrix of the second 
derivatives negatively definite) is equivalent to maximizing the log-likelihood function.
REFERENCES 
Bates, D. M., & Watts, D. G. (1988). Nonlinear regression analysis and its applications. New York, NY: John Wiley 
& Sons. 
Fox, J. (2002). An R and S-PLUS companion to applied regression. Thousand Oaks, CA: Sage Publications. 
Fox, J. (2008). Applied regression analysis and generalized linear models. Thousand Oaks, CA: Sage Publications. 
Jaccard, J. (2001). Interaction effects in logistic regression. Thousand Oaks, CA: Sage Publications. 
McCullagh, P., & Nelder, J. A. (1989). Generalized linear models (2nd ed.). London: Chapman & Hall/CRC. 
Nelder, J. A., & Wedderburn, R. W. M. (1972). Generalized linear models.  Journal of the Royal Statistical Society. 
Series A (General), 135(3), 370–384. 
Neter, J., Kutner, M., Nachtsheim, C., & Wasserman, W. (1999). Applied linear statistical models (4th ed.). Chicago, 
IL: Irwin/McGraw-Hill.

---

## Page 239

Appendix B
ADVANCED ANALYTICS USING R
In this appendix, we introduce the open source statistical software environment R and 
show how it can be used for pricing analytics. In the coming sections, we cover basic infor-
mation aimed to help you get started with R. We illustrate specific topics and features 
of R in the context of real pricing problems. We combine these disparate elements into  
single, stand-alone pricing applications in the section that concludes the appendix.
THE R ENVIRONMENT
In a recent article in the New York Times, R, as a computing environment, is portrayed 
as being important “to the point that it’s hard to overvalue it” (Vance, 2009). R is cred-
ited with “becoming [the data analysts’] lingua franca partly because data mining has 
entered a golden age, whether being used to set ad prices, find new drugs more quickly, 
or fine-tune financial models” (Vance, 2009). R’s quick acceptance and increasing popu-
larity (Fox, 2009; Muenchen, 2013; Vance, 2009) have been partly attributed to its being 
an open source environment with its users being able to access, modify, and share the 
source code to better answer their specific needs. Instead of offering our own explana-
tion about what R is or is not, we encourage the reader to visit the R’s official website 
available at www.r-project.org to get a complete understanding of what R entails. As a 
summary, the following is an excerpt from the R online documentation:
R is a language and environment for statistical computing and graphics. […] One of 
R’s strengths is the ease with which well-designed publication-quality plots can be 
produced, including mathematical symbols and formulae where needed. Great care 
has been taken over the defaults for the minor design choices in graphics, but the 
user retains full control. R is available as Free Software under the terms of the Free 
Software Foundation’s GNU General Public License in source code form. It compiles 
and runs on a wide variety of UNIX platforms and similar systems (including Free-
BSD and Linux), Windows, and Mac OS. […] The term “environment” is intended 
228

---

## Page 240

Advanced Analytics Using R  229
to characterize it as a fully planned and coherent system, rather than an incremen-
tal accretion of very specific and inflexible tools, as is frequently the case with other 
data analysis software. R, like S, is designed around a true computer language, and 
it allows users to add additional functionality by defining new functions. Much of 
the system is itself written in the R dialect of S, which makes it easy for users to fol-
low the algorithmic choices made. For computationally intensive tasks, C, C++, and 
Fortran code can be linked and called at run time. Advanced users can write C code to 
manipulate R objects directly. […] R can be extended (easily) via packages. […] R has 
its own LaTeX-like documentation format, which is used to supply comprehensive 
documentation, both on-line in a number of formats and in hardcopy.
(R Core Team, 2013c) 
HOW TO INSTALL R AND ITS CONTRIBUTED PACKAGES
In this section, we describe the process of installing R and its contributed packages on 
computers running a Windows-based operating system. For installing R on Mac, Unix, 
Unix-alike and Linux platforms, we refer the reader to the R Installation and Administra-
tion manual available at http://cran.r-project.org/manuals.html (R Core Team, 2013b).
The precompiled binary distributions of the base R system and contributed packages 
can be found on the official website of the R Project at www.r-project.org. If CRAN 
(Comprehensive R Archive Network) is selected under the Download, Packages sec-
tion, and a preferred CRAN mirror is chosen, then your internet browser should take 
you to the Download and Install R web page. If a Windows installation is sought, then 
the Windows hyperlink should be selected to get to where the binary files are. Since 
the contributed packages will be installed on request, the base subdirectory should be 
selected next to get the Windows XP-style installer. At the time of writing (January 2014), 
R version 3.0.2 was available for download. Once acquired, the installer can be run in the 
normal manner, for example, by double-clicking on the R-3.0.2-win.exe file in Windows 
Explorer. Alternatively, R can be installed directly without saving the installer locally. 
During the installation, users may safely select all the defaults by simply clicking the Next 
button on each installation screen. When the installation completes, R can be launched 
by selecting it from the list of all programs available in Windows. The following is a 
detailed list with the steps required to install R and its contributed packages.
The R installation requires the following steps:
1. Open your favorite internet browser and navigate to www.r-project.org.
2. Under the Download, Packages section on the left-hand side of your computer 
screen, click on CRAN.
3. Select one of the available CRAN Mirrors (e.g., under USA, click on http://cran.cnr.
Berkeley.edu for the CRAN mirror from the University of California, Berkeley).
4. Under Download and Install R, click on Windows to get the precompiled binary 
distribution for Windows.
5. Under Subdirectories, click on base to get the binaries for the base distribution.
6. Click on Download R 3.0.2 for Windows and save the Windows installer locally in 
a directory of your choice (at the time of writing, R 3.0.2 was the last R release).
7. Open your Windows Explorer, go to the directory you chose and double-click on 
the Windows installer.

---

## Page 241

230  Advanced Analytics Using R
8. Follow the instructions to complete the R installation (for a typical user, the default 
options should work just fine).
9. Once the installation completes, R should appear in the list of Windows-available 
applications (Start/All Programs/R).
The R-contributed packages installation requires you to follow the following steps:
1. Start R (e.g., go to Start/All Programs/R and click on R x64 3.0.2 to launch R on a 
64-bit computer).
2. Select Packages from the drop-down menus at the top of the R console.
3. Select Install Package(s) …
4. Select one of the available CRAN mirrors (e.g., USA (CA1)).
5. From the available Packages, select the ones that you would like to install (e.g., car).
6. In R type 
library("Package") to load package Package in the current work-
ing environment (e.g., library("car")).
GETTING STARTED WITH R
When you launch R in Windows, the R console opens up at which time the R environ-
ment is ready to take and execute your R commands. If you use R interactively, you are 
expected to type in the R commands at the command prompt. The default R prompt 
is 
>. Alternatively, you can write your commands in script or external R files that you 
can later run or load in the current working space using appropriate R commands (e.g., 
source). We illustrate both ways of interacting with R below.
Let’s suppose that you sell a product for which you have paid a unit price of $2.70. 
Based on prior market research, you have determined that demand d(p) for this product 
varies linearly with the retail price p. The underlying product price-response function is 
d(p) = 53.70 – 4.30 . p. Your intention is to compute the revenue and profit that you will 
likely experience at a unit retail price p of $7 and $8, respectively. In R, you can calculate 
these elements easily as in the following R code chunk, where: > is the command prompt; 
# introduces a comment; <– is the assignment operator; c() is a function that combines 
its attributes into a vector; +, –, * are binary arithmetic operators; round() is a func-
tion that rounds the values of its first argument to (in this case) one decimal place; and 
print() is a function that prints its argument.
> # INPUT PARAMETERS
> D <– 53.70 # demand intercept d(p = 0)
> m <– –4.30 # demand slope
> p <– c(7.00, 8.00) # retail prices
> c <– 2.70 # product cost
> # COMPUTE REVENUE
> r <– round((D + m * p) * p, 1)
> print(r)
[1] 165.2 154.4
> # COMPUTE PROFIT
> pr <– round((D + m * p) * (p-c), 1)
> pr
[1] 101.5 102.3
>

---

## Page 242

Advanced Analytics Using R  231
In R, the commands entered interactively at the command prompt are echoed auto-
matically in the R console. One exception is the assignment operation, which is silent. 
In the previous example, we start by setting up four vectors to hold the elements of the 
price-response function (i.e., 
D and m), the anticipated retail prices (i.e., p), and the pur-
chase price (i.e., c). Using the binary arithmetic operators +, –, and *, we compute in a 
single pass the requested entities and assign them to the appropriate vectors r and pr. All 
vector operations implied by +, –, and * are performed element by element with shorter 
vectors being recycled as needed. To show the content of the revenue and profit vectors, 
we use either the 
print() function or the direct call to the corresponding R object, in 
which case the call to the print() function is implicit. The first element of a vector is 
labeled [1], even when, as with D, m, and c, for example, we deal with one-element vec-
tors. The final R command prompt indicates that R is ready to take on, interpret, and 
execute another R command.
For an exploratory working session such as the previous one, working with R inter-
actively usually suffices. However, there are many instances in practice when such an 
approach is not appropriate, let alone convenient. Often, if a task is envisioned to be 
repetitive, a series of R commands is saved in R script files that can later be loaded in an 
R working space on request. For example, let’s suppose that we have saved a cleaned ver-
sion of the previous commands in the plain-text script file 
Revenue&Profit.R. This 
file may look like the following:
# INPUT PARAMETERS
D <- 53.70; m <- –4.30; p <- c(7.00, 8.00); c <- 2.70
# COMPUTE REVENUE
r <- round((D + m * p) * p, 1)
# COMPUTE PROFIT
pr <- round((D + m * p) * (p-c), 1)
where, to conserve space, we have preferred to specify the input parameters in the same 
line and separate them by semicolons (i.e., ;). This file can be loaded in an R session 
using the source command as in the R code chunk shown later in this section. As you 
can see, the results are identical to those of the interactive exercise we have gone through 
previously. In addition, you may have noticed the presence of two other convenience 
functions not practiced before. The 
rm function, called in this way, removes all objects 
from the current R working space. The construct involving the setwd function is used 
to set the working directory to where our script file resides (please note the use of the 
Unix-like path separator 
/ even in a Windows-style working environment).
> # CLEAR THE WORKING SPACE
> rm(list=ls(all=TRUE))
> # SET WORKING DIRECTORY
> setwd("C:/Routledge/Appendix-B")
> # LOAD SCRIPT IN THE WORKING SPACE
> source("Revenue&Profit.R")
> r
[1] 165.2 154.4
> pr
[1] 101.5 102.3

---

## Page 243

232  Advanced Analytics Using R
This section has been intended to whet your appetite for experimenting with R. As we 
are aware that our brief introduction and the few examples provided may be insufficient 
for you to get a clear understanding of what R can do for you, we refer you again to the 
R manuals available online at www.cran.r-project.org/manuals.html. Among these, An 
Introduction to R is a must lecture for those interested in becoming proficient in R (Vena-
bles, Smith, & R Core Team, 2013).
GETTING HELP IN R
For most R functions, documentation is provided online. To open up the documenta-
tion pages for a topic 
topic, type at the R command prompt ?topic or help(topic) 
(e.g., ?print or help(c)). At times, to get the expected behavior, you may have to 
surround the topic by quotation marks. For example, to get help on what ? does, you 
have to type in ?"?" or else R behaves (correctly) contrary to your expectations. If you 
would like to browse the documentation by yourself or just get additional resources, 
type 
help.start() to initialize the HTML version of the help (both offline and online 
behaviors are supported). To get help on the R syntax and operators, use ?Syntax 
(operator syntax and precedence), ?Arithmetic (arithmetic operators), ?Logic (logi-
cal operators), ?Comparison (relational operators), ?Extract (object operators), and 
?Control (control-flow constructs).
At times, you may not know the name of your topic precisely. However, you could 
use ??topic or help.search("topic") to search the help system for documenta-
tion that matches topic in some elements of the documentation files (e.g., name, title, 
alias). For example, if you forgot how to fit and handle linear models in R, you could 
use 
help.search("linear models") to get a multiple-entry list with all (package, 
function) pairs that are somehow related to your topic of choice. To review any one of 
the entries in the result list you could use 
?package::function (e.g., ?stats::lm) 
to do so.
Many documentation pages end with executable examples. To run these examples, 
you have to highlight the blocks that interest you, copy them in the clipboard, and then 
paste them in a running instance of R. If you would like to run all examples associated 
with a given topic at once, you could use the 
example function to do so. For instance, 
example("smooth", package = "stats")  runs all examples provided in the 
Example section of the smooth function in the stats package. Occasionally, you may 
want to load data sets available in some R contributed packages in your R working space. 
To list a package’s available data sets or to load some or all of them in R, you could use 
the 
data function. For example, data(package = "rpart") lists the four data sets 
available in package rpart. Alternatively, data("solder", package = "rpart") 
loads the data set solder in the running instance of R.
If you are like many of us, at times, you will find that no matter how much effort you 
put into solving a problem in R, you just cannot do it. Often, R, as a computing envi-
ronment, may overwhelm you. Other times, the problem itself may not let you sleep 
at night. Whatever the reasons for your anxiety could be, do not lose faith—if you are 
facing a difficult problem, there is a high likelihood that someone else has faced it and 
solved it already. Thus we recommend that you become familiar with the features of the

---

## Page 244

Advanced Analytics Using R  233
R forum available online at http://r.789695.n4.nabble.com. If your search of the topics 
already discussed, and likely solved, by the members of the R community does not lead 
to a successful closure, you could become a registered member and post your question(s) 
online. From our experience, the likelihood of not getting a timely and relevant answer 
from the R users is quite low.
COMMON OBJECTS IN R
R operates on named objects. The most important objects in R are the vectors defined as 
collections of items of the same type. Currently, R supports six types of vectors: charac-
ter, complex, integer, logical, numeric, and raw (for details, see 
?vector). We illustrate 
how vectors are set up in the next R code chunk. Vector v1 consists of five integers 
combined with function c(). Vector v2 is a sequence of integers that starts at 1 and goes 
up to 5 in increments of 1. Through simple (element by element) arithmetic operations, 
vectors 
v1 and v2 are combined to lead to vector v3. Vector v4 is a numeric sequence 
that runs from 1 to 2 in increments of 0.25. Vector v5 is a four-element character vector. 
Vector v6 evaluates to true where vector v1 is greater or equal to 15, and to false other-
wise. Lastly, vector v7 is set up by repeating true, false, and NA (or missing value) two 
times, three times, and one time, respectively.
> v1 <- c(1, 15, 10, 40, 25) # integer vector
> v1
[1] 1 15 10 40 25
> v2 <- 1:5 # integer vector
> v2
[1] 1 2 3 4 5
> v3 <- v1^2 + 2 * v2 # integer vector
> v3
[1] 3 229 106 1608 635
> v4 <- seq(1,2,0.25) # numeric vector
> v4
[1] 1.00 1.25 1.50 1.75 2.00
> v5 <- c("This", "is", "an", "example") # character vector
> v5
[1] "This" "is" "an" "example"
> v6 <- (v1 >= 15) # logical vector
> v6
[1] FALSE TRUE FALSE TRUE TRUE
> v7 <- rep(c(TRUE, FALSE, NA), times=c(2,3,1)) # logical vector
> v7
[1] TRUE TRUE FALSE FALSE FALSE NA
Often, R users have to work with subsets of the elements of vectors. These can be 
selected by appending to the name of the vector an index vector of the form [Index 
Vector]. The following illustrates the most common subsetting operations:

---

## Page 245

234  Advanced Analytics Using R
> v1[1] # Selects 1st element of v1
[1] 1
> v1[-1] # Selects all but 1st element of v1
[1] 15 10 40 25
> v1[1:3] # Selects first three elements of v1
[1] 1 15 10
> v1[c(1,3,5)] # Selects 1st, 3rd and 5th element of v1
[1] 1 10 25
> v1[v1 >= 25] # Selects all elements of v1 ≥ 25
[1] 40 25
> v5[-c(2,3)] # Selects all but 2nd and 3rd elements of v5
[1] "This" "example"
> v7[!is.na(v7)] # Selects all non missing values of v7
[1] TRUE TRUE FALSE FALSE FALSE
In addition to vectors, R operates on other types of objects as well. Matrices and arrays, 
multidimensional representations of vectors, are typically used with constructs that con-
sist of elements of the same data type (e.g., numeric or character). Factors are used in 
connection with categorical variables that show a finite number of levels. Lists are collec-
tions of elements of different data types, including lists. Data frames are special forms of 
lists that consist of variables of the same size and unique row names. Finally, functions 
are objects, too. 
A technology and entertainment products retailer, such as Best Buy, who sells prod-
ucts in several countries across the world, could store its product prices in a matrix to 
facilitate the quick withdrawal of vital operations information. In the limited example 
provided here, subsetting the price matrix appropriately helps the retailer get the price 
at which Toshiba DVD players are sold in Mexico. To create the price matrix, we use 
the 
matrix command and force a nine-element price vector into a three-by-three data 
structure whose elements are filled by row. We change the column and row names of the 
matrix for convenience only.
> # ORIGINAL PRICE VECTOR IN THE LOCAL CURRENCY: USD, CAD, MXN
> p <– c(39.99, 38.49, 465, 34.99, 33.49, 405, 39.99, 38.49, 465)
> # CREATE PRICE MATRIX pm
> pm <- matrix(p, nrow=3, ncol=3, byrow=TRUE)
> colnames(pm) <- c("US (USD)", "Canada (CAD)", "Mexico (MXN)")
> rownames(pm) <- c("Philips DVD", "Toshiba DVD", "Sony DVD")
> pm
 US (USD) Canada (CAD) Mexico (MXN)
Philips DVD 39.99 38.49 465
Toshiba DVD 34.99 33.49 405
Sony DVD 39.99 38.49 465
> # GET THE PRICE AT WHICH TOSHIBA DVD PLAYERS ARE SOLD IN MEXICO
> pm[2,3]
[1] 405

---

## Page 246

Advanced Analytics Using R  235
In the likely event that the retailer would prefer to have the price information dis-
played by manufacturer, this can be accomplished easily by devising a three-dimension 
array. We illustrate this case in the following R code chunk where we force the original 
nine-element price vector into a one-by-three-by-three array.
> # CREATE THE PRICE ARRAY BY BRAND
> pm.b <- array(p, dim = c(1, 3, 3), dimnames=list(c("Price"), 
c("US (USD)", "Canada (CAD)", "Mexico (MXN)"), c("Philips 
DVD", "Toshiba DVD", "Sony DVD")))
> pm.b
, , Philips DVD
 US (USD) Canada (CAD) Mexico (MXN)
Price 39.99 38.49 465
, , Toshiba DVD
 US (USD) Canada (CAD) Mexico (MXN)
Price 34.99 33.49 405
, , Sony DVD
 US (USD) Canada (CAD) Mexico (MXN)
Price 39.99 38.49 465
Often, retailers place the products they sell in distinct price tiers based on the prod-
uct-perceived quality. In the previous example, the retailer groups items into two 
price tiers. The low-price tier consists of items priced below 37.50USD, or, equiva-
lently, 36.20CAD and 435.20MXN, respectively. To operationalize this price classifi-
cation, we create a character vector using the 
ifelse command that we coerce then 
into a factor. For both objects we use the str command to display the internal object 
structure.
> # CREATE A PRICE TIER CHARACTER VECTOR
> ptf <- ifelse(p <= c(37.5, 36.2, 435.2), "Low-Tier", "High-Tier")
> ptf
[1] "High-Tier" "High-Tier" "High-Tier" "Low-Tier" "Low-Tier" 
[6] "Low-Tier" "High-Tier" "High-Tier" "High-Tier"
> # SHOW INTERNAL STRUCTURE 
> str(ptf)
 chr [1:9] "High-Tier" "High-Tier" "High-Tier" ...
> # CREATE THE PRICE TIER FACTOR
> ptf <- factor(ptf)
> # SHOW INTERNAL STRUCTURE
> str(ptf)
 Factor w/ 2 levels "High-Tier","Low-Tier": 1 1 1 2 2 2 1 1 1
> ptf
[1] High-Tier High-Tier High-Tier Low-Tier Low-Tier Low-Tier 
[7] High-Tier High-Tier High-Tier
Levels: High-Tier Low-Tier

---

## Page 247

236  Advanced Analytics Using R
In certain cases incentives exist for organizations to store several data elements in the 
same data constructs. The retailer we introduced in the previous examples may find it 
beneficial to keep the list of countries it serves, the list of brands it sells, and the prices it 
charges in the same data object. As these data elements are of different types (i.e., char-
acter and numeric objects), we group them together in a list using the 
list command. 
We then illustrate how various elements of the list can be queried for easy information 
withdrawal or data reuse.
> # CREATE THE LIST
> country <- c("US", "Canada", "Mexico")
> brand <- c("Philips", "Toshiba", "Sony")
> ls <- list(Country = country, Brand = brand, Price = pm)
> ls
$Country
[1] "US" "Canada" "Mexico"
$Brand
[1] "Philips" "Toshiba" "Sony" 
$Price
US (USD) Canada (CAD) Mexico (MXN)
Philips DVD  39.99 38.49 465
Toshiba DVD 34.99 33.49 405
Sony DVD 39.99 38.49 465
> # DISPLAY BRAND LIST
> ls$Brand
[1] "Philips" "Toshiba" "Sony" 
> # SHOW THE PRICE AT WHICH TOSHIBA DVDs SELL IN MEXICO
> ls$Price[2,3]
[1] 405
We conclude this section by referring to the data object that you will experience the 
most if you intend to become proficient in R. To this end, data frames are special lists 
used for storing data tables. Unlike matrices, data frames do not have to consist of data 
elements of the same type. We illustrate this subtle point by creating a data frame that 
bundles the numeric price vector with the price tier factor and the character country 
vector and displays them together in a table-like format. We create the data frame using 
the 
data.frame command. We show the first four rows (or the header) using the 
head command. Finally, we display the internal structure of the object using the str 
command.
> # CREATE THE DATA FRAME
> df <- data.frame(Price = p, Tier = ptf, 
+ Country = rep(country, 3), stringsAsFactors=FALSE)
> # SHOW HEADER (WITH 4 ENTRIES)
> head(df, n = 4)

---

## Page 248

Advanced Analytics Using R  237
 Price Tier Country
1 39.99 High-Tier US
2 38.49 High-Tier Canada
3 465.00 High-Tier Mexico
4 34.99 Low-Tier US
> # SHOW INTERNAL OBJECT STRUCTURE
> str(df)
'data.frame': 9 obs. of 3 variables:
 $ Price : num 40 38.5 465 35 33.5 ...
 $ Tier : Factor w/ 2 levels "High-Tier","Low-Tier": 1 1 1 2 2 
2 1 1 1
 $ Country: chr "US" "Canada" "Mexico" "US" ...
WRITING FUNCTIONS IN R
Since functions are R objects, we could have discussed them in the previous section. 
However, due to their importance in executing repetitive tasks, we prefer to discuss them 
at length in the next paragraphs.
R functions are defined using the reserved word 
function, which is followed by a 
possibly empty list of formal arguments. These arguments are provided to the function 
in round brackets. The argument list is followed by the body of the function supplied in 
curly brackets. When the function is called, the formal parameters supplied by the user 
(if any are present) are used to evaluate the R expressions provided in the function’s 
body. The general syntax for defining a function is:
fun.name <- function(arg1[= def1], arg2[= def2], …) 
  {R expressions}
where def1 and def2 are optional default values for formal arguments arg1 and arg2. 
The function is called by using fun.name(arg1= val1, arg2= val2, …)  where 
val1 and val2 could take on the default values def1 and def2 or some other user-
specified values. To facilitate the (re)use of the results returned by the function, the func-
tion call is usually assigned to a data element as the following:
result <- fun.name(arg1= val1, arg2= val2, …)
The result data element consists of all elements that the function returns through an 
explicit call to the return statement. Alternatively, if return is missing, the function 
returns the value of the last evaluated expression from the body of the function.
We illustrate the practical use of writing R functions with one of the examples 
discussed in Chapter 6. The juvenile products retailer computed for one of its repre-
sentative products a linear price-response function with an intercept a of 53.70 and a 
slope b of –4.30. Given the cost of $2.50 incurred by the retailer to acquire the good, 
we intend to write a simple R function to help the product manager compute the 
optimal retail price for this product. We build the 
opt.price function such that the 
characteristics of the price-response function, the cost incurred, and an optimization 
control parameter are the function’s only formal arguments. For convenience, we 
associate these arguments with some default values, which tend to follow the figures

---

## Page 249

238  Advanced Analytics Using R
the retailer experienced with this item. The optimization control parameter refers to 
a starting value for the optimization search algorithm—we consider that a value of 
$5 is a reasonable default value for this parameter. With these arguments, we construct 
the price-dependent profit function that we intend to maximize. Keeping things at 
a generic level, we express the profit function as the product between the quantity 
expected to materialize at a price point p (i.e., a + b . p) and the unit profit associ-
ated with that price point (i.e., p–cost ). We then call the built-in R function 
optim to 
solve for the optimal price. For internal argument compliance, we supply optim with 
values for all its required and some of its optional arguments. In addition to the 
parameters that we already discussed, we make use of 
fnscale to specify that we 
intend to maximize the profit function and method to indicate our optimization 
method preference. Finally, we ask the function to return the result of the price opti-
mization step.
opt.price <- function(a=53.70, b=-4.30, cost=2.50, st.val=5.00) {
 # DEFINE THE PROFIT FUNCTION
 profit.function <- function(p, a=a, b=b, cost=cost) 
  {(a + b*p)*(p - cost)}
 # MAXIMIZE THE PROFIT FUNCTION
 res <- optim(par=st.val, fn=profit.function, a=a, b=b, 
  cost=cost, method = c("BFGS"), control=list(fnscale=-1))
 # RETURN OBJECT res
 return(res)
} # end opt.price
To compute the optimal price for the product, the product manager can call opt.
price in many equivalent ways. Since we provided argument defaults that are specific 
to this problem, the following function calls can all be used interchangeably: 
opt.price() # call 1
opt.price(53.7, -4.3, 2.5, 5.0) # call 2
opt.price(a=53.7, b=-4.3, cost=2.5, st.val=5.0) # call 3
opt.price(st.val=5.0, cost=2.5, b=-4.3, a=53.7) # call 4
opt.price(st.val=5, cost=2.5) # call 5
In the first call, since no user-defined arguments are supplied, the function uses the 
default values to pass to the R expressions present in the body of the function. In the sec-
ond call, since no names for arguments are provided, R matches these by their position. 
In the third call, arguments are fully specified by their names and values. Here, the argu-
ment matching is done by name—a named argument is matched to the formal argument 
that carries the same name. Name matching takes precedence over positional matching. 
This is illustrated in the fourth call, where even though the position of the arguments has 
changed, the R environment is capable of correctly matching all arguments provided. 
Last but not least, the fifth call shows that after the name matching takes place, R relies 
on the default values for the remaining of the arguments to complete the task. Any of 
these five equivalent function calls recommends an optimal product retail price of $7.49 
as the following depicts:

---

## Page 250

Advanced Analytics Using R  239
> opt.price(a=53.7, b=-4.3, cost=2.5, st.val=5)
$par
[1] 7.49
$value
[1] 107.25
$counts
function gradient 
 7 3 
$convergence
[1] 0
$message
NULL
As we mentioned in one of the previous paragraphs, functions are suited for repetitive 
tasks. Imagine that the product manager reviews the latest trends in the product sales 
and updates the parameters of the price-response function to 65.5 and –5.6 for a and 
b, respectively. If nothing else changes, the updated optimal price of $7.10 can be easily 
computed with a function call of the following form:
> opt.price(a=65.5, b=-5.6, cost=2.5, st.val=5)
$par
[1] 7.10
$value
[1] 118.40
$counts
function gradient 
 7 3 
$convergence
[1] 0
$message
NULL
Moreover, if the product manager were in charge of the pricing function for hundreds 
or thousands of products, a function to compute individual optimal prices based on 
minimum input arguments would come in handy. 
We conclude this section by referring readers interested in deepening their under-
standing of how to write efficient functions in R to Chapter 10 of the R manual An Intro-
duction to R available at www.cran.r-project.org/manuals.html.
HANDLING EXTERNAL FILES IN R
R as a statistical computing environment can load data from database management sys-
tems (DBMSs) such as Oracle and Teradata or external data files. Since a discussion on 
how R interacts with the growing number of DBMSs is beyond the scope of this book, we 
focus on how R handles external data files.
Often, the external data files that R needs to deal with are plain-text files. Typically, 
these files consist of data entries that are delimited either by white space or by special 
characters or at preset locations on each input line. Among the character-delimited

---

## Page 251

240  Advanced Analytics Using R
text files, tab-delimited and comma-separated values files are commonly used in many 
industry applications. The fixed width text files impose a maximum width for each of 
the fields in the file and are easier to inspect visually but require more storage space. We 
illustrate how R handles both of these types of files using the 
read.table and read.
fwf commands.
Returning to the example of the juvenile products retailer, let’s suppose that the 
characteristics of the price-response functions have been computed for all products. A 
limited subset of this information is conveniently depicted in comma-delimited and 
fixed-width formats below. Note the presence of the pipe character | in the header of 
the fixed width file—while this character is not needed in different working environ-
ments, we use such a construct here to make sure that the data-loading step completes 
successfully in R.
##### Comma Separated Values File #####
############# Product.csv #############
Product,Cost[$],Intercept,Slope
V4C3D5R2,2.5,53.7,-4.3
V4C3D5R3,3.0,47.9,-3.9
V4C3D5R4,2.3,59.8,-4.5
########### Fixed Width File ##########
############# Product.txt #############
Product |Cost[$]|Intercept|Slope
V4C3D5R2 2.5 53.7 -4.3
V4C3D5R3 3.0 47.9 -3.9
V4C3D5R4 2.3 59.8 -4.5
Assuming that the two plain-text files are saved in the working directory C:/Routledge/
Appendix-B, we can read them in R using the commands provided in the next code snip-
pet. We use read.table and read.fwf to load the comma-separated values file and the 
fixed-width file, respectively. For a successful data load, we provide relevant input values 
for some of the functions’ formal arguments. In both cases, we acknowledge the presence 
of a header at the top of the file (
header), we impose the classes to be assumed by the 
various data fields (colClasses), and we intentionally do not check the syntactic validity 
of the variable names to account for the presence of special characters such as $ (check.
names). For each of the commands, we provide appropriate entries for the file arguments 
and the header separators (sep). For read.fwf, we specify the widths in number of char-
acters of the fixed-width fields (widths). Last but not least, we check with str that the 
files loaded correctly and inspect the first entry in each file with head. 
> # SET WORKING DIRECTORY
> setwd("C:/Routledge/Appendix-B")
> # READ COMMA DELIMITED FILE
> data1 <- read.table("Product.csv", header=TRUE, sep=",",
+ colClasses=c("character", rep("numeric", 3)), check.names=FALSE)
> str(data1)

---

## Page 252

Advanced Analytics Using R  241
'data.frame': 3 obs. of 4 variables:
 $ Product : chr "V4C3D5R2" "V4C3D5R3" "V4C3D5R4"
 $ Cost[$] : num 2.5 3 2.3
 $ Intercept: num 53.7 47.9 59.8
 $ Slope : num -4.3 -3.9 -4.5
> head(data1,1)
  Product  Cost[$] Intercept Slope
1 V4C3D5R2 2.5     53.7      -4.3
>
> # READ FIXED WIDTH FILE
> data2 <- read.fwf("Product.txt", widths=c(9,8,10,5), 
+ header=TRUE, 
+ sep="|", colClasses=c("character", rep("numeric", 3)),
+ check.names=FALSE)
> str(data2)
'data.frame': 3 obs. of 4 variables:
 $ Product : chr "V4C3D5R2" "V4C3D5R3" "V4C3D5R4"
 $ Cost[$] : num 2.5 3 2.3
 $ Intercept: num 53.7 47.9 59.8
 $ Slope : num -4.3 -3.9 -4.5
> head(data2,1)
  Product  Cost[$] Intercept Slope
1 V4C3D5R2 2.5     53.7      -4.3
Up to this point, we assumed that the external files were known explicitly. In many 
cases, however, the external data files have to be selected from long lists of candidate 
files. For example, imagine that a plain-text file similar in content to Product.csv file 
is generated for all product categories that the retailer sells. Furthermore, imagine that 
these files share the same location with other thousands of files that are important yet 
irrelevant for the tasks the product manager needs to take care of. In instances like this, 
R can be of help if the category level files are named consistently based on well-defined 
naming patterns. If this is the case, R can search a specified directory for files whose 
names match a prespecified regular expression. The product manager can then work 
only with those files that satisfy the search requirements.
To provide an illustrative example, we consider that the category level files at the 
juvenile products retailer are saved following the name convention 
CT_DTS_NP.csv, 
where CT is a 12-character unique category identifier, DTS is a 14-character date and time 
stamp, and NP is an up to three-character auxiliary element that provides the number of 
items in the category CT. To identify all files that qualify from the current directory, we 
use the list.files command with the appropriate input value for its pattern argu-
ment. Specifically, we construct a regular expression that follows the built-in name con-
vention and relies on certain classes of characters to attempt the match. In this context, 
[[:alnum:]]{12}, for example, refers to a string that consists of exactly 12 alphanu-
meric characters. In contrast, [[:digit:]]{1,3} refers to a string that consists of one, 
two, or three numerical digits. Altogether, three files with their names displayed in the 
following code chunk qualify for further investigation. The savvy reader should check and 
make sure that the identified files do indeed follow the preset name convention.

---

## Page 253

242  Advanced Analytics Using R
> # SET WORKING DIRECTORY
> setwd("C:/Routledge/Appendix-B")
> # GET THE FILES THAT MATCH THE PATTERN
> files <- list.files(path=".", pattern = 
+ "^[[:alnum:]]{12}_[[:digit:]]{14}_[[:digit:]]{1,3}.csv")
> files
[1] "T12389XLT654_20110412141535_879.csv"
[2] "V12345SLT987_20110412141529_234.csv"
[3] "X14879ABC962_20110412141540_63.csv"
We conclude this section with a few thoughts on how R interacts with data files native 
to other computing environments such as SAS, Stata, and SPSS. The foreign package 
included with the R base distribution provides several functions that facilitate the import 
of such files in R. Among these, read.xport, read.dta, and read.spss allow R to 
operate on data files native to SAS, Stata, and SPSS, respectively. For more details on this 
topic, we encourage you to consult the R Data Import/Export manual available at www.
cran.r-project.org/manuals.html (R Core Team, 2013a).
RUNNING R SCRIPTS
In one of the introductory sections of this appendix, we briefly referred to R scripts and 
how they can be loaded and executed in a running instance of R with the 
source com-
mand. Since R scripts deserve a little more attention, we return to this topic to focus on 
other points of interest.
To begin with, Windows-based R has its own script editor that can be launched by 
selecting 
New Script under the File drop-down menu. While writing R scripts, com-
mands for editing and executing them are available in both File and Edit menus of 
the R GUI interface. However, since the R user interface targets primarily R power users, 
writing scripts in R may turn out to be an intimidating task for novice R users. If this 
is your case, we recommend you write your scripts in a familiar text editor (e.g., Note-
pad++, WinEdt), save them with the .R extension and either copy/paste or 
source them 
in R. We also recommend you to show patience and perseverance toward working in 
R—your effort is profitable and will pay off shortly.
Often, in a production environment you would like to run R scripts in a nonin-
teractively way—that is, without launching R explicitly and manually executing your 
scripts within the running instance of R. If you were a retailer, for example, you might 
have to post-process all your daily sales data from hundreds of stores every night at 
midnight. You would do this to get the most recent sales trends in all sales areas that 
you serve or to explore the current performance of a newly introduced product. In 
this case, instead of opening your R environment (likely remotely) and instructing R 
to run your scripts, you would rather schedule your working environment to run the 
scripts without supervision at precisely 12:00 midnight. No matter what your reason 
is to have R run noninteractively, you can do it easily under Windows or any other 
operating system that supports the installation of R. For Windows users, providing 
that the path to the R executable is part of the 
path environment variable, R can be 
called to run noninteractively from the Windows command prompt with a single-line 
construct such as the following:

---

## Page 254

Advanced Analytics Using R  243
R CMD BATCH –-no-restore –-no-save Revenue&Profit.R 
 Revenue&Profit.Rout
where R CMD BATCH instructs R to run noninteractively your R script Revenue&Profit.
R, --no-restore instructs R not to load any saved R workspace if one exists in the cur-
rent directory, --no-save instructs R that no data sets are to be saved at the end of the R 
session, and Revenue&Profit.Rout is the name of the file to which the output is writ-
ten. To improve your efficiency further, you can include this command in a batch file 
and ask the Windows scheduler to execute this file at 12:00 midnight every night. A setup 
like this helps you focus more on what your business needs are and less on technical 
details that are not always error-free. For more details on these topics, we encourage you 
to consult the An Introduction to R manual available at www.cran.r-project.org/manuals.
html (Venables al., 2013).
ADVANCED ANALYTICS USING R
In this section, we build on skills and knowledge we acquired previously and use R 
to solve complete forecasting and pricing examples. Wherever possible, we recycle 
some of the R code we already discussed. We provide details relevant to our problems 
next.
Example 1: Sales Forecasting at Company X
We show how solving a forecasting problem should be approached in practice using the 
monthly sales data from company X (Hyndman, 2013b). This data set, available on line 
at www.datamarket.com, covers the period between January 1965 and May 1971 and 
consists of a total of 77 (all valid) monthly sales figures. Building on the observed sales 
patterns, we would like to forecast the monthly sales likely to be experienced by company 
X in the coming year. Following the formal discussion from Chapter 2, this requires us to 
use a common forecast origin (i.e., May 1971) to compute forecasts for a sequence of 12 
consecutive forecast horizons (i.e., June 1971 through May 1972) based on the available 
historical data (i.e., data from January 1965 until May 1971).
As shown in the next R code snippet, we precede the actual forecasting task (lines 
24–28) with a series of R commands that eventually help us select the exponential 
smoothing technique that represents the data best. In particular, once we clear the 
working environment and set the path to the working directory (lines 01–04), we load 
the R-contributed packages 
rdatamarket  (Briem, 2012) and forecast (Hynd-
man, 2013a) (lines 05–07). We need these add-on packages because they facilitate the 
fetching of the actual data from www.datamarket.com (via the 
dminit and dmlist 
commands from the rdatamarket package) and the automatic computation of the 
forecast accuracy measures on the estimation and the holdout samples (via the accu-
racy command from the forecast package). We load the monthly sales data from 
company X into R (lines 08–10) by initializing a datamarket client with a user-spe-
cific application programming interface (API) key and performing an API request that 
retrieves and stores the fetched data into an R data frame 
a. The user-specific API keys 
are provided to all datamarket members upon the free registration on www.datamar-
ket.com.

---

## Page 255

244  Advanced Analytics Using R
01 ### CLEAR THE WORKING SPACE
02 rm(list=ls(all=TRUE))
03 ### SET THE WORKING DIRECTORY
04 setwd("C:/Routledge/Appendix-B")
05 ### LOAD THE REQUIRED R-CONTRIBUTED PACKAGES
06 library(rdatamarket)
07 library(forecast)
08 ### REQUEST THE DATA FROM DataMarket.com THROUGH AN API KEY
09 dminit("ADD YOUR OWN API KEY HERE")
10 a <- dmlist("22mp")
11 ### GET THE ESTIMATION SAMPLE DATA
12 data <- ts(data=a[1:65,2], start = 1965, frequency = 12)
13 ### RUN TRIPLE ES (MULTIPLICATIVE) ON THE ESTIMATION SAMPLE
14 tes.m <- HoltWinters(x=data, alpha = NULL, beta = NULL, gamma 
= NULL, seasonal="multiplicative")
15 ### COMPUTE FORECAST ACCURACY MEASURES ON THE ESTIMATION 
   SAMPLE
16 tes.m.acc.es <- accuracy(f=as.numeric(tes.m$fitted[,1]), 
   x=data[13:length(data)])
17 ### COMPUTE PREDICTIONS FOR THE RECORDS IN THE HOLDOUT
   SAMPLE
18 tes.m.pred <- predict(tes.m, n.ahead=12)
19 ### COMPUTE FORECAST ACCURACY MEASURES ON THE HOLDOUT
   SAMPLE
20 tes.m.acc.hs <- accuracy(f=as.numeric(tes.m.pred), 
    x=a[66:nrow(a),2])
21 
22 (The R code assessing the performance of all other exponential 
smoothing techniques not shown due to space constraints)
23 
24 ### RUN TRIPLE ES (MULTIPLICATIVE) ON THE FULL DATA SET
25 data.all <- ts(data=a[,2], start = 1965, frequency = 12)
26 tes.m <- HoltWinters(x=data.all, alpha = NULL, beta = NULL,
   gamma = NULL, seasonal = "multiplicative")
27 ### COMPUTE LONG-TERM FORECASTS
28 tes.m.pred <- predict(tes.m, n.ahead=12, 
    prediction.interval=TRUE)
To align with the objective of this exercise, we split the data set into an estimation 
sample (consisting of the first 65 monthly sales records) and a holdout sample (con-
sisting of the last 12 monthly sales records) (lines 11–12). We then fit the four expo-
nential smoothing models discussed in Chapter 2 to the estimation sample (via the 
HoltWinters command from the base R) and assess their forecast accuracy on both 
the estimation and the holdout samples. A summary of the relevant forecast accuracy 
measures together with the model parameters optimized over the estimation sample is 
provided in Table B.1. As it is readily apparent from this table, the triple exponential 
smoothing with multiplicative seasonality describes both samples best. For conven-
ience, we depict the performance of this model in terms of its data fit in panel A of 
Figure B.1. In addition, we provide in the R code chunk above (lines 13–20) the R

---

## Page 256

Advanced Analytics Using R  245
code that allows the replication of the model’s Table B.1 accuracy figures. To replicate 
all other accuracy figures from Table B.1, the HoltWinters command needs to be 
revised and called as follows:
### SIMPLE EXPONENTIAL SMOOTHING
ses <- HoltWinters(x=data, alpha=NULL, beta=FALSE, 
gamma=FALSE)
### DOUBLE EXPONENTIAL SMOOTHING
des <- HoltWinters(x=data, alpha=NULL, beta=NULL, gamma=FALSE)
### TRIPLE EXPONENTIAL SMOOTHING - ADDITIVE SEASONALITY
tes.a <- HoltWinters(x=data, alpha = NULL, beta = NULL, gamma 
= NULL, seasonal="additive").
Similarly, the x vector in the accuracy command that computes the forecast accu-
racy measures on the estimation sample (in the line-numbered R code snippet above, 
see line 16) needs to be modified to account for how R initializes the various exponen-
tial smoothing techniques (recall from Chapter 2 that some records are removed from 
the estimation procedure after the initialization). In particular, the entire R expression 
where 
x is required as an input should write as in the following:
Table B.1 Model Selection Using Forecast Accuracy Measures
1. Model Parameters (Optimized over all Entries in the Estimation Sample)
Model /H9251/H9252/H9253
Simple Exponential Smoothing 0.9999 – –
Double Exponential Smoothing 0.7700 0.9473 –
Triple Exponential Smoothing
Additive 0.7657 0.0000 1.0000
Multiplicative 0.5589 0.0000 0.62222
2. Forecast Accuracy Measures on the Estimation Sample (January 1965–May 1970)
Model ME RMSE MAE MPE MAPE
Simple Exponential Smoothing 0.547 86.812 68.736 –5.675 29.957
Double Exponential Smoothing –0.100 91.190 67.823 6.297 29.529
Triple Exponential Smoothing
Additive 0.006 59.722 43.734 –4.216 16.821
Multiplicative 5.263 53.213 38.458 –1.066 14.873
3. Forecast Accuracy Measures on the Holdout Sample (June 1970–May 1971)
Model ME RMSE MAE MPE MAPE
Simple Exponential Smoothing 299.241 377.961 299.241 52.192 52.192
Double Exponential Smoothing 687.864 743.702 687.864 155.953 155.953
Triple Exponential Smoothing
Additive 142.760 188.683 142.760 23.899 23.899
Multiplicative –56.662 87.507 71.474 –9.144 14.725

---

## Page 257

246  Advanced Analytics Using R
### SIMPLE EXPONENTIAL SMOOTHING
ses.acc.es <- accuracy(f=as.numeric(ses$fitted[,1]), x=data[2:
length(data)])
### DOUBLE EXPONENTIAL SMOOTHING
des.acc.es <- accuracy(f=as.numeric(des$fitted[,1]), x=data[3:
length(data)])
Based on the relative forecast accuracy performance depicted in Table B.1, we com-
pute the long-term forecasts using the triple exponential smoothing with multiplicative 
seasonality (in the line-numbered R code snippet above, see lines 24–28). We show these 
forecasts together with the corresponding prediction intervals in panel B of Figure B.1 
and in Table B.2. We produce these forecasts so as to minimize the mean squared (one-
step prediction) error over the full sample, that is, the sample that combines the estima-
tion and the holdout sample.
Example 2: Retail Price Setting
Often, organizations need to decide on how much they should charge their customers for 
the products or services requested. At times, they should also investigate whether or not 
the pricing strategies currently in place still align with the evolving market requirements. 
Since in many instances the two concepts overlap significantly, in what follows, we focus 
on the former task of determining the optimal product/service prices. In our example, 
(A) Estimation/Holdout Sample Analysis (for Model Selection)
Monthly Sales
Time
1500
1000
500
0
1965 1966 1967 1968 1969 1970 1971 1972
(B) Long-Term Forecasts
Time
1500Monthly Sales
1000
500
0
1965 1966 1967 1968 1969 1970 1971 1972
Actual Monthly Sales In-Sample One-Step-Ahead Forecasts (Estimation Sample)
Out-of-Sample Forecasts (Holdout Sample)
Actual Monthly Sales In-Sample One-Step-Ahead Forecasts (All Data)
Long-Term Forecasts Bounds of the Prediction Intervals for Long-Term Forecasts
Figure B.1 Sales Forecasting at Company X.

---

## Page 258

Advanced Analytics Using R  247
we assume that the organization—the juvenile products retailer of Chapter 6—did some 
market research and computed the price-response functions for all its products. We fur-
ther assume that these functions, together with the cost information, are available locally 
(vs. remotely) in comma-delimited files organized by product category (see the follow-
ing code snippet for a relevant snapshot of the file content). As it is quite likely that they 
are the outcome of an automated process, these files follow the naming convention dis-
cussed in a previous section of this appendix.
######### PRODUCT CATEGORY INPUT FILE ##########
###### X14879ABC962_20110412141540_63.csv ######
Product,Cost[$],Intercept,Slope
A4F5X9F2,4.8,89.4,-4.5
A4F5X9F3,4.6,90.3,-4.3
A4F5X9F4,4.9,85.7,-4.8
(60 more entries are not shown due to space constraints)
Our goal is to write efficient R code to help us compute the optimal product prices 
based on the available inputs. We show the final version of our R script in the code 
snippet that follows this paragraph. After we clear the working space and set the work-
ing directory (lines 01–04), we identify the files that qualify for the task based on name 
pattern matching (line 19). We keep our code generic as the product breadth and depth 
do not impact our approach. We then load the files sequentially in R and combine their 
content in a master product data frame (lines 20–23). We use 
by, an R construct that 
Table B.2 Long-Term Forecasts and Prediction Intervals
1. Model Parameters (Optimized over the Full Data Set)
Model /H9251/H9252 /H9253
Triple Exponential Smoothing
Multiplicative 0.6054 0.0000 0.4896
2. Long-Term Forecasts and Prediction Intervals
Month Forecast Upper Bound Prediction Intervals Lower Bound Prediction Intervals
Jun-71 276.9 359.4 194.4
Jul-71 389.5 509.8 269.2
Aug-71 563.8 739.2 388.3
Sep-71 894.9 1171.1 618.6
Oct-71 1164.8 1525.2 804.3
Nov-71 1216.5 1595.8 837.2
Dec-71 908.7 1199.7 617.8
Jan-72 866.5 1150.1 583.0
Feb-72 493.2 671.1 315.3
Mar-72 391.5 548.8 234.2
Apr-72 302.6 443.0 162.2
May-72 277.8 396.7 158.9

---

## Page 259

248  Advanced Analytics Using R
applies a function to a data frame split by a factor, to compute the optimal prices for all 
products and product categories (lines 24–26 and 06–16). We format the output and 
merge it to the original data (lines 27–34). We show a snapshot of the results in Table 
B.3, where the first column is shown for convenience only and is not part of the R out-
put. We supplement these business insights with intelligence on the shape of the product 
profit functions, an example of which we depict in Figure B.2. Due to space constraints, 
we do not provide the R code that creates these figures; it builds, however, on the 
plot 
command and its many fine-tuning formal arguments. Our R script being kept generic 
offers you, our savvy reader, at least one important benefit. Specifically, if you were to 
Table B.3 Product-Level Optimal Prices and Expected Proﬁ  ts
Product Category Product Cost ($) Intercept Slope Optimal Price ($) Expected Profit ($)
X14879ABC962 A4F5X9F2 4.8 89.4 –4.5 12.3 255
X14879ABC962 A4F5X9F3 4.6 90.3 –4.3 12.8 289
X14879ABC962 A4F5X9F4 4.9 85.7 –4.8 11.4 201
…
T12389XLT654 V4C3D5R2 2.5 53.7 –4.3 7.5 107
T12389XLT654 V4C3D5R3 3.0 47.9 –2.9 9.8 132
T12389XLT654 V4C3D5R4 2.3 59.8 –3.5 9.7 191
…
V12345SLT987 Z4F3D5T6 7.2 115.9 –2.3 28.8 1073
V12345SLT987 Z4F3D5T7 6.0 130.8 –2.8 26.4 1160
V12345SLT987 Z4F3D5T8 6.5 120.3 –2.5 27.3 1083
…
0
0
20
40Demand
Expected Profit ($)
Price P ($)
60
80
51 0 1 5 2 0
0
50
100
150
200
250
Price Response Function
Profit Function Optimal Price
Figure B.2 Price-Response Function, Profit Function and the Optimal Price (Product: A4F5X9F2).

---

## Page 260

Advanced Analytics Using R  249
replicate our results, all you have to change in our code would be the path to the working 
directory where the input files reside. This is an add-on benefit that comes with good (R) 
programming habits.
01 ### CLEAR THE WORKING SPACE
02 rm(list=ls(all=TRUE))
03 ### SET WORKING DIRECTORY
04 setwd("C:/Routledge/Appendix-B")
05 
06 ### FUNCTION TO COMPUTE THE OPTIMAL PRICE
07 opt.price <- function(x) {
08   # INITIALIZE INPUT PARAMETERS
09  a<- x[1,3]; b<-x[1,4]; cost<-x[1,2]; st.val=5
10  # DEFINE THE FUNCTION TO BE MAXIMIZED
11  obj.fun.linear <- function(p, a=a, b=b, cost=cost) 
   {(a+b*p)*(p - cost)}
12   # MAXIMIZE THE FUNCTION
13  res <- optim(par=st.val, fn=obj.fun.linear, a=a, b=b,
  cost=cost, method=c("BFGS"), control=list(fnscale=-1))
14   # RETURN OBJECT res
15   return(res)
16 } # end opt.price
17 
18 ### READ AND COMBINE THE CATEGORY DATA FILES
19 files <- list.files(path=".", 
 pattern="^[[:alnum:]]{12}_[[:digit:]]{14}_[[:digit:]]{1,3}.csv")
20 for (findex in 1:length(files)) {
21  data.tmp <- read.table(file=files[findex], header=TRUE,
sep=",", colClasses=c("character", rep("numeric",3)), 
check.names=FALSE)
22  if (findex == 1) {data <- data.tmp} else {data <- 
  rbind(data, data.tmp)}
23 } # end for findex
24 ### COMPUTE THE OPTIMAL PRICES FOR ALL PRODUCTS
25 res <- by(data, factor(data[,1]), FUN=opt.price,
 simplify=TRUE)
26 res <- do.call("rbind", res)
27 # FORMAT OUTPUT
28 res <- data.frame(res[,1:2], Product=row.names(res))
29 res <- res[,c(3,1:2)]
30 names(res) <- c("Product", "Optimal Price", "Expected 
Profit")
31 res[,2] <- unlist(res[,2])
32 res[,3] <- unlist(res[,3])
33 ### MERGE RESULTS
34 data <- merge(data, res)

---

## Page 261

250  Advanced Analytics Using R
REFERENCES 
Briem, G. T. (2012). rdatamarket: Data access API for DataMarket.com R package version 0.6.4. Retrieved from 
http://cran.r-project.org/package=rdatamarket. 
Fox, J. (2009). Aspects of the social organization and trajectory of the R project. The R Journal, 1(2), 5–13. 
Hyndman, R. J. (2013a). forecast: Forecasting functions for time series and linear models (with contributions 
from Slava Razbash and Drew Schmidt). R package version 4.05. Retrieved from http://cran.r-project.
org/package=forecast. 
Hyndman, R. J. (2013b). Time Series Data Library. Retrieved June 24, 2013, from http://data.is/VVOndh. 
Muenchen, R. A. (2013, February 12). What analytic software are people discussing? Message posted to 
www.r-bloggers.com/what-analytic-software-are-people-discussing. 
R Core Team. (2013a). R data import/export. Vienna, Austria: R Foundation for Statistical Computing. Retrieved 
from http://cran.r-project.org/doc/manuals/r-release/R-data.pdf. 
R Core Team. (2013b). R installation and administration. Vienna, Austria: R Foundation for Statistical Computing. 
Retrieved from http://cran.r-project.org/doc/manuals/r-release/R-admin.pdf. 
R Core Team. (2013c). R: A language and environment for statistical computing. Vienna, Austria: R Foundation for 
Statistical Computing. Retrieved from www.r-project.org/. 
Vance, A. (2009, January 6). Data analysts captivated by R’s power. New York Times. Retrieved April 1, 2011 from 
www.nytimes.com. 
Venables, W. N., Smith, D. M., & R Core Team. (2013). An introduction to R. Vienna, Austria: R Foundation for 
Statistical Computing. Retrieved from http://cran.r-project.org/doc/manuals/r-release/R-intro.pdf.

---

## Page 262

INDEX
Note: The following abbreviations have been used – f = figure; n = note; t= table
251
accuracy measures: forecasting 12–16, 17 f&t, 18
‘achievable by me’ price discount 217
additive models 65, 66–7 t, 68, 72
additive seasonality 33, 34 f, 35, 41
adjusted R-square value 60
age-based segmentation 2, 3, 6
airline industry 1, 3–4, 8, 43, 62; bid prices 93, 94, 95; 
booking limits 84–5; dynamic pricing 168–9, 
171, 184; Expected Marginal Seat Revenue Model 
(EMSR) 89, 90t, 91–2; multiple time series 116; 
nested booking limits 87, 88 f&t; out-of-stock 
events 98; perceived fairness of pricing 217; 
projection-detruncation (PD) method 132; 
seasonality 35, 36f
Akaike’s Information Criterion (AIC) 16, 17, 158
analytical modeling step 63, 65
anchoring see reference pricing
annual percent rate (APR) 201, 202, 204, 207 t, 208, 
210n; expected profit 196–7
arc elasticity 147
ARIMA see autoregressive integrated moving average 
models
auto lenders 195–6, 208; data dictionary 197t; 
logistic regression 203 t, 206t; rate interaction 
effects 204t; tree-based classification 
algorithm 198f, 199t, 200f, 201–2, 205f, 207t
autoregressive integrated moving average models 
(ARIMA) 11, 12, 28, 31
averaging method (AM) 115 t, 116–17, 118t, 119t, 134
bargaining 167–8
Bayesian Information Criterion (BIC) 16, 17
bell-curve distribution 142 f, 143, 144
benchmark forecasting methods 13, 15
Bernoulli distribution 221, 222
bias 15–16
BIC see Bayesian Information Criterion
bid price controls 92 t, 93f, 94f, 95t, 96t
bid-response functions 186–7, 188, 194t; holdout 
sample 209f&t; interest rate optimisation 197, 
199t, 200f, 201, 202, 208
Big Data 6–7
Bonus Buys 72, 73, 75
booking: curves 99, 100 f, 116, 117, 120; horizons 116, 
117, 120, 126; limits 84–5, 86f, 87, 88f&t, 89–92; 
perceived fairness of pricing 217
brick-and-mortar retailers 157, 179
brute force method 79, 80
bucket prices 87, 88 f
business analytics 
6–7
business-to-business (B2B) environments 136, 
153t; traditional price optimisation and 188, 
189f; 186–8, 208t, 209f&t, 210; customer 
segmentation 187, 190, 191, 192, 193t; 
customised pricing probability models for 
price optimisation 186–8, 189f, 190, 191, 
192, 195; data dictionary 197 t; estimating 
probability function 189–90; implementing 
customised pricing optimisation 195–6; 
logistic regression 203t, 206t; measuring 
performance 193t, 194t; rate interaction 
effects 204t; tree-based classification 
algorithm 198f, 199t, 200f, 201–2, 205f, 207t
business-to-consumer pricing (B2C) 153 t, 168; 
customised pricing 196–7, 208t, 209f&t, 210; 
data dictionary 197t; logistic regression 203 t,

---

## Page 263

252  Index
business-to-consumer pricing (cont.):
 206t; rate interaction effect 204t; tree-based 
classification algorithm 198 f, 199t, 200f, 201–2, 
205f, 207t
business/leisure-based segmentation 2, 3–4, 84, 85, 
86, 87
‘buyer regret’ 217
buying behaviours 1–2
capacity allocation 169
capacity-based revenue management 7, 96–7; 
determining booking limits 84–5, 86 f, 87, 88f&t, 
89–92; network revenue management 92t, 93f, 
94f, 95t, 96t; news vendor model 81 f, 82t, 83; 
single order opportunity inventory problem 77, 
78t, 79t, 80t, 81; see also news vendor model
capacity-constrained industries 1
CART (decision tree) 198, 200, 204, 207
category hierarchy-grouping pricing 169
censored single-period items 106, 107 t, 108t, 110, 
114t, 115
centered weighted moving averages 35
CHAID (decision tree) 198f, 199t, 200f, 201, 204, 207–8
channel-based pricing 5
Chi Square tests 207
complete-data log likelihood function 123
constant-elasticity price-response function 143, 144f, 
146t, 149; price elasticity 158 t, 161t, 162
consumer search cost 137
‘consumer utility’ 137
convergence test 125–6, 131
coupons 6
‘critical ratio’ 83, 86, 89, 90, 178 t
cumulative demand distribution function 110, 113 t
customer behaviour 212–13, 218–19; perceived 
fairness of pricing 217–18; prospect theory 215, 
216f; reference pricing 213–15, 218
customer satisfaction 218
customer segmentation 1–2, 86–7, 146; business-
to-business (B2B) environments 187, 192; 
markdowns 172, 184; price elasticity 152, 165; 
price optimisation 162, 190; product-based 
segmentation and 2–6
customer surveys 157, 162 t
customer web search history 6
customised pricing 170, 182; business-to-business 
(B2B) environments 186–8, 189 f, 190, 
191, 192, 195; business-to-consumer (B2C) 
environments 196–7, 208 t, 209t&f, 210
data frames 236–7
database management systems (DBMSs) 240
demand distribution 
47, 78t, 80, 82, 96, 106; booking 
limits 87, 88, 89; censored single-period 
items 106, 107 t, 108t, 110, 114t, 115; price-
dependency 183f; private brands/labels 180, 
181t; unconstraining 99
demand points (P-methods) 108
DES see double exponential smoothing
descriptive analytics 7
dichotomous logistic regression model 220–1; 
linear/logistic regression models for 221, 222 f, 
223f, 224, 225t; logit link function and odds 
ratio 225–6; quality of fit 226, 227n
discounting 2, 3, 6, 62, 85; customer behaviour 216, 
217
double exponential smoothing (DES) 29–30, 31 f, 32t; 
unconstraining 119, 120 t, 121t, 122f, 126, 134; 
see also simple exponential smoothing; triple 
exponential smoothing
dual entitlement 217
dynamic pricing 167–71, 184, 214; see also markdown 
pricing
dynamic regression models 10–12
e-business see online retailing
E-like Step 130, 131, 132
e-mail campaigns 170, 179, 180, 182, 184
effort-based discounts 6
elasticity (pricing) 143, 144 f, 147, 148t, 149f, 
151–2; estimating 156–7; price-response 
functions 158t, 159f, 160t, 161t, 162t, 163t; main 
steps of pricing initiative 164–5; see also pricing 
analytics
EMSR see expected marginal seat revenue model
end-of-season clearance periods 173–4, 175–6, 182, 
184
estimation samples 41
Excel (Microsoft) 29, 48, 83, 86, 162; linear 
programming formulation 94 f, 95t; linear 
regression analysis 51, 52f, 53f, 54f, 55f, 156; 
price optimisation 190
expectation step (E-step) 
123, 124, 125, 126
expectation-maximisation (EM) algorithm 122–6, 
127t, 128t, 134
expected marginal seat revenue model (EMSR) 88 t, 
89, 90t, 91–2
expected profit calculation 78, 79 t, 80t, 83, 191f, 
209f&t; product-level optimal prices 248 t
expert opinion 157
‘expiring capacity’ 84–5
explanatory forecasting models 10, 11
exponential moving average 182
exponential smoothing 12, 18, 41, 44; double 
exponential smoothing 29–30, 31f, 32t; simple 
exponential smoothing 25–7, 28f, 29t; triple 
exponential smoothing 33, 34f, 35, 36f, 37t, 38t, 
39t
extrapolative forecasting models 7, 10, 11–12, 44
fashion industry 20, 100–1, 103, 160t, 161t, 162; 
forecasting 30, 31f; linear programming 178–80, 
181t, 182, 183f, 184t; markdowns 172, 173; slow-
moving items 174, 175, 176–7, 178t, 184
financial services industry 186, 191, 192
fixed time period inventory models 116
food retailing 77, 78 t, 79t, 80t, 218; common mistakes 
when using regression models to forecast 53,

---

## Page 264

Index  253
54; estimating linear regression model in Excel 
(Microsoft) 51, 52 f, 53; maximum likelihood 
estimation technique 56 f, 57f, 58t, 59f; normal 
distribution 81f, 82f, 83; promotional flyer 
variable 61f
forecasting 8; accuracy measures 12–16, 17f&t, 18; 
objectives of 9–10; sales 243–4, 245t, 246f, 247t; 
theory of 10–12
gains/losses 215, 216 f
gender-based segmentation 2
generic forecast error 12
global price-response models 144
grocery stores 47, 70, 71 f, 72–3, 74t, 75; censored 
single-period items 106, 107 t, 108t, 109t, 110; 
cumulative demand distribution function 110, 
113t; double exponential smoothing (DES) 121 t, 
122; expectation-maximisation (EM) 
algorithm 126; hourly sales rates 111–12, 117; 
price segmentation 152; projection-detruncation 
(PD) method 132, 133 t; reference pricing 214; 
Tocher’s inverse cumulative demand distribution 
function 110, 114 t, 115
Gumbel cumulative distribution function 110, 114t, 115
‘heterogeneous customers’ 137
high-traffic generating events 62, 63, 68, 69
historical price/demand data 137, 138, 139, 180
holdout sample 16, 17–18, 19 f, 44, 75, 76; 
bid-response functions 209 f&; logistic 
regression 195, 208
hospitality industry 1, 8, 60, 61, 62; bid prices 93t, 
94f, 95t, 96t; booking curves 99, 100f; booking 
limits 84, 85, 86f; dynamic pricing 168–9, 171, 
184; multiple time periods 116; out-of-stock 
events 98; perceived fairness of pricing 217; 
reference pricing 213–14; unconstraining 98–9, 
100f
in-season planning 103
in-season product replenishment 169
in-store promotions 60
incomplete-data (log) likelihood function 122, 123, 124
information technology (IT) system networks 108, 
169, 170
internet retailing see online retailing
‘interpersonal comparisons’ 217
intuition-driven forecasting 41
inverse S-shaped price-response function 163, 187
least squares estimation technique 48–9, 50 f, 51, 55, 
59, 68; price-response function 156, 159, 161
legacy airlines 85
linear price-response function 140 f, 143f, 146t, 149; 
price elasticity 
159, 160t, 161, 162
linear programming 178, 179–80, 181t, 182, 183f, 
184t; bid prices 93, 94, 95, 97
linear regression 10, 36, 114, 220, 222 f, 223f, 
dichotomous logistic regression models 221, 
222f, 223f, 224, 225t; Excel (Microsoft) 51, 
52f, 53f, 54f, 55f, 156; least squares estimation 
technique 48–9, 50 f, 51; maximum likelihood 
estimation technique 55, 56 f, 57f, 58t, 59f, 76
log transformation 73, 74 t, 161, 163t
logistic regression models 193 t, 221, 222f, 223f, 
224, 225t; business-to-business (B2B) 
environments 203, 204, 205f, 206t, 207; 
measuring performance 193 t, 194
logit link function 225–6
logit model 189–90, 191 f, 192, 194
logit price-response function 145, 146 t, 149, 199t, 
200f, 220
long-term forecasts 18, 23, 26, 30, 35
losses see gains/losses
LOTUS algorithm 204, 205, 208
M-like Step 131
MAE see mean absolute error
mail-in rebates 6
manufacturing industry 8–9, 43
MAPE see mean absolute percentage error
marginal costs 79, 85
marginal deal contribution 191 f
markdown pricing 4, 171–4, 184–5, linear 
programming 178, 179–80, 181t, 182, 183f, 184t; 
slow-moving items 174–7, 178 t; 
 see also dynamic 
pricing
market feedback 140
MASE see mean absolute scaled error
maximisation step (M-step) 123, 124, 125, 126
maximum likelihood estimation technique 55, 56f, 
57f, 58t, 59f, 76; dichotomous logistic regression 
models 224, 225 t; price-response function 156; 
unconstraining 117, 122–6
mean absolute error (MAE) 23
mean absolute percentage error (MAPE) 14
mean absolute scaled error (MASE) 15
mean relative absolute error (MRAE) 13–14
mean squared error (MSE) 18, 120; forecasting 23, 
27, 31, 39, 43
median smoothing 71
membership-based segmentation 2
missing values 139
Monte Carlo Simulation 80–1
moving averages 44, 71, simple 18, 19, 20f, 21t, 22; 
exponential 182; weighted 22 f, 23t, 24–5t
MRAE see mean relative absolute error
MSE see mean squared error
multi-leg flights 92
multiple linear regression 60, 76
multiple time series 13, 15, 92, 116
multiplicative models 65, 66–7 t, 72, 74t, 180, 181t
multiplicative seasonality 33, 34 f, 35, 41
multivariate logistic regression model 192, 201, 204, 208
Naïve #3 see averaging method (AM)
nested booking limits 87, 96; expected marginal seat 
revenue model (EMSR) 88f&t, 89, 90, 92t

---

## Page 265

254  Index
network revenue management 92 t, 93f, 94f, 95t, 96t
news vendor model 81 f, 82t, 83; booking limits 86–7, 
88, 89–90, 92, 96; see also capacity-based revenue 
management
‘nonlinear least square estimation’ 220
nonlinear price-response function 147 f, 220
normal distribution 80, 81 f, 82t, 83, 85; expected 
marginal seat revenue model (EMSR) 88 t, 89
objective functions 139, 149, 150 f, 151
odds ratio 225–6
one-step-ahead forecasts 13, 16, 41; exponential 
smoothing 28, 31, 34, 39; simple/weighted 
averages 18, 20, 21
online retailing 100–1, 102 f, 103, 104f, 105f, 106; 
dynamic pricing 169–70, 174, 179, 180, 182; 
elasticity (pricing) 158
online travel aggregators 171
opaque channels 170, 171
open source statistical software see R (open source 
statistical software)
optimal ordering quantity 83
optimisation software packages 174, 214
ordinary least squares method 156, 159, 161
out-of-stock (OOS) events 62, 63, 68, 71, 98, 139; 
double exponential smoothing (DES) 119–20; 
dynamic pricing 169; food retailers 106, 108, 
109t, 110; retail industry 101, 102, 103, 104 f, 174
outliers 139
overage 79, 83, 85, 86, 87, 168; markdowns 171–4, 184
overbooking problem 89
overpricing 156
P-methods 108
package-based pricing 4–5
perceived fairness of pricing 217–18, 219
personalised prices 137
placement 47
planning: history-based 101, 102 f, 103–4
point elasticity 147, 151
Point of Sales (PoS) systems 108
power price-response function 145 f, 146t
prediction intervals 12
predictive analytics 7
price discrimination 188
price execution 139–40
price experiments 157, 158, 159, 160
price optimisation 218; customer segmentation 152; 
customised pricing 190; elasticity and 151, 152; 
objective function 149, 150f, 151
price-ratio elastic demand 73
price-response models 70, 139, 140 f, 141f, 142f, 188; 
common price-response models 143f, 144 f, 
145f, 146t; elasticity and 156, 157–8, 159f, 160 t, 
161, 165; profit function and 249 f; prospect 
theory 216; sensitivity 146, 147 f, 152
price-sensitivity 3, 5, 6, 84, 87, 99; business-to-
business (B2B) environments 187, 190, 191; 
business-to-consumer (B2C) environments 200, 
202; dynamic pricing 169, 172; measures 146, 
147f, 148t, 149f; reference pricing
  213, 214
pricing: perceived fairness of 217–18
pricing analytics 13, 61, 65–6; common price-
response models 143f, 144f, 145f, 146 t; 
measures of sensitivity 146, 147 f, 148t, 149f; 
microeconomic view of consumer-purchasing 
decisions 137; optimisation 149, 150f, 151–2; 
practice of 152, 153 t, 154f, 155–6; price-response 
function 140f, 141f, 142f; process 138f, 139–40; 
see also elasticity (pricing)
pricing capabilities 153 t, 154f, 165–6
private brands/labels 178–9, 180, 181 t
probability density function 57, 58, 142f, 143
probability fractiles (V-methods) 108
product attributes 187
product availability 101, 102 f, 104f, 105f, 116
product customisation 173
product rebates 217
product-based segmentation 2–6
product-level optimal prices 248 t
product-limit estimation technique 106, 107, 108 t, 
110, 119, 134
profit 149, 150 f, 151
projection-detruncation (PD) 126, 128 t, 129f, 130–1, 
134; demand unconstraining 132 t, 133t
promotion forecasting 47–8, 75–6; additive and 
multiplicative models 66–7 t; estimating 
promotion effects 60, 62–3, 65, 68 t, 69f&t, 70; 
food retailing 70, 71 f, 72–3, 74t, 75; planning 
and optimisation 64 t; promotional flyer 
variable 60, 61f; see also regression analysis
promotion history 68 t, 69f, 75
promotion planning and optimisation (PPO) 63, 64 t
promotions: codes 
6; in-store 60; reference 
pricing 215; timing 62–3
proportionality constant 109
prospect theory 215, 216f, 218
protection levels 85, 86f, 89, 90, 92 t, 99
push/pull business model 100, 101
qualitative/quantitative forecasting 10–11, 12
R (open source statistical software environment) 27, 
29, 30, 35, 40, 48; common objects 
in 233–7; getting help in 232–3; getting 
started 230–2; handling external files 
in 240–2; installation 228–30; price-response 
functions 156; retail price setting 247, 248t, 
249f, 250; running R scripts 242–3; sales 
forecasting 243–4, 245 t, 246f, 247t; writing 
functions in 237–40
R-squared values 53, 54, 60, 158
race-based segmentation 2, 3
random walk without drift 13, 23, 31, 39
reference pricing 213–15, 218
regression analysis 7, 47, 75, common mistakes in using 
to forecast 53, 54; Excel (Microsoft) 51, 52f, 53f, 
54f, 55f; linear regression/least squares estimation

---

## Page 266

Index  255
technique 48–9, 50f, 51; linear regression/
maximum likelihood estimation technique 55, 
56f, 57f, 58t, 59f, 76; multiple linear regression 60, 
76; see also promotion forecasting
relative error subclass of forecasting measures 13, 14–15
relative mean squared error (RelMAE) 14–15 
requests-for-proposal (RFPs) 186, 187
retail industry 62; customer behaviour 218; dynamic 
pricing 169, 170–1; elasticity (pricing) 158t; linear 
programming 178–80, 181t, 182, 183f, 184t; 
markdowns 172–3, 174; price setting 247, 248t, 
249f, 250; promotions 65, 68t, 69t&f, 70; reference 
pricing 214; slow-moving items 173, 174–7, 178t, 
184; unconstraining 100–1, 102f, 103, 104f, 105f, 106
reverse s-shaped price-response function 144 f, 145f, 
146t, 189f
RFPs see requests-for-proposal
risk aversity/neutrality 190
safety stock 96, 98
sales 139; daily 106, 107 t, 108, 110, 121t; 
forecasting 243–4, 245 t, 246f, 247t; hourly 
rates 109t, 111–13t, 134
sales agents 187–8, 191, 195
sampling 16, 17–18
SAS (statistical software package) 29, 156
scale-dependent/independent forecasting accuracy 
measures 13–15
scope creep 164
‘screen-scraping’ 214
‘search cost’ 137
seasonal time-based pricing 4, 27, 33, 35, 36, 37 t; 
business travel 84; private brands/labels 
179–80, 181t; promotion and 72, 73, 75; retail 
industry 100–1, 103
segmentation variables 192, 193
sell-outs see out-of-stock events
shadow prices 95
short-run elasticity 152
simple exponential smoothing 25–7, 28 f, 29t; see 
also double exponential smoothing; triple 
exponential smoothing
simple linear regression 75–6
simple moving average 
18, 19, 20f, 21t, 22
single orders opportunity inventory problem 77, 78 t, 
79t, 80t, 81; retail industry 101
single-period items 106, 107 t, 108t, 110, 114t, 115
slow-moving items 173, 174–7, 178 t, 184
social networks 6
spiral down phenomenon 99, 105–6
SPSS (Statistical Product and Service Solutions): 
forecasting manual sales 39, 40 f, 41, 42f&t, 43t, 
44f, 45
Standard Normal Distribution 82 t
Stata (statistical software package) 156
state space models 11, 12
static pricing 168, 170, 174
statistical software packages see R; SAS; STATA
stock-outs see out-of-stock events
technology and entertainment products 
retailing 234–6
textile industry see fashion industry
third-party search engines 6
time series forecasting 7, 10, 11, 18, 44, 47
time-dependence 172, 173
time-indifference 126
Tocher’s inverse cumulative demand distribution 
function 110, 114 t, 115
tracking signal 16, 25
travel industry 1, 84, 213
tree-based classification algorithms 198 f, 199t, 200f, 
201, 204
trendlines 51, 53, 55
trial and error method 80, 81
triple exponential smoothing 33, 34f, 35, 36f, 37t, 
39t; illustration of use 16; in-sample forecasting 
accuracy measures 38 t; see also double 
exponential smoothing; simple exponential 
smoothing
uncertainty 9, 11, 75, 121, 138, 215; business-to-
business (B2B) environments 187, 189; 
capacity-based revenue management 81, 93, 96, 
97; dynamic/markdown pricing 169, 172, 173, 
180
unconstraining 98–9, 100 t, 33–4; averaging 
method (AM) 115t, 116–17, 118t, 119t; double 
exponential smoothing (DES) 119, 120 t, 121t, 
122f; estimation of demand distribution of 
censored single-period items 106, 107 t, 108t, 
110, 114t, 115
 ; expectation-maximisation (EM) 
algorithm 122–6, 127t; hourly sales rates 109 t, 
111–13t; out-of-stock (OOS) events 101, 102 f, 
103, 104f, 105f, 106; projection-detruncation 
(PD) 126, 128t, 129f, 130–1, 132t, 133t
underage 79, 83, 86, 87
underpricing 156, 160
utility 137, 213, 219
V-methods (probability fractiles) 108
validation samples 41
Validation step 63
variables 48, 51, 54, 55, 60; pricing 167–8
versioning 3
weighted moving average 22 f, 23t, 24–5t
willingness-to-pay (WTP) 3, 84, 85, 87, 98, 137; 
customer behaviour 217; dynamic pricing 168, 
170; price sensitivity 147, 149, 152; price-
response function 141 f, 142f, 143, 144, 165
win probability 191 f
win/loss probability 192, 193 t
winner-takes-all bidding situations 188
Yield Management see Capacity-Based Revenue 
Management
z-value 83

---

## Page 267

Taylor & Francis 
eBooks 
FOR liBRARIES 
Over 23,000 eBook titles in the Humanities, 
Social Sciences, STM and Law from some of the 
world's leading imprints. 
Choose from a range of subject packages or create your own! 
~ Free MARC records 
~ COUNTER-compliant usage statistics 
~ Flexible purchase and pricing options 
~ Off-site, anytime access via Athens or referring URL 
~ Print or copy pages or chapters 
~ Full content search 
~ Bookmark, highlight and annotate text 
~ Access to thousands of pages of quality research 
at the click of a button 
For more information, pricing enquiries or to order 
a free trial, contact your local online sales team. 
UK and Rest of World: online.sales @tandf.co .uk 
US, Canada and Latin America : 
e-reference@taylorandfrancis.com 
www.ebooksubscriptions.com 
f.{
LPSPAW"dfm @ &ESTeBOOK • ... 
PUBLISHE. • Taylor & FrancIs r:!.1im;! 
• 2 =:.1~~ Taylor & Francis Group
