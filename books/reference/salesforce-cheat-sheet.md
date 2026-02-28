# Salesforce Cheat Sheet

**Author:** Weflow  
**Format:** PDF  
**Category:** reference

---

## Page 1

Object Description Key Fields Relationships
Account Represents a business or individual customer account in
Salesforce.
Account Name, Industry,
Type, URL
Related to Contacts, Opportunities, and
Cases
Contact An individual associated with an Account, often representing a
customer or a business contact. First Name, Last Name, Email Linked to Account, Opportunities, and
Cases
Opportunity Tracks sales deals and revenue potential for an Account. Opportunity Name, Stage,
Amount, Close Date
Connected to Account and Contacts (via
Contact Roles)
Lead Represents a potential prospect or opportunity that has not yet
been qualified.
Lead Source, Status,
Company
Can be converted into an Account,
Contact, and Opportunity
Case Manages customer inquiries and support issues. Case Number, Status, Priority Related to Account and Contact
Campaign Tracks marketing campaigns aimed at Leads and Contacts. Campaign Name, Budget,
Start Date Linked to Leads and Contacts
Product Catalogs items that a business sells; often associated with
Opportunities through Price Books.
Product Name, Product Code,
Price
Related to Opportunity through
OpportunityLineItem
Price Book Defines different pricing structures for Products that can be
used in various Opportunities. Price Book Name Related to Products and
OpportunityLineItems
Quote Represents a proposal to a customer including Products, Price,
and Terms. Quote Name, Total Amount Related to Opportunities
Task & Event Tracks tasks, calls, emails, and meetings, providing activity
history for Accounts, Contacts, Leads, and Opportunities. Task Name, Due Date, Status Related to multiple objects like Account,
Contact, Opportunity, etc.
Order Manages finalized sales and product shipments. Order Number, Status Related to Account, Opportunity, and
Quote
Asset Tracks items that customers have purchased, including status
and maintenance. Asset Name, Serial Number Linked to Account and Contact
Contract Contains terms and conditions of a customer’s agreement with
the business. Contract Start Date, Status Related to Account and Opportunities
Custom Objects Allows users to create unique objects to fit specific business
needs beyond standard Salesforce objects.
Custom fields per business
need
Can have custom relationships as
needed
Salesforce Overview
Industry: #1 CRM (21.7% market share, competitors: Microsoft, Oracle, SAP, Hubspot)
FY24 Revenue: $34.9 Billion @ non-GAAP Operating Margin of 30.5%
Market Cap (Oct 6, 2024): $284 Billion (world's 40 most valuable companies)
Number of customers: 150,000 (Notable: Amazon Web Services, Spotify, and T-Mobile)
Number of employees: 72,682 (51% in the US)
Enterprise and Departmental Custom Applications
Appexchange Business Partner Packages
Sales Services Services Commerce
Community IOT Analytics Einstein
Capability Area Description Key Actions
User Management Manage user accounts, permissions, roles, and access
settings. Create/edit users, assign profiles, set roles, enable MFA.
Data Management Import, export, and maintain data integrity within Salesforce. Use Data Loader, import wizard, manage duplicate rules.
Security Settings Configure security settings to protect data and ensure
compliance.
Field-level security, encryption, session settings, IP
restrictions.
Customization Configure Salesforce to meet business requirements by
creating custom objects, fields, and relationships.
Add custom objects/fields, set up record types, configure
page layouts.
Automation Streamline business processes through automation tools. Set up Flows, Process Builder, Workflow Rules, Approval
Processes.
Reporting and Analytics Generate insights with reports and dashboards, providing
valuable data analysis and visualization tools for users. Create reports/dashboards, configure scheduled reports.
App Management Manage and integrate third-party applications and tools via
AppExchange. Install/uninstall apps, configure AppExchange packages.
Change and Release
Management
Test and deploy new changes within different Salesforce
environments to ensure stability and manage releases
effectively.
Use Sandboxes, Change Sets, track release notes.
System Health and
Performance
Monitor and optimize Salesforce performance and manage
platform health checks.
Enable debug logs, use Health Check, and view system
status.
Mobile Configuration Configure Salesforce Mobile App settings to ensure the
mobile experience aligns with business needs.
Customize navigation, set mobile-specific layouts, enable
offline access.
Documentation and Training
Provide support and resources for end-users, document
processes, and ensure compliance with training
requirements.
Create training materials, configure in-app guidance.
Name Date Amount Category Current Name
Slack Dec 2020 $27.7B Collaboration Slack
Tableau Jun 2019 $15.7B Analytics Tableau, part of Customer 360
Mulesoft Mar 2018 $6.5B Integration MuleSoft Anypoint Platform
ExactTarget Jun 2013 $2.5B Marketing Automation Marketing Cloud (with Pardot)
Demandware Jun 2016 $2.8B E-commerce Commerce Cloud
ClickSoftware Aug 2019 $1.35B Field Service Management Field Service Lightning
Vlocity Feb 2020 $1.33B Industry-Specific CRM Salesforce Industries
Heroku Dec 2010 $212M Cloud Platform (PaaS) Heroku
Krux Oct 2016 $800M Data Management Platform Salesforce DMP
Datorama Jul 2018 $800M Marketing Analytics Marketing Cloud Intelligence
Quip Aug 2016 $750M Collaboration Quip
Buddy Media Jun 2012 $745M Social Media Marketing Social Studio
Acumen Solutions Jan 2021 N/A Cloud Consulting Salesforce Professional Services
Salesforce Lightning Architecture
Salesforce Careers & Education
Events Certificates
Dreamforce (San Francisco, USA)
Salesforce's flagship event, held annually in San Francisco.
Focus: Product launches, keynotes from Salesforce executives, expert-
led sessions, and networking opportunities.
Salesforce World Tour
Takes Dreamforce content to major cities worldwide, allowing more
people to attend closer to home.
Cities: New York, London, Sydney, Paris, Tokyo, Amsterdam, and more.
TrailblazerDX (San Francisco, USA)
Previously called TrailheaDX, this developer-focused event takes place
annually in San Francisco.
Focus: Designed for developers, architects, and admins, with an
emphasis on technical training, product updates, and innovations.
Highlights: Hands-on sessions, certifications, and workshops centered
on Salesforce development and customization.
Salesforce Connections (Chicago, USA)
Premier digital marketing and commerce conference, typically held in
Chicago.
Focus: Marketing Cloud, Commerce Cloud, and related solutions.
Salesforce Basecamp (Regional)
Smaller regional events called "Basecamp" take place in cities across
the globe, providing more localized Salesforce content and networking
opportunities.
Focus: Salesforce solutions tailored to regional businesses, with
workshops and product demos.
Dreamforce to You (Virtual)
A virtual extension of Dreamforce, designed for those who can’t attend
in person.
Highlights: Global accessibility and recorded sessions, which
participants can view on-demand.
Salesforce Cheat Sheet
Salesforce Producs Salesforce Industries
Salesforce Top 10 Implementation Partners Globally
Salesforce Data Model
Salesforce Administrator Certifications
Salesforce Architect Certifications
Data Architecture and Management Designer
Sharing and Visibility Designer
Development Lifecycle and Deployment Designer
Identity and Access Management Designer
Integration Architecture Designer
Heroku Architecture Designer
Salesforce Consultant Certifications
Specialize in Sales, Service, Field Services, etc.
Salesforce Developer Certifications
Salesforce Certified Platform Developer I
Salesforce Certified Platform Developer II
Salesforce Certified B2C Commerce Developer
Salesforce Certified Industries CPQ Developer
Salesforce Marketing Cloud Certifications
Salesforce Designer Certifications
 Salesforce Product-Specific Certifications
CPQ, Pardot, Tableau, etc.
Salesforce Business Analyst Certification
Salesforce Industries Certifications
Learn
 Salesforce Trailhead
Salesforce's free, interactive learning platform. It offers modules, projects, and trails
that cover everything from basic to advanced Salesforce skills.You can sign up for free
at Trailhead.
Salesforce Certification Paths
Earning Salesforce certifications is one of the best ways to demonstrate your expertise
to potential employers. Start with the Salesforce Certified Administrator or Platform
Developer I for foundational knowledge.
Salesforce Courses on Online Learning Platforms
Sites like Udemy, Pluralsight, LinkedIn Learning, and Coursera offer Salesforce courses.
These courses often include video tutorials, quizzes, and projects.
Hands-On Practice with a Salesforce Developer Org
Salesforce offers free Developer Edition accounts with access to nearly all Salesforce
features. Sign up for a free developer account at Salesforce Developers.
Salesforce Documentation and Release Notes
Salesforce has detailed documentation and release notes for each major update.
Comprehensive source for technical details and new feature updates. Explore the
documentation at Salesforce Help & Training.
Salesforce Community and Forums
Salesforce Trailblazer Community, Stack Exchange, Reddit, and LinkedIn groups. Join
the Trailblazer Community and search for groups based on your role or interest.
YouTube Channels and Blogs
Popular YouTube Channels: Salesforce Ben, SFDC99, and Salesforce Apex Hours offer
tutorials, tips, and insights.
Blogs: Sites like Salesforce Ben, Admin Hero, and Jitendra Zaa cover a variety of
Salesforce topics, including coding tutorials, feature updates, and certification tips.
Salesforce Partner and Training Programs
Research reputable Salesforce training partners or visit the Salesforce Training section
on Trailhead Academy
Instantly available declarative no-code/ low-code application microservices
Instantly available core configurable (no-code) enterprise microservices
Salesforce.trust.com technical foundation
Einstein Application
Microservices
Application Tooling
Data Model
Standard Objects
Custom Objects
External Objects
Immutable Objects
Automations
Rules/ Constraints 
Instant/ Time-basd Headless Worksflows
GUI Driven Dynamic Workflows
Approvals/ Escalations
APEX Triggers
Reporting
UX
Lightening UI Design Framework
Lightening UI Components
Client-side Dynamic UI Framework
Mobile SDK
Reports/ Dashboards/ Analytics
Processing
Deep Learning
Sentiment & Intent Reasoning
Vision & Voice Processing
Machine Learning
Scoring
Recommendations Processing
Preidctions & Propensity Models
Forecasting
Declarative No-Code Einstein Tooling
Prediction Builder
Bots
Declarative No-Code Tooling
Setup UI
Reporting/ Dashboard Buiklder
Schema Builder
Programmatic Low-Code
Developer Console
Force.com IDE
Workbench
ANT Migration Tool
Salesfroce DX
Security
User Identify/ SSO / GeoFencing 
Multi-factor Authentifcation
User Profiles/ Permissions
Object/ Role/ Field Security
Ownerhip/ Sharing Rules
Authority Delegations
Internationalization
Multi-currency/ Conversions
Translation
Locale Specific Notations
Mobility
iOS/ Android Applications
Configurable Mobile Extensibility
Custom Branding
Disconnected Access
Callaboration
Omni-channel Alerts/ Notifications
Email Integrations
Calendars/ Events/ Tasks/ Activities
Teams/ Groups/ Queues
Knowledge Base
Communities/ Groups
Compliance & Forensics
Encryption
Field-level Audit Trail
User Activity Monitoring
Events
Core Global Multi-Tenant/ MetaData Infrastructure, HA/DR, Governance, Performance and Security Operations, International Security and Privacy Compliance
API First / Instantly Mobile
Salesforce Admin Features
Salesforce Acquisitions
Revenue Intelligence powered by AI 
   
 A c t i v i t y  C a p t u r e    P i p e l i n e  M a n a g e m e n t   
 C o n v e r s a t i o n  I n t e l l i g e n c e    S a l e s  F o r e c a s t i n g
