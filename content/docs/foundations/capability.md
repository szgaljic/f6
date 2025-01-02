---
title: Capability
weight: 2
---

## Overview

_Ensuring technology delivers its intended purpose with excellence._

At its core, software exists to solve problems, meet needs, and deliver value to users and stakeholders. **Capability represents the foundation of functionality**—the workflows, features, and solutions that define the software’s purpose. 

The Capability foundation emphasizes delivering the right functionality, at the right time, to the right users. It's about carefully considering the purpose of the software and prioritizing it's feature sets. Capability also underscores the importance of intentionality. Adding unnecessary features or poorly implementing required ones can dilute focus, introduce technical debt, and create frustration for users. 

## What is Capability?

**Capability** is captured through in-depth discussions where stakeholders describe their needs, and the implementation team translates these into functional and non-functional requirements. 

**Functional requirements** define the specific behaviors, features, or workflows the system must deliver to meet user and business needs, as distinct from **Non-Functional requirements**, which address performance, scalability, or other operational characteristics.

The process typically involves capturing the current state, defining the desired future state, and identifying the gaps between the two. These gaps represent the project scope. While this is a standard industry practice, the F6 Framework enhances it by applying **Capability Mapping** to clearly correlate requirements into business needs.

{{% callout note %}}
A detailed guidance on conducting holiistic discovery sessions is covered in [F6 Discovery Process](/docs/f6-discovery/).
{{% /callout %}}

### Examples of Capability

Capability can be described in several ways. Here are a few high-level examples:

- **Core Workflow Efficiency:** A fintech platform may prioritize seamless transaction flows, such as enabling one-click payment for customers while ensuring real-time fraud checks in the background. This capability streamlines user experience while maintaining robust security.

- **Regulatory Compliance Enablement:** A healthcare application must integrate features that ensure compliance with HIPAA, such as audit trails, secure data sharing, and patient consent management. These capabilities are foundational to operating in a regulated industry.

- **Scalability for Growth:** An e-commerce site designed for a small customer base must be capable of scaling to handle seasonal spikes, like Black Friday traffic, with features such as dynamic resource allocation and robust caching mechanisms.

## Capability Mapping

Central to the Capability foundation is **Capability Mapping**. It provides a structured approach to align business goals with technical execution by creating clear mappings between high-level objectives and implementation strategies. 

This process focuses on mapping and alignment. It does not directly address trade-offs, project planning, or risk evaluation, which are covered in other aspects of the F6.

The steps are as follows:

1. **Business to Product:** TBD.
2. **Product to Technical:** TBD.
3. **Implementation:** TBD.

### Business to Product

Every solution starts with trying to understand its purpose and the problems it aims to solve. For illustration, we will use a **FinTech payment processing system** as an example to show how business goals translate into technical execution.

We start by identifying **business needs**—the core drivers of value for the organization and its users. Imagine the stakeholders gathered in a strategy meeting, discussing their goals for the new platform. Their conversations might sound like this:

- _"We need to proactively detect and prevent fraudulent transactions to protect our customers and our reputation."_
- _"Compliance with financial regulations like AML and KYC is non-negotiable."_
- _"Our platform must handle thousands of transactions per second and support customers across multiple regions."_
- _"Customers expect a seamless checkout experience, whether they’re on desktop or mobile."_
- _"We want to reduce revenue loss by optimizing transaction retries and routing payments efficiently."_
- _"Cost efficiency is key; we need to monitor and optimize our processing fees."_
- _"Data security is paramount; sensitive payment information must be protected at all costs."_
- _"Instant payment confirmations and real-time updates are table stakes in today’s competitive landscape."_
- _"We need our system to integrate seamlessly with financial institutions worldwide."_

We can distill these statements down, and then map them into specific **Product Requirements**—the user-facing features and workflows required to fulfill those needs. These requirements provide a blueprint for what the platform must deliver to achieve its goals.

| **Business Need**           | **Product Requirements**                                                                 |
|------------------------------|-----------------------------------------------------------------------------------------|
| Payment Processing           | Payment gateway integrations |
| Regulatory Compliance        | AML/KYC verification, Audit trails, Transaction reporting, Data retention policies       |
| Scalability                  | High-volume transaction processing, Multi-region support, Dynamic resource allocation     |
| Customer Retention           | Seamless checkout experience, Personalized recommendations, Multi-payment options         |
| Revenue Optimization         | Transaction retries, Smart routing, Revenue leakage reports, Audit trails, Transaction reporting |
| Cost Efficiency              | Optimized processing fees, Batch processing for settlements, Infrastructure cost monitoring |
| Data Security and Privacy    | Encryption of sensitive data, Tokenization of payment information, Consent management     |
| Real-Time Processing         | Instant payment confirmations, Real-time transaction updates, Push notifications         |
| Interoperability             | Integration with financial institutions, Open API ecosystem, Cross-border payment capabilities |

