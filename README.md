# Insurance-Claims-Dashboard

INSURANCE
Claims Processing Dashboard — Analysis Report
Source: 05_insurance_claims.csv · 3,000 claims
Prepared by: Arunabha Lahiri
Report type: Dashboard analysis & insights summary
Companion to: Power BI portfolio dashboard build
Executive Summary
Of 3,000 claims filed, 64.1% were approved, with an average processing time of 8.5 days. 7.7% of all claims were flagged for potential fraud, and 18.7% of claims breached a 14-day service-level target. Total claimed value was $23.94M against $12.94M actually approved for payout — a gap that reflects the combined effect of rejections, partial approvals, and claims still in progress. Processing speed is broadly consistent across regions, with a difference of only 0.6 days between the slowest and fastest region.
Detailed Analysis
1. Claims Pipeline & Status
Of the current book, 1,923 claims are Approved, 480 are Pending, 351 are Rejected, and 246 remain Under Investigation.
The 726 claims still open represent the working backlog operations should focus on clearing first, since they carry the most schedule risk against SLA targets.
2. Processing Time by Region
Average processing time ranges from 8.3 days in Mumbai (fastest) to 8.9 days in Bangalore (slowest). The spread between regions is narrow (under a day), which suggests processing time is not strongly driven by region-specific operational bottlenecks, and any SLA improvement effort should look at claim-type or complexity drivers instead.
18.7% of all claims currently exceed a 14-day processing target, which is the more actionable SLA metric to track going forward.
Recommendation: since regional variation is minor, focus SLA improvement on claim complexity and documentation completeness rather than restructuring regional teams.
3. Financial Exposure by Policy Type
Claimed vs. approved amount by policy type: Auto claimed $9.56M, approved $5.38M (56.3% of claimed value); Health claimed $6.92M, approved $3.74M (54.1% of claimed value); Property claimed $5.05M, approved $2.78M (55.1% of claimed value); Life claimed $2.42M, approved $1.04M (42.9% of claimed value).
4. Fraud Exposure
Overall fraud-flag rate is 7.7%. By incident type, Medical Emergency carries the highest flag rate at 8.9%, meaningfully above the claim-book average.
Fraud flag rate differences across incident types are relatively modest (roughly 6-9%), suggesting fraud risk is spread fairly evenly rather than concentrated in one incident category — a useful finding for calibrating investigation resourcing.
Recommendation: while Medical Emergency claims warrant a modest extra layer of review, the narrow spread across incident types means blanket, category-wide fraud rules would likely be less effective than claim-level anomaly scoring.
Key Recommendations
1. Prioritize clearing the 726-claim open backlog to reduce SLA breach rate below the current 18.7%.
2. Investigate processing time by claim complexity/documentation completeness rather than region, since regional variation is minimal.
3. Review approval-rate gap by policy type — Life claims show the lowest approved-to-claimed ratio and warrant a closer look at rejection reasons.
4. Calibrate fraud review resourcing using claim-level scoring rather than incident-type rules, given the narrow spread in fraud rates across incident types.
Data & Methodology Notes
This dataset is synthetically generated for portfolio purposes; claim amounts, statuses and fraud flags are randomly distributed and do not reflect a real insurer's book. A production version of this analysis would also incorporate earned premium to calculate a true loss ratio, and adjuster-level review notes to validate fraud flag accuracy.
Methodology: figures in this report are computed directly from the underlying row-level dataset (not estimated), using the same aggregation logic as the DAX measures defined for the companion Power BI dashboard, so the numbers here should reconcile with the dashboard's KPI cards and charts.
