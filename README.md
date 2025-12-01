# Snowflake Intelligence Demo - Snowmobile Telco

This project demonstrates the comprehensive Snowflake Intelligence capabilities for **Snowmobile Telco**, the UK's leading B2B communications provider, including:
- **Cortex Analyst** (Text-to-SQL via semantic views)
- **Cortex Search** (Vector search for unstructured documents)  
- **Snowflake Intelligence Agent** (Multi-tool AI agent with orchestration)
- **Git Integration** (Automated data loading from GitHub repository)

## About Snowmobile Telco

Snowmobile Telco is a UK-based B2B communications provider specialising in:
- **UCaaS** (Unified Communications): Horizon, Microsoft Teams Phone, Webex, CircleLoop
- **CCaaS** (Contact Centre): Horizon Contact, Cirrus, Amazon Connect Managed
- **Voice Services**: SIP Trunking, Inbound, Phoneline+
- **Connectivity**: Business Broadband, Ethernet, SD-WAN
- **Security**: Snowmobile Secure (MDR, SOC, Security Awareness)

**Key Facts:**
- ~£500M annual revenue
- 858,000+ UCaaS seats deployed
- 168,000+ mobile subscribers
- 128,000+ IoT connections
- 88% 5G population coverage
- 1,050+ active channel partners
- Operations in UK, Netherlands, Spain, Germany
- AIM listed (moving to Main Market May 2025)

## Key Components

### 1. Data Infrastructure
- **Star Schema Design**: 16 dimension tables and 6 fact tables covering Finance, Sales, Marketing, HR, Mobile, and Network
- **Mobile & 5G Data**: Network coverage, tariffs, devices, KPIs, and subscriber metrics
- **B2B Customer Model**: 1,000 business customers across SMB, Enterprise, Public Sector, and Partner segments
- **Channel Partner Focus**: Sales through channel partners with customer vertical segmentation
- **Realistic Sample Data**: B2B sales transactions with industry and regional breakdowns
- **Database**: `SNOWMOBILE_AI_DEMO` with schema `SNOWMOBILE_SCHEMA`
- **Warehouse**: `Snowmobile_Demo_WH` (XSMALL with auto-suspend/resume)

### 2. Semantic Views (5 Business Domains)
- **Finance Semantic View**: Revenue by product, partner economics, unit economics
- **Sales Semantic View**: Partner performance, seat growth, deal pipeline
- **Marketing Semantic View**: Campaign ROI, partner marketing, competitive intelligence
- **HR Semantic View**: Employee data, departments, certification tracking
- **Network Semantic View**: 5G/4G coverage, mobile tariffs, devices, network KPIs, subscriber metrics

### 3. Cortex Search Services (7 Domain-Specific)
- **Finance Documents**: Financial reports, vendor contracts (Microsoft, Cisco, AWS), ESG reports
- **HR Documents**: Employee handbook, performance guidelines, department overviews
- **Marketing Documents**: Campaign strategies, competitive analysis, NPS reports
- **Sales Documents**: Channel partner playbooks, retention strategies, customer success
- **Strategy Documents**: Market position, investor relations, board presentations
- **Network Infrastructure**: 4G/5G coverage, mobile network strategy, IoT solutions, fibre broadband, eSIM, roaming
- **Demo Scripts**: CEO/CFO/CMO demo scripts and presentations

### 4. Snowflake Intelligence Agent
- **Multi-Tool Agent**: Combines Cortex Search, Cortex Analyst, Web Scraping, and File Access capabilities
- **Cross-Domain Analysis**: Can query all business domains and documents
- **Partner-Focused Insights**: Revenue attribution, partner performance, channel analytics
- **Natural Language Interface**: Responds to business questions across all departments
- **Visualization Support**: Generates charts and visualizations for data insights

## Demo Script: Snowmobile Telco C-Level Executive Demo

This demo is tailored for **Snowmobile Telco** C-level executives (CEO, CFO, CMO, CCO). All data uses **British Pounds (£)**, **UK regions**, and references **B2B communications competitors** (8x8, RingCentral, Mitel, Vonage).

### Key Metrics Reference
| Metric | Value |
|--------|-------|
| Annual Revenue | £500 million |
| Q4 Revenue | £132 million |
| UCaaS Seats | 858,000 |
| Teams Phone Seats | 82,000 |
| Mobile Subscribers | 168,000 |
| IoT Connections | 128,000 |
| 5G Population Coverage | 88% |
| 4G Population Coverage | 99.5% |
| 5G Download Speed | 320 Mbps avg |
| Mobile ARPU | £21.20 |
| eSIM Adoption | 48% |
| Active Partners | 1,050 |
| Customer NPS | +45 |
| Partner NPS | +52 |
| Monthly Churn | 0.95% |
| EBITDA Margin | 22% |
| LTV:CAC | 6.2x |