For example, "Fraud Prevention and Detection" translates into a set of tools and techniques that proactively identify and mitigate risks. The emphasis here is on capturing the "what" without diving into specific tools or solutions.

It’s common for product requirements to overlap so we can refine them down into **Product Themes**—groups of related features or workflows that represent a cohesive area of functionality. 

| Product Theme        | Product Requirements                                              |
|----------------------|-------------------------------------------------------------------|
| Multiple Payment gateway | Payment gateway integrations, Smart routing |
| Fraud Detection      | Fraud monitoring, Transaction risk scoring, Alerts and notifications |
| Advanced User Experience      | Seamless checkout interface, Multi-payment options, Instant payment confirmations |
| Real-Time Processing         | Instant payment confirmations, Real-time transaction updates, Push notifications         |
| Real-Time Processing         | Instant payment confirmations, Real-time transaction updates, Push notifications         |
| Scalability          | High-volume transaction processing, Multi-region support, Dynamic resource allocation |
| Compliance           | AML/KYC verification, Audit trails, Transaction reporting        |
| Cost Optimization    | Transaction retry mechanisms, Smart routing, Optimized processing |


### Product to Technical

Once product requirements are established, the next step is translating them into Technical Requirements. This step ensures captures that each product feature or workflow is backed by a defined set of technical specifications that can be implemented by engineers.

The process begins by organizing Product Requirements into Product Themes—groups of related features or workflows that represent a cohesive area of functionality. Product Themes allow for better prioritization and help identify synergies or overlaps among requirements.

| **Product Theme**           | **Product Requirements**                                                          |
|------------------------------|-----------------------------------------------------------------------------------------|
|  |  |
|  |  |
|  |  |

ChatGPT: Write a narrative, then take those Product themes and map into Technical Requirements.

| **Product Theme**           | **Technical Requirements**                                                          |
|------------------------------|-----------------------------------------------------------------------------------------|
|  |  |
|  |  |
|  |  |

### Technical to Implementation

| **Technical Requirement**                      | **Implementation**                        | **Tools & Products**                                                        |
|------------------------------------------------|-------------------------------------------|-----------------------------------------------------------------------------|
| Fraud monitoring                                | Real-time fraud detection system          | AWS Fraud Detector, Snowflake, Splunk                                      |
| Alerts and notifications                        | Event-driven notification system          | AWS SNS, Twilio, Firebase                                                  |
| Compliance with AML/KYC regulations             | Identity verification platform            | Okta, Auth0, Jumio                                                         |
| Seamless checkout experience                    | Responsive checkout interface             | React, Vue, Flutter                                                        |
| High-volume transaction processing              | Scalable distributed transaction handler  | AWS DynamoDB, Google Cloud Spanner, Apache Cassandra                       |
| Multi-payment options                           | Payment gateway integration               | Stripe, Braintree, Adyen                                                   |
| Personalized recommendations                    | Recommendation engine                     | TensorFlow, AWS Personalize, Google AI Recommendations                     |
| Transaction retry mechanisms                    | Workflow engine with retry logic          | Apache Airflow, Temporal, Camunda                                          |
| Smart routing to payment processors             | Payment processor routing algorithm       | Python custom logic, AWS Step Functions, Google Cloud Functions            |
| Anomaly detection in transactions               | Machine learning-based anomaly detection  | Databricks, AWS SageMaker, Azure ML                                        |
| Encryption of sensitive data                    | Data encryption service                   | AWS KMS, HashiCorp Vault, Google Cloud KMS                                 |
| Tokenization of payment information             | Tokenization service                      | TokenEx, Braintree, Stripe                                                 |
| Instant payment confirmations                   | Real-time message queue system            | AWS Kinesis, Apache Kafka, Google Pub/Sub                                  |
| Logging and monitoring                          | Centralized logging and monitoring stack  | Splunk, Elastic Stack, AWS CloudWatch                                      |
| Long-term data retention                        | Archival storage system                   | AWS S3 Glacier, Google Cloud Storage, Azure Blob Storage                   |

## Trade-Offs

### Prioritization

## Impact

## Why Mapping Matters

The mapping exercises are critical to ensuring alignment between business and technical teams because they:

- Help stakeholders and engineers visualize the connection between business needs and technical implementations.
- Provide clarity on trade-offs between building custom solutions versus leveraging existing tools and products.
- Foster a shared language for prioritizing features and understanding the impact of technical decisions on business outcomes.

By leveraging these mappings, teams can make more informed decisions, align their efforts, and ensure the software system delivers its intended purpose while staying adaptable for future needs.