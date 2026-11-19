# Purplle Marketing Campaign Performance Dashboard

An interactive Power BI project that analyzes marketing campaign performance across campaign types, channels, target audiences, languages, and time periods. The goal is to help a marketing team understand where revenue and conversions are coming from, how efficiently marketing spend is being used, and which campaigns may need attention.

## Business Problem

Marketing teams may run many campaigns across multiple channels and audience groups. Looking only at total revenue does not show whether the campaigns are cost-efficient or profitable.

This project explores five business questions:

1. Which campaign types contribute to revenue, conversions, and profit?
2. Which marketing channels generate stronger revenue and click-through rates?
3. How do CPC, CAC, and CPL vary across channels and target audiences?
4. Which target audiences and languages show stronger conversion performance?
5. How do profit and ROI change by month, quarter, campaign type, and campaign duration?

## Dashboard Overview

The report contains four interactive pages.

### 1. Campaign Performance Overview

- High-level campaign performance and KPI summary
- Monthly revenue and performance trend
- Revenue compared with acquisition cost
- Engagement score by campaign type
- Funnel analysis: impressions → clicks → leads → conversions
- Campaign-level performance table
- Filters for language, campaign type, and customer segment

### 2. Channel Analysis

- Revenue contribution by marketing channel
- CTR comparison across channels
- CPC and CAC comparison by channel
- CTR distribution by campaign type
- Helps investigate which channels attract engagement and which are more expensive to use

### 3. Target Audience Analysis

- Conversion rate by target audience
- Revenue contribution by customer segment
- CTR and conversion rate by language
- Cost per lead (CPL) by target audience
- Language-level performance table
- Month, language, campaign type, and customer segment filters

### 4. Campaign Performance and Trend

- Profit contribution by campaign type
- Bottom 10 campaigns by profit
- Quarterly ROI comparison
- Monthly revenue and profit trend
- ROI by campaign duration bucket

## Dataset Snapshot

The project dashboard was built using campaign data with the following reported aggregate totals:

| Metric | Reported total |
|---|---:|
| Revenue | 28,540,346,627 |
| Impressions | 6,120,750,589 |
| Clicks | 260,138,378 |
| Conversions | 57,126,268 |
| Campaigns | 55,555 |
| Leads | 103,912.846 |

*These are aggregate values supplied for the project. Confirm the report's filters, data types, and measure definitions before using them in formal business reporting. Currency and lead units should be documented from the source dataset.*

## Key Insights to Derive from the Dashboard

The report is designed to identify the following insights. The actual winning channels, audience groups, campaign types, and periods should be stated only after checking the corresponding visual values and slicer selections.

- **Campaign effectiveness:** Compare campaign types by revenue, acquisition cost, conversions, and ROI to distinguish high-revenue campaigns from cost-efficient campaigns.
- **Channel efficiency:** Compare channel revenue and CTR alongside CPC and CAC. A channel with many clicks is not automatically the channel with the best conversion or acquisition efficiency.
- **Audience quality:** Compare conversion rate and CPL by target audience. This helps distinguish audiences that engage from audiences that convert efficiently.
- **Language performance:** Compare CTR and conversion rate by language to identify differences in engagement and conversion.
- **Profitability:** Use the profit-by-campaign-type visual and bottom-10 campaign table to locate campaigns that may be reducing overall profitability.
- **Time trends:** Compare monthly profit and revenue and quarterly ROI to identify periods that need further investigation.
- **Campaign duration:** Compare ROI across duration buckets to understand whether campaign length is associated with different returns.

## Business Recommendations

Recommendations should be finalized after validating the actual values and filters in the report. The analysis supports these decision areas:

1. **Reallocate budgets carefully:** Test increasing investment in channels and campaign types that show stronger ROI and acceptable CAC, rather than allocating budget based on clicks or revenue alone.
2. **Review expensive channels:** Investigate channels with high CPC or CAC. Check audience targeting, creative quality, landing-page experience, and conversion tracking before reducing spend.
3. **Prioritize converting audiences:** Consider targeted experiments for audience groups with stronger conversion rates and efficient CPL.
4. **Improve low-profit campaigns:** Review the bottom 10 campaigns by profit, including their revenue, acquisition cost, campaign type, and targeting. Pause or redesign only after confirming the cause.
5. **Plan around performance trends:** Use monthly profit and quarterly ROI patterns to guide campaign timing and budget planning.
6. **Test campaign duration:** Compare duration buckets and run controlled tests before deciding whether shorter or longer campaigns deliver better returns.
7. **Monitor the full funnel:** Track impressions, clicks, leads, and conversions together. This helps locate where potential customers drop out of the campaign journey.

## Data Preparation and Validation Considerations

- Check whether `Channel_Used` contains multiple channel names in one value (for example, `Facebook, Google`).
- If multi-channel values are split into separate rows, define an attribution approach before aggregating revenue, cost, leads, or conversions. Otherwise, campaign totals may be duplicated across channels.
- Validate blanks, duplicate campaign identifiers, data types, and date fields.
- Confirm the definitions and calculation logic for ROI, profit, CTR, CPC, CAC, CPL, and conversion rate.
- Check whether the lead field is a count or a calculated/weighted value before presenting it as a whole-number lead total.

## KPIs and Measures

The report includes analysis of:

- Revenue
- Acquisition cost / total cost
- Profit
- ROI
- Impressions
- Clicks
- Leads
- Conversions
- Click-through rate (CTR)
- Cost per click (CPC)
- Customer acquisition cost (CAC)
- Cost per lead (CPL)
- Conversion rate
- Engagement score

*Use the DAX definitions in the Power BI model as the source of truth for each metric.*

## Tools and Technologies

- **Microsoft Power BI** — interactive dashboard and reporting
- **Power Query** — data preparation and transformation
- **DAX** — KPI and analytical measures
- **Data visualization** — campaign, channel, audience, funnel, and trend analysis

## How to Use

1. Download or clone this repository.
2. Open `purplle_1.pbix` in Microsoft Power BI Desktop.
3. Navigate through the four report pages.
4. Use the slicers to explore language, campaign type, customer segment, and month where available.
5. Compare the visuals together before drawing conclusions. For example, review revenue alongside profit and ROI, and clicks alongside conversions and CAC.

## Repository File

- `purplle_1.pbix` — Power BI report containing the dashboard, visuals, and data model.

## Skills Demonstrated

Power BI · Power Query · DAX · Marketing Analytics · KPI Analysis · Data Visualization · Funnel Analysis · Profitability Analysis · Business Problem Solving · Data Validation

---

**Author:** Priya Darshini P.  
**Project:** Purplle Marketing Campaign Performance Dashboard