---

### 👔 CEO: Strategic Overview
1. **Business Health** *(Documents)*  
   "Give me an executive summary of our H1 2025 performance."

2. **Market Position** *(Documents)*  
   "How are we positioned against 8x8, RingCentral, and Mitel?"

3. **Microsoft Teams** *(Documents)*  
   "What's our progress on Microsoft Teams Phone?"

4. **Competitive Threats** *(Documents)*  
   "What opportunities does 8x8's strategic review create for us?"

5. **Revenue by Region** *(Structured Data)*  
   "What is our total revenue by UK region?"

---

### 💰 CFO: Financial Performance
1. **Revenue Analysis** *(Structured Data)*  
   "What is our revenue breakdown by product category?"

2. **Unit Economics** *(Documents)*  
   "What is our customer lifetime value and acquisition cost?"

3. **Revenue by Industry** *(Structured Data)*  
   "Show me revenue breakdown by customer industry."

4. **Revenue by Vertical** *(Structured Data)*  
   "What is revenue by customer vertical - SMB, Enterprise, Public Sector?"

5. **Vendor Spend** *(Structured Data + Documents)*  
   "Show me vendor spend breakdown by Ericsson, Nokia, Apple, and Samsung"

---

### 📢 CMO: Partner Marketing & Customer
1. **Campaign Performance** *(Documents)*  
   "Which marketing campaigns delivered the best ROI in 2024?"

2. **Customer Satisfaction** *(Documents)*  
   "What is our NPS and how do we compare to competitors?"

3. **Campaign Leads** *(Structured Data)*  
   "Which campaigns generated the most leads?"

4. **Competitive Intelligence** *(Documents)*  
   "What are the key competitive threats from 8x8 and RingCentral?"

5. **Channel Performance** *(Structured Data)*  
   "Which marketing channels generated the most leads and impressions?"

---

### ⚙️ CCO: Channel & Operations
1. **Top Products** *(Structured Data)*  
   "What are our top selling products by revenue?"

2. **Churn Analysis** *(Documents)*  
   "What is our monthly churn rate and what are the main drivers?"

3. **Seat Growth** *(Documents)*  
   "What is our UCaaS seat growth by product?"

4. **Sales by Region** *(Structured Data)*  
   "Which UK regions have the highest sales?"

5. **Customer Industries** *(Structured Data)*  
   "Which industries generate the most revenue?"

---

### 🔗 Cross-Functional Insights
1. **Product by Segment** *(Structured Data)*  
   "Which products sell best to Enterprise vs SMB customers?"

2. **Campaign Attribution** *(Structured Data)*  
   "Which campaigns generated the most opportunities?"

3. **Top Customers** *(Structured Data)*  
   "Who are our top 10 customers by revenue?"

4. **Sales Rep Performance** *(Structured Data)*  
   "Which sales reps have the highest revenue?"

5. **Product Category Trends** *(Structured Data)*  
   "How does revenue compare across Snowmobile Elements categories?"

---

### 📄 Document Search (Strategy & Compliance)
1. **Investor Relations**  
   "What does our investor relations FAQ say about dividend policy?"

2. **Regulatory Compliance**  
   "What are our Ofcom compliance obligations for One Touch Switch?"

3. **Partner Agreements**  
   "What are the key terms of our Microsoft partnership?"

4. **ESG Commitments**  
   "What are our sustainability targets and progress?"

5. **Competitive Strategy**  
   "What is our strategic response to 8x8's challenges?"

---

### 🌐 Network Infrastructure (CTO/CIO)
1. **Network Uptime**  
   "What is our network uptime and platform reliability?"

2. **5G Coverage Analysis**  
   "What is our 5G coverage by UK region and how do we compare to EE and Vodafone?"

3. **Mobile Network Performance**  
   "What are our average 5G download speeds and latency?"

4. **IoT Connectivity**  
   "How many IoT connections do we have and what are the main use cases?"

5. **Infrastructure Overview**  
   "Where are our data centres located and what's their capacity?"

---

### 📱 Mobile & 5G (CTO/CMO)
1. **Mobile Subscriber Growth**  
   "What is our mobile subscriber count and growth trend?"

