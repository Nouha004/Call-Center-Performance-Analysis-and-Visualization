# Call Center Team Performance Dashboard
![Pizza Sales Dashboard](Call_center.png)
![Pizza Sales Dashboard](Call_center2.png)

# Overview
This project features a comprehensive Call Center Team Performance Dashboard that provides insights into agent performance, call metrics, and operational efficiency. The dashboard is built on a structured data model that enables detailed analysis of call center operations across multiple dimensions.

# Data Model Structure
The dashboard is built on a sophisticated data model with the following components:

**1. Core Data Tables**

Agent Table: Contains agent information including:

Agent names and identifiers

Contact information (email, address)

Agent images for visual recognition

Additional agent information

Call Facts Table: Contains detailed call records including:

Call ID and timestamps

Talk duration metrics

Answer status (answered/unanswered)

Department information

Time details (hour, minute)

Calendar Dimension: Temporal analysis framework with:

Date hierarchy

Day, month, and weekday information

Month-run sequencing for period comparisons

Weekday classification

**2. Performance Metrics Framework**

The model calculates comprehensive performance indicators:

Answer Performance Metrics:

Answered calls (7/8 threshold shown)

% Unanswered calls

Answered Rate

Average Speed of Answer (ASA)

ASA Growth metrics

ASA Performance Management indicators

Call Duration Metrics:

Average Talk Duration

Converted duration metrics

Duration Growth percentages

Performance Management duration metrics

Duration trend indicators

Volume Metrics:

Total Calls volume

Calls Growth percentages

Calls growth direction indicators

Maximum and Minimum call values

**3. Dimensional Model**

The data model follows a star schema design:

Fact Table: Call records with timestamps, agent IDs, and performance metrics

Dimension Tables:

Date dimension for temporal analysis

Agent dimension for performance tracking

Department dimension for organizational analysis

Time dimension (hour/minute) for intra-day analysis

# Key Features

**1. Agent Performance Tracking**

Individual agent answer rates and performance

Visual agent identification with photos

Comprehensive contact information

Department-based grouping

**2. Temporal Analysis**

Daily, weekly, and monthly performance trends

Hourly and minute-level granularity for intra-day analysis

Weekday patterns and seasonal trends

Growth metrics for performance tracking

**3. Operational Efficiency Metrics**

Call answer efficiency measurements

Talk duration optimization

Speed of answer benchmarks

Performance management indicators

# Data Processing and Transformation

**ETL Processes Implemented:**

_Data Integration:_ Combined call records, agent information, and temporal data

_Metric Calculation:_ Created complex performance indicators including:

Growth percentages

Converted duration metrics

Performance management benchmarks

_Data Hierarchy Creation:_ Built date and time hierarchies for drill-down analysis

_Relationship Establishment:_ Connected fact tables with dimension tables

**Data Quality Measures:**

Implemented collapse/expand functionality for data navigation

Created sign indicators for growth trends (positive/negative)

Established min/max value tracking for outlier detection

# Dashboard Components

**Page 1:** Operational Overview
Summary metrics and KPIs

High-level performance indicators

Trend analysis and growth metrics

**Page 2:** Detailed Analysis
Agent-level performance details

Department-wise breakdown

Temporal analysis with drill-down capabilities

Comparative performance metrics

# How to Use the Dashboard

Monitor Daily Performance: Use the calendar dimension to track daily metrics

Analyze Agent Efficiency: Review individual agent performance through answer rates and talk duration

Identify Trends: Use growth metrics to identify improving or declining performance areas

Optimize Staffing: Use hourly/minute data to optimize shift planning

Department Comparison: Compare performance across different departments

# Potential Applications

Real-time performance monitoring

Historical trend analysis

Agent performance evaluation and coaching

Operational efficiency optimization

Resource allocation and staffing planning

Service level agreement (SLA) compliance tracking

# Technical Implementation

**Data Modeling:** Star schema design with conformed dimensions

**Metric Calculation:** DAX or similar language for complex metrics

Visualization: Interactive dashboard with drill-through capabilities

Data Refresh: Scheduled updates for current performance monitoring
