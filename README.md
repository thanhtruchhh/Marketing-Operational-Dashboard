# Marketing Operational Dashboard Project

## Project overview

A flower shop leverages Facebook ads to enhance reach, foster engagement, and ultimately boost revenue. With each campaign tailored to specific customer segments, our goal is to achieve diverse objectives aimed at captivating audiences.

To streamline the management and optimize the performance of these campaigns, we introduce an interactive dashboard. This dashboard caters to the needs of marketing personnel and those responsible for executing Facebook ad strategies. It serves as a comprehensive tool for real-time monitoring, providing timely alerts to address concerns such as excessive spending or underperforming campaigns.

In particular, our end users are keenly focused on the key metric of "Cost per Mess" as a pivotal indicator of campaign effectiveness. A higher Cost per Mess implies that the campaign is less efficient.

This project was built on Google Sheet. You can access the result file directly [here](https://docs.google.com/spreadsheets/d/1H5GB4YMnA3J-RNzYCvU19ZFCKR4yG9n6mFG8Ow3Z9Xw/edit?usp=sharing).

## 2. Data Dictionary

| Column              | Description                                           |
|---------------------|-------------------------------------------------------|
| Reporting starts    | Date of the report                                    |
| Campaign name       | Name of the campaign                                  |
| Ad Set Name         | Subset within a campaign                              |
| Ad name             | Individual ad within an ad set                         |
| Objective           | Campaign objective                                    |
| Reach               | Number of people reached                              |
| Impressions         | Number of ad views                                     |
| Frequency           | Impressions per unique viewer (Frequency = Impressions/Reach) |
| Amount spent (VND)  | Total expenditure in Vietnamese Dong                   |
| CTR                 | Click-through rate                                    |
| CPC (All) (VND)     | Cost per click                                        |
| CPM (VND)           | Cost per 1,000 impressions                             |
| Cost per 1,000 people reached (VND) | Cost per 1,000 people reached                 |
| Conversions         | Number of conversions                                 |
| Conversion values   | Value of successful conversions                       |
| Cost per conversion | Cost per conversion                                   |
| Post comments       | Number of post comments                               |
| Link clicks         | Number of link clicks                                 |
| Messaging Conversations Started | Number of initiated messaging conversations |

The dataset is in Vietnamese. You can download the original dataset [here](https://docs.google.com/spreadsheets/d/1ltfJFzrKwA87iO-tcMkR2FnPGTQD9Hy1hQgHvymByH8/edit?usp=sharing).

## Approach

 - Establishing an interactive layer where data dynamically changes based on user filters.
 - Ensuring that the information presented in the tables and charts across the dashboard is seamlessly drawn from this layer.

## Output

<img width="654" alt="Marketing Operational Dashboard Capture" src="https://github.com/thanhtruchhh/Marketing-Operational-Dashboard/assets/145547282/a6c0542b-b055-4bf2-bad2-4d9878009b17">

The project comprises a Google Sheet with multiple sheets. The main component is the "Dashboard" sheet, featuring:

- Filters: Location, Start date, End date.
- Users can input a Target Cost per Mess. If the Average Cost per Mess exceeds the target, the dashboard issues a warning.
   <img width="827" alt="Average Cost per Mess" src="https://github.com/thanhtruchhh/Marketing-Operational-Dashboard/assets/145547282/db4a31b0-35f0-418d-9561-a70225daa759">
- Scorecards displaying key KPIs: Total spend, Total mess, Avg cost per mess, Total mess of messages campaigns, Total mess of engagement campaigns.
- Three charts illustrating Total spend, Total mess, and Cost per mess over time.
- Three tables showcasing:
    - Top 5 efficient campaigns.
    - Top 5 inefficient campaigns.
    - Top 5 spent campaigns.

To ensure accessibility for all end users, including those with color blindness, alerts in the dashboard are presented using a combination of background color changes and symbols:
- `✓` + Green background: Good Performance
- `⚠` + Light red background: Needs Improvement
- `⨉` + Dark red background: No Effectiveness
  <img width="679" alt="Warnings" src="https://github.com/thanhtruchhh/Marketing-Operational-Dashboard/assets/145547282/a5dc30ee-c5a9-4204-8ee8-da225186bb57">