2. **5G Rollout Progress**  
   "What is our 5G rollout status by region?"

3. **Device Portfolio**  
   "What devices do we offer - iPhone 16, Samsung Galaxy S25, Pixel 9?"

4. **Mobile Tariffs**  
   "What business mobile plans do we offer and what are the prices?"

5. **eSIM Adoption**  
   "What is our eSIM adoption rate and which devices support it?"

---

### 📋 Demo Flow Recommendation for C-Suite

1. **CEO Opening** (5 min): Strategic documents, competitive position, market analysis
2. **CFO Deep Dive** (5 min): Revenue by product/industry/region, vendor contracts
3. **CMO Analysis** (5 min): Campaign performance, NPS reports, competitive intelligence
4. **CCO Operations** (5 min): Top products, regional sales, industry breakdown
5. **CTO/CIO Infrastructure** (5 min): Network uptime, 5G coverage, mobile performance
6. **Mobile & 5G** (5 min): Subscriber growth, device portfolio, eSIM adoption, IoT
7. **Cross-Functional** (5 min): Product-segment analysis, campaign attribution, top customers
8. **Document Search** (5 min): Investor relations, compliance, ESG commitments

This progression showcases how Snowmobile Telco executives can access strategic insights across all business domains through natural language queries, combining structured data analysis with unstructured document search for comprehensive decision support.

## Snowmobile Elements Product Portfolio

| Category | Products |
|----------|----------|
| **Snowmobile Connect** | Horizon, Teams Phone, Webex, CircleLoop, iPECS |
| **Snowmobile Experience** | Horizon Contact, Cirrus, Amazon Connect Managed |
| **Snowmobile Enable** | SIP Trunks, Inbound, Phoneline+, FUSION IoT |
| **Snowmobile Secure** | MDR, SOC, SafeWeb, Vulnerability Management |
| **Snowmobile Solutions** | Managed Networks, Enterprise Solutions, SnowmobileUCX |
| **Mobile Business Plans** | Business Essential SIMs, Enterprise SIMs, Pooled Data |
| **5G Enterprise** | 5G Business Plans, Private 5G, Network Slicing |
| **IoT & M2M** | IoT SIMs, Fleet Trackers, Smart Meters, CCTV |
| **Mobile Devices** | iPhone 16 series, Samsung Galaxy S25 series, Google Pixel 9 series, iPads, Tablets |
| **Fibre Broadband** | FTTP, Ethernet, Dedicated Lines |
| **Connectivity** | Business Broadband, SD-WAN, 4G/5G Backup |

## Competitors Referenced

| Competitor | Type | Key Positioning |
|------------|------|-----------------|
| **8x8** | UCaaS/CCaaS | XCaaS platform, financial challenges |
| **RingCentral** | UCaaS | Enterprise focus, channel conflict |
| **Mitel** | UCaaS/On-Prem | Legacy transition, cloud challenges |
| **Vonage** | CPaaS | API focus, Ericsson owned |
| **Microsoft Direct** | Voice | Teams Phone calling plans |

## Setup Instructions

**Single Script Setup**: The entire demo environment is created with one script:

1. **Run the complete setup script**:
   - Copy the contents of `sql_scripts/demo_setup.sql`
   - Execute in a Snowflake worksheet

2. **Post-Setup Verification**:
   - Run `SHOW TABLES IN SNOWMOBILE_AI_DEMO.SNOWMOBILE_SCHEMA;` to verify 25 tables created
   - Run `SHOW SEMANTIC VIEWS;` to verify 5 semantic views (Finance, Sales, Marketing, HR, Network)
   - Run `SHOW CORTEX SEARCH SERVICES;` to verify 7 search services

3. **Access the Agent**:
   - Navigate to Snowflake Intelligence
   - Select `Snowmobile_Executive_Agent` from agents list

---

## 📝 Complete List of Sample Prompts

### Sales & Revenue Analysis
| Prompt | Data Source |
|--------|-------------|
| "What is our total revenue by customer industry?" | Structured Data |
| "What are our top selling products by revenue?" | Structured Data |
| "Which UK regions have the highest sales?" | Structured Data |
| "Who are our top 10 customers by revenue?" | Structured Data |
| "What is revenue by customer vertical - SMB, Enterprise, Public Sector?" | Structured Data |
| "Which products sell best to Enterprise vs SMB customers?" | Structured Data |
| "Which sales reps have the highest revenue?" | Structured Data |

