# Adult-Social-Care-Dashboard
Power BI dashboard analysing Adult Social Care performance across 153 English councils
# Adult Social Care Performance Dashboard

A Power BI dashboard analysing Adult Social Care outcomes and financial pressure across 153 English local authorities, built using NHS Digital's ASCOF 2023-24 dataset.

## Why I built this

I'm job hunting for Performance Officer / Information Analyst roles in the public sector, and I wanted something that proved I can actually work with real, messy government data — not just a tidy tutorial dataset. So I picked NHS Digital's Adult Social Care Outcomes Framework data and built a dashboard that tells a proper story: how councils are performing, what's driving the pressure on them, and what's coming next.

## What's in it

**Page 1 — National Overview**
National averages for social contact (59.26%) and care home admissions (14.98 per 100,000), plus the 11 worst-performing councils and a map showing where every council sits.

**Page 2 — Council Performance**
A RAG-rated table of all 153 councils (red/amber/green based on social contact score), a region filter, and a scatter plot testing whether councils that spend more actually get better outcomes.

**Page 3 — Financial Pressure**
Context on the £27.1bn national ASC spend (up 14.2% in a year) and what that means for service delivery.

**Page 4 — Policy Context**
A look at what happens next, given the UK Shared Prosperity Fund ended in March 2026 with no confirmed replacement for the preventative services that keep people out of care homes.

## Skills this shows

- **Data cleaning**: NHS Digital suppresses small numbers with "x" for privacy reasons (disclosure control) — I had to handle that properly in Power Query rather than just letting totals silently break
- **DAX**: custom measures to split out specific outcome metrics from a single value column
- **Table relationships**: joined my main dataset to an ONS council-to-region lookup table so I could filter by region
- **Data storytelling**: not just charts for the sake of charts — the dashboard moves from performance → spend → policy risk, the way an actual analyst would frame it for a council or NHS audience

## Tools used

Power BI Desktop, Power Query, DAX, ONS open geography data

## Data sources

- NHS Digital, [Measures from the Adult Social Care Outcomes Framework (ASCOF) 2023-24](https://digital.nhs.uk/data-and-information/publications/statistical/adult-social-care-outcomes-framework-ascof)
- NHS Digital, [Adult Social Care Activity and Finance Report 2023-24](https://digital.nhs.uk/data-and-information/publications/statistical/adult-social-care-activity-and-finance-report/2023-24)
- ONS, Local Authority District to Region (December 2023) Lookup
- UK Government, [UK Shared Prosperity Fund Prospectus](https://www.gov.uk/government/publications/uk-shared-prosperity-fund-prospectus)
