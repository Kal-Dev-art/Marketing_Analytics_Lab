# Marketing Analytics Lab

## Project Overview

The Marketing Analytics Lab is a hands-on project I created to develop practical experience across marketing analytics, CRM, marketing automation, customer segmentation, website tracking, and business intelligence.

The project simulates an end-to-end marketing technology and analytics environment where website activity can generate CRM data, contacts can be segmented based on their interests and behavior, marketing workflows can respond to those contacts, and campaign performance can be analyzed through business intelligence reporting.

Rather than focusing on a single platform, this lab demonstrates how CRM, marketing automation, customer data, analytics, and business intelligence can work together to support data-driven marketing decisions.

---

## HubSpot CRM & Marketing Automation

I integrated the lab website with HubSpot to create a hands-on CRM and marketing automation environment.

The website includes an embedded lead-capture form that collects:

- First Name
- Last Name
- Email
- Company Name
- Job Title
- Primary Interest

The Primary Interest field allows contacts to identify areas such as Data Analytics, Business Intelligence, CRM & Marketing Automation, and SEO & Search Analytics.

Form submissions create CRM contact records that can be used for segmentation and marketing workflows.

### CRM & Automation Implementation

- Integrated HubSpot website tracking with the lab website.
- Embedded a HubSpot lead-capture form.
- Created and configured custom CRM properties.
- Captured website visitors as CRM contacts.
- Created contact segmentation based on Primary Interest.
- Tested contact lifecycle activity and CRM data collection.
- Built an automated post-submission workflow.
- Created personalized follow-up email communication triggered by form activity.
- Tested the complete visitor-to-contact-to-automation workflow.

This portion of the project demonstrates how website interactions can become structured CRM data that supports segmentation, personalization, and automated marketing communication.

---

# Power BI Marketing Analytics & Business Intelligence Dashboard

## Dashboard Overview

The Power BI component of the Marketing Analytics Lab is an end-to-end business intelligence solution designed to analyze marketing campaign, channel, customer activity, lead, conversion, spend, and revenue data.

The dashboard transforms raw marketing data into an interactive executive reporting environment that can be used to evaluate campaign performance, monitor marketing KPIs, compare acquisition channels, identify performance trends, and support data-driven decision-making.

The project covers the full Power BI workflow from data preparation and transformation through dimensional modeling, DAX development, visualization, and interactive dashboard design.

---

## Key Performance Indicators

The Power BI model includes measures for:

- Total Impressions
- Total Clicks
- Click-Through Rate (CTR)
- Total Leads
- Total Conversions
- Conversion Rate
- Lead Conversion Rate
- Total Marketing Spend
- Cost Per Click (CPC)
- Cost Per Lead (CPL)
- Cost Per Conversion
- Total Revenue
- Return on Ad Spend (ROAS)

---

## Technical Implementation

### Data Preparation & Power Query

Raw campaign, contact, and activity datasets were imported into Power BI and prepared using Power Query.

Data preparation included:

- Reviewing column data types and data quality.
- Transforming date and datetime fields for time-based analysis.
- Creating a date-only activity field from activity timestamps.
- Cleaning inconsistent text values.
- Identifying and correcting leading and trailing whitespace that initially caused relationship cardinality problems.
- Validating transformed data before loading it into the analytical model.

### Data Modeling

A dimensional model was developed to support reliable filtering and analysis across multiple datasets.

The model includes:

- `RawContacts`
- `RawActivities`
- `RawCampaignPerformance`
- `DimCampaign`
- `DimDate`
- Dedicated DAX measurement table

One-to-many relationships were created between dimension and fact-like tables using campaign IDs, contact IDs, and dates.

Single-direction filtering was used to maintain a clean and predictable analytical model.

The campaign dimension was created to provide reusable campaign attributes such as Campaign ID, Campaign Name, and Channel.

A dedicated date dimension was created to support monthly and chronological trend analysis.

### DAX Measures

Reusable DAX measures were developed for traffic, funnel, cost, conversion, and revenue analysis.

Examples include:

- Total Impressions
- Total Clicks
- CTR
- Total Leads
- Total Conversions
- Conversion Rate
- Total Spend
- Cost Per Click
- Cost Per Lead
- Cost Per Conversion
- Total Revenue
- ROAS

DAX measures were organized within a dedicated measurement table to keep the analytical model structured and maintainable.

### Time Intelligence & Sorting

A reusable date dimension was implemented to support time-based reporting.

Month and year fields were configured for chronological sorting so that monthly performance visualizations display in the correct calendar sequence rather than alphabetical or metric-based order.

---

## Dashboard Features

The finished Power BI dashboard includes:

### Executive KPI Summary

Headline cards provide an immediate view of:

- Impressions
- Clicks
- CTR
- Leads
- Conversions
- Marketing Spend

### Campaign Performance

An interactive campaign comparison analyzes clicks and leads across individual marketing campaigns.

### Monthly Performance Trend

A time-series visualization compares clicks and leads across months to identify changes in marketing performance over time.

### Channel Performance

Channel-level analysis compares lead generation and conversions across marketing channels.

### Interactive Filtering

The dashboard includes interactive slicers for:

- Marketing Channel
- Month / Year

Selections dynamically update KPI cards and dashboard visualizations, allowing performance to be analyzed for specific channels and periods.

---

## Business Questions Addressed

The dashboard is designed to help answer questions such as:

- Which campaigns generate the most traffic and leads?
- Which marketing channels produce the strongest lead and conversion performance?
- How does marketing performance change over time?
- What percentage of impressions generate clicks?
- How efficiently does marketing spend generate leads and conversions?
- How do campaign results change when filtering by channel or reporting period?
- Which areas of marketing performance may require additional investment or optimization?

---

## Tools & Technologies

- Power BI
- Power Query
- DAX
- Microsoft Excel
- HubSpot CRM
- HubSpot Marketing Automation
- HTML
- GitHub Pages
- Data Modeling
- Dimensional Modeling
- Data Visualization
- Marketing Analytics
- CRM Analytics
- Customer Segmentation
- Business Intelligence

---

## Skills Demonstrated

This project demonstrates hands-on experience across an integrated marketing analytics workflow, including:

- CRM data management
- Marketing automation
- Lead capture
- Customer segmentation
- Personalized marketing workflows
- Data cleaning and transformation
- Power Query
- Dimensional data modeling
- Relationship design
- DAX measure development
- Marketing KPI development
- Campaign performance analysis
- Channel performance analysis
- Conversion analysis
- Interactive dashboard development
- Business intelligence reporting
- Data visualization
- Data-quality troubleshooting
- Translating marketing data into business insights

The project demonstrates how customer data can move from website interaction and CRM capture through segmentation and automation and ultimately into analytics and business intelligence reporting.

---

## Dashboard Preview

![Marketing Performance Dashboard](power-bi/dashboard-screenshot.png)

---

## Project Purpose

This lab was built as a practical environment for expanding my experience across marketing technology, CRM, automation, digital analytics, and business intelligence.

The goal is to continue developing the environment by integrating additional analytics and marketing technologies and using the resulting data to build increasingly advanced measurement, segmentation, automation, and reporting workflows.