### Financial Analysis
| Prompt | Data Source |
|--------|-------------|
| "What is our revenue breakdown by product category?" | Structured Data |
| "Show me revenue breakdown by customer industry." | Structured Data |
| "How does revenue compare across Snowmobile Elements categories?" | Structured Data |
| "What is our customer lifetime value and acquisition cost?" | Documents |
| "Show me vendor spend breakdown by Ericsson, Nokia, Apple, and Samsung" | Structured Data |
| "What are our network equipment costs vs device procurement costs?" | Structured Data |
| "What are our key commitments with Microsoft, Cisco, and AWS?" | Documents |

### Marketing Campaign Analysis
| Prompt | Data Source |
|--------|-------------|
| "Which marketing campaigns delivered the best ROI in 2024?" | Documents |
| "Which campaigns generated the most leads?" | Structured Data |
| "Which marketing channels generated the most leads and impressions?" | Structured Data |
| "Which campaigns generated the most opportunities?" | Structured Data |
| "What is our NPS and how do we compare to competitors?" | Documents |

### HR & Workforce Analysis
| Prompt | Data Source |
|--------|-------------|
| "What is our employee count by department?" | Structured Data |
| "Show me the department structure and headcount." | Structured Data |
| "What are the performance review guidelines?" | Documents |

### Strategic Documents & Competitive Intelligence
| Prompt | Data Source |
|--------|-------------|
| "How are we positioned against 8x8, RingCentral, and Mitel?" | Documents |
| "What opportunities does 8x8's strategic review create for us?" | Documents |
| "What's our progress on Microsoft Teams Phone?" | Documents |
| "Give me an executive summary of our H1 2025 performance." | Documents |
| "What is our strategic response to 8x8's challenges?" | Documents |
| "What are the key competitive threats from 8x8 and RingCentral?" | Documents |

### Network Infrastructure & Mobile
| Prompt | Data Source |
|--------|-------------|
| "What is our network uptime and platform reliability?" | Documents |
| "What is our 5G coverage by UK region?" | Structured Data + Documents |
| "What are our average 5G and 4G download speeds?" | Structured Data |
| "How do we compare to EE, Vodafone, and Three on 5G coverage?" | Documents |
| "What is our mobile subscriber count and ARPU?" | Structured Data |
| "What mobile business plans do we offer and at what price points?" | Structured Data |
| "What are our IoT connectivity solutions and how many connections?" | Documents |
| "What is our mobile network strategy for 2025?" | Documents |
| "What devices do we support - iPhone 16, Galaxy S25, Pixel 9?" | Structured Data + Documents |
| "What is our eSIM adoption rate?" | Documents |
| "What IoT/M2M tariffs do we offer?" | Structured Data |
| "What is our network performance by region - latency, speed?" | Structured Data |

### Regulatory & Compliance
| Prompt | Data Source |
|--------|-------------|
| "What are our Ofcom compliance obligations for One Touch Switch?" | Documents |
| "What are our sustainability targets and progress?" | Documents |
| "What does our investor relations FAQ say about dividend policy?" | Documents |
| "What are the key terms of our Microsoft partnership?" | Documents |

### Vendor Spend Analysis (Mobile/Telco)
| Prompt | Data Source |
|--------|-------------|
| "Show me vendor spend breakdown by Ericsson, Nokia, Apple, and Samsung" | Structured Data |
| "What are our network equipment costs vs device procurement costs?" | Structured Data |
| "What is our spend with mobile network partners (EE, Three, O2)?" | Structured Data |
| "What are our IoT hardware costs with Cradlepoint and Teltonika?" | Structured Data |
| "Show me device procurement spend by Apple vs Samsung" | Structured Data |
| "What is our total spend on network infrastructure vendors?" | Structured Data |

### Churn & Retention
| Prompt | Data Source |
|--------|-------------|
| "What is our monthly churn rate and what are the main drivers?" | Documents |
| "What is our UCaaS seat growth by product?" | Documents |

---

## 🚫 Questions the Agent Will NOT Answer

The agent has guardrails and will politely decline questions unrelated to Snowmobile Telco business data:

| Off-Topic Question | Agent Response |
|-------------------|----------------|
| "What time is it?" | Redirects to business questions |
| "Who is the prime minister?" | Redirects to business questions |
| "Tell me a joke" | Redirects to business questions |
| "What's the weather?" | Redirects to business questions |

The agent will respond: *"I can only help with questions about Snowmobile Telco business data. For example, you could ask about sales performance, revenue by product, network uptime, or competitive analysis."*
