# Pipeline Visibility Cheat Sheet

**Author:** Weflow  
**Format:** PDF  
**Category:** reference

---

## Page 1

Warnings 
Complexity: low               Accuracy: low to medium Complexity: medium to high              Accuracy: high Complexity: high               Accuracy: medium to high
What Pitfalls
Who Monday Tuesday Wednesday Thursday Friday
CRO   Forecast meeting with
managers, RevOps, etc.      
RevOps Analysis & question
formulation Formulate action items Chase action items
from week before    
Managers   Forecast meeting with reps to
inspect & adjust
Reps       Forecast call
submission  
Forecast tool Forecast call lock,
snapshot, pacing   Reminder (submission,
pipeline hygiene)
Final submission
reminder
Automated roll-up,
adjustments & track change
4. Reporting & Snapshots
Why What Implementation
What Pitfalls Implementation
Implementation
What Pitfalls
Consistently applying a sales methodology helps you
separate unqualified from real deals. Technology can help
you sync your methodology to your CRM so you get
consistent data while your reps can focus on qualifying.
Solution: Auto-sync MEDDIC (or other qualification) fields to
the right Salesforce records based on meeting recordings
(e.g. with Weflow)
Create AI field templates and prompts
Auto-sync to multiple Salesforce records
Reps can now focus on the deal
Activity Data Meeting Notes
Pipeline Visibility Cheat Sheet
Automate CRM data capture: Clean opportunity data is the foundational element to deal execution, reviews, and forecasting
MEDDIC, SPICED, etc. data Key CRM fields
Accurate CRM fields ensure that deal reviews and forecasts
are based on real-time, high-quality data. Missing or
inaccurate information means you lack visibility.
Solution: Use stage exit criteria to drive the completion of
data fields that informs deal reviews and forecasts:
Stage
Amount
Close date
Products (if used)
Forecast category (often automated)
Sales conversations contain critical details about deal
status, objections, and next steps. Manual note-taking is
time-consuming and inconsistent, leading to lost insights
and poor CRM hygiene.
Solution: Auto-record, transcribe, and summarize meetings
to improve rep productivity and Salesforce hygiene (e.g.
with Weflow)
Automate note-taking
Generate AI meeting summaries
Sync recordings & summaries to Salesforce
Complete activity data ensures visibility into deal velocity
and progression. Ideally, it also reveals insights into the
buying committee. However reps often forget to log critical
interactions, leading to incomplete data & missing visibility.
Solution: Auto-capture emails, meetings, and contacts from
Google Workspace or Microsoft 365 (e.g. with Weflow)
Automate activity capture
Map activities to opportunities
Enable reps to see and adjust attribution in Outlook/
Gmail/ Google Calendar
Warnings Signals Views
Assessing pipeline health: Analytics to help you identify pipeline gaps and trends early
See how your pipeline value is pacing over time. Drill
into opportunities driving those changes by
segment, geo, stage, or forecasting categories.
Pipeline Value & Pacing Pipeline Waterfall Stage Conversion & Win Rate Pipeline CoverageOpportunitites Created Sales Cycle Length
3. Roll-up
Dynamic weighted forecast AI forecastBottom-up forecast
Each stage has a closing probability that is multiplied by the deal amount.
Weighted forecasts are an easy, low-effort way to get started.
Typically, companies run a weekly-, or bi-
weekly forecast cadence to submit, review,
and adjust forecast calls. Start with one team
and a simple cadence before involving the
entire revenue org. If done right, bottom-up
forecasts give you highly accurate forecasts.
AI forecasts based on historical data, snapshots, and deal velocity.
Treat it as an additional data point after rolling up your bottom-up forecast. 
and / or and / orExample Pitfalls What to weight on
Probability * amount = 
weighted forecast
Discovery stage: 10%
Demo stage: 20%
Value alignment: 35%
Proposal: 60%
Negotiation: 90%
Closed Won: 100%
Unclear stage exit criteria 
Sales stages not followed
Probabilities are wrong
Probabilities are hard-coded
Probabilities are not
adjusted over time
Stage
Forecast categories
(pipeline, best case,
commit, most likely)
Other (depending on your
unique sales motion and
business requirements) 
Poor process governance
Poor data and pipeline hygiene inevitably
lead to inaccurate forecasts
Missing forecast submissions
Failing to create a culture and
accountability around forecasting
Operating cadence (example) 1. Forecast submission 2. Inspection & Adjuments
Advanced forecast tools
allow you to roll up your
forecast by role
hierarchy, product, or
territory. They also allow
you to see how the
forecast call has
changed (increased or
decreased), how often,
and by whom.
Snapshot your pipeline & forecast to track deal, pipeline, & forecast changes.
Deals and forecasts
change week by week:
Slipped to next
quarter
Stage progression
Amount changes
Pipeline: 
number of deals
deal amount
forecast category
close date
Forecast: amount
Duplicate spread-
sheet tabs
Snapshot reporting
in Salesforce
Forecasting tool 
Database (BigQuery)
Each manager can
adjust the forecast calls
of reps who report to
them. The better your
data and visibility into
deals, the more
accurate adjustments
will be. 
No track change
No adjustment
notes
No deal-by-deal
adjustment
snapshots
Poor deal hygiene
Spreadsheet: Use
comments to adjust
(not reliable as it’s not
tracked/stored)
Salesforce: Not
possible
Forecasting software
(getweflow.com)
Advanced forecast tools
allow you to submit
forecast calls 
by including/ excluding
deals into your forecast
calls. Deal insights help
you get better visibility
and make a more
accurate forecast call.
AI can help you get a more holistic forecast
by considering patterns and factors beyond
those typically taken into account for
weighted or bottom-up forecasts. Examples:
Deal velocity
Past forecast accuracy by rep/manager
Closed/won probability depending on
multivariate deal characteristics 
Poor data and pipeline hygiene inevitably
lead to inaccurate forecasts
Changes in processes or external factors
take time to be reflected in your forecast
High technical complexity often requires
internal resources and knowledge
Black box characteristics can lead to low
trust within the org
Reps and/or managers submit forecast calls that roll up the organization.
Start with one team to reduce initial complexity before rolling it out.
Revenue & Sales Forecasting: Use multiple methodologies to run your new logo, expansion, and renewals forecast
Assessing deal health: Use deal insights to inspect deals, identify risks, and define next steps
Deals without clear next steps often stall or slip.
Ensuring every opportunity has a defined action
plan helps move deals forward and keeps them on
track. You need a clear future commitment in the
form of: 
group demo scheduled
trial onboarding schaeduled
security meeting scheduled
legal red line process and intro done
Next steps
How frequent are touch points on the opp/account?
A healthy deal will have frequent touch points
facilitated by both parties. Low activity velocity can
indicate stalled deals, lack of urgency, or loss of
interest. Get visibility into:
Numbers of emails sent/ received
Number of meetings scheduled (past, future)
Number of redlines exchanges
Flag deals with declining engagement
Activity velocity Multi-threading Access to power Review communication Sales methodology
Identify that there are multiple customer contacts
actively engaged in the deal. How many people are
involved in the conversation?
Multi-threading helps ensure that you build a base
of influencers, including anyone who will have an
input in the decision-making process. Winning deals
typically have multiple champions.
Check to make sure each deal has not only multiple
stakeholders engaged but the key decision-makers.
Are you in touch with the right people? Deals should
include the person who recommends the purchase
decision and the person who approves it.
Bring yourself up to speed quickly by drilling into the
latest calls and email conversations. Sometimes a
good level of engagement, solidified next steps, and
being in touch with the right people can provide a
false sense of security—what's missing here is
context.
Use AI to summarize deal communication.
Whether you use MEDDICC, MEDDPICC, SPICED,
BANT, or a combination of those - sales
methodologies are frameworks that help you
understand the health of an opportunity, and
increase the likelihood of getting deals done.
Disclaimer - ensure fields are auto-updated to get
the context of the deal.
Configure warnings to identify
opportunities at risk and take action. 
Examples:
Slipped
Ghosted
Stalled in stage
Single threaded
No access to power
Cycle Length Overdue 
No activity over the last X days 
Opportunity signals (like Weflow deal
signals) that can be added to pipeline
views.
Examples:
Deal age
Inactivity
Days in Stage
Last activity data
Engagement score
Next meeting date
Closed date pushed
Pipeline views to help sales leaders
and reps to focus on moving deals
forward.
Examples:
Swing deals
Deal reviews
Deal hygiene
Renewal pipeline
Expansion pipeline
Next quarter pipeline
My opportunities - this quarter
Analyze revenue leakage throughout your stages
by analyzing stage conversion and win rates.
Tracking the creation of new opps and analyze which
channels are driving opportunity creation
Analyze and track pipeline coverage to make
sure you’re on track to reach your revenue goals.
Measure sales cycle length by by segment, geo,
team, or rep to shorten your cycle length.
Track how your pipeline changes over time. See
what drives those changes like e.g. new opps,
amount changes, closed-won/lost or pulled-
in/slipped opportunities. 
Source: Weflow (getweflow.com) Source: Weflow (getweflow.com) Source: Weflow (getweflow.com)
Source: Weflow (getweflow.com) Source: Weflow (getweflow.com) Source: Weflow (getweflow.com) Source: Weflow (getweflow.com) Source: Weflow (getweflow.com) Source: Weflow (getweflow.com)
Source: Weflow (getweflow.com)
Source: Weflow (getweflow.com)
Revenue Intelligence powered by AI 
   
 A c t i v i t y  C a p t u r e    P i p e l i n e  M a n a g e m e n t   
 C o n v e r s a t i o n  I n t e l l i g e n c e    S a l e s  F o r e c a s t i n g
