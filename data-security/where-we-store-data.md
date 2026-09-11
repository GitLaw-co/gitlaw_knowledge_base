---
title: Where we store data
slug: where-we-store-data
category: data-security
excerpt: Our data storage and processing infrastructure is designed to ensure the security, privacy, and efficiency of your data.
---

**Data Storage Locations**

Our data storage and processing infrastructure is designed to ensure the security, privacy, and efficiency of your data. Here's a detailed overview of where and how we store and manage data:

1.  Primary Data Storage:
    - Google Servers (Belgium, EU): The majority of our data is securely stored on Google servers located in Belgium. This ensures compliance with EU data protection regulations and provides robust security measures.
2.  Databases:
    - PostgreSQL: Some of our structured data is stored in PostgreSQL databases. PostgreSQL is a powerful, open-source object-relational database system known for its reliability and performance.
    - Elasticsearch: For enhanced search capabilities and real-time data analytics, we utilize Elasticsearch. This allows us to quickly retrieve large volumes of data.
3.  Analytics and Monitoring:
    - Segment: We use Segment to manage and route analytics data to various destinations. This helps us gain insights into user interactions and improve our services.
    - Sentry: Some tracing and error monitoring data are sent to Sentry. This allows us to detect and resolve issues in our applications swiftly.
4.  Third-Party Integrations:
    - AI providers: For AI features we send document content to Anthropic, OpenAI, and Google to carry out the specific task you requested. See [GitLaw Subprocessors](/knowledge-base/gitlaw-subprocessors) for the full list of processors.
