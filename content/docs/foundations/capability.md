---
title: Capability
weight: 2
---

## Overview

_Ensuring technology delivers its intended purpose with excellence._

At its core, software exists to solve problems, meet needs, and deliver value to users and stakeholders. **Capability** represents the foundation of functionality—the workflows, features, and solutions that define the software’s purpose. 

This foundation emphasizes delivering the right functionality, at the right time, to the right users. It's about carefully considering the purpose of the software and prioritizing it's feature sets. Capability also underscores the importance of intentionality. Adding unnecessary features or poorly implementing required ones can dilute focus, introduce technical debt, and create frustration for users. 

A system that fulfills its purpose with precision and clarity becomes not just functional, but invaluable. 

## Discovery and Analysis

Uncovering capability invovles in-depth discussions where stakeholders describe their needs, and the implementation team translates these into functional and non-functional requirements. 

**Functional requirements** define the specific behaviors, features, or workflows the system must deliver to meet user and business needs, as distinct from **Non-Functional requirements**, which address performance, scalability, or other operational characteristics.

The process typically involves capturing the current state, defining the desired future state, and identifying the gaps between the two. These gaps represent the project scope. While this is a standard industry practice, the F6 Framework enhances it by applying **Capability Mapping** to clearly correlate Business Needs into these requirements.

The mapping exercises described below bring structure and provide a way to reason about what capabilties are required and why.

{{% callout note %}}
A detailed guidance on conducting holiistic discovery sessions is covered in [F6 Discovery Process](/docs/f6-discovery/).
{{% /callout %}}

## Capability Mapping

Central to the Capability foundation is **Capability Mapping**. It provides a structured approach to align business goals with technical execution by creating clear mappings between high-level objectives and implementation strategies. This exercise ensures alignment, avoids redundancy, and provides clarity for decision-making.

This process focuses on mapping and alignment. It does not address trade-offs, project planning, or risk evaluation, which are covered in other foundational aspects of the F6 Framework.

The steps are as follows:

1. **Requirements Mapping:** Identify Business Needs and map them to Product Requirements and Technical Requirements. This step ensures a clear understanding of the "what" behind the product.
2. **Theme Consolidation:** Group the requirements into logical themes to manage complexity and highlight overlaps.
3. **Implementation Mapping:** Refine the requirements into themes, mapping them to specific implementations techniques, tools and products.

### Requirements Mapping

The **Requirements Mapping** exercise begins by identifying high-level **Business Needs**, which represent the core drivers of value for the solution. These are then mapped to **Product Requirements**, which define the features and behaviors the software must exhibit to meet those needs. Finally, these product requirements are translated into actionable **Technical Requirements** that can be implemented by the engineering team.

For the purposes of concrete illustration, we will use a FinTech payment processing system as an example to show how business goals translate into technical execution.

| **Business Need**           | **Product Requirements**                                                                 | **Technical Requirements**                                                                 |
|------------------------------|-----------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------|
| Fraud Prevention and Detection | Fraud monitoring, Transaction risk scoring, Alerts and notifications, Chargeback management | Anomaly detection algorithms, Real-time data pipelines, Rule-based systems, Transaction logging and analysis |
| Regulatory Compliance        | Compliance Requirements, AML/KYC verification, Audit trails, Transaction reporting, Data retention policies       | Compliance frameworks (e.g., PCI-DSS), Identity verification systems, Logging and monitoring, Data archival systems |
| Scalability                  | High-volume transaction processing, Multi-region support, Dynamic resource allocation     | Load balancing, Horizontal scaling, Distributed databases, Cloud-based architecture       |
| Customer Retention           | Seamless checkout experience, Personalized recommendations, Multi-payment options         | User state management, Recommendation engines, Payment gateway integration, Mobile SDKs |
| Revenue Optimization         | Transaction retry mechanisms, Smart routing to payment processors, Revenue leakage reports | Payment processor routing algorithms, Failure-handling mechanisms, Data aggregation and reporting tools |
| Cost Efficiency              | Optimized processing fees, Batch processing for settlements, Infrastructure cost monitoring | Cost modeling systems, Batch processing frameworks, Cloud cost optimization tools        |
| Data Security and Privacy    | Encryption of sensitive data, Tokenization of payment information, Consent management     | End-to-end encryption, Tokenization services, Data masking techniques, Access control systems |
| Real-Time Processing         | Instant payment confirmations, Real-time transaction updates, Push notifications         | Event-driven architectures, Low-latency message queues, Real-time processing frameworks |
| Interoperability             | Integration with financial institutions, Open API ecosystem, Cross-border payment capabilities | API management platforms, Protocol translation layers, Message format standardization    |

This table provides a means to understand the connection between business needs, product behavioral requirements and technical implementation requirements. 

For example, "Fraud Prevention and Detection" translates into a set of tools and techniques that proactively identify and mitigate risks. The emphasis here is on capturing the "what" without diving into specific tools or solutions.

### Theme Consolidation

Once the requirements are defined, the next step is to group both Product Requirements and Technical Requirements into logical themes. This serves two purposes: simplifying the complexity of the requirements and creating alignment between what the business wants to achieve and how it will be implemented.

By consolidating themes at both the product and technical levels, we can identify possible patterns or overlaps between business needs, effectively de-duping requirements. 

#### Product Themes

Product Themes group related requirements that reflect the user-facing aspects of the system, such as workflows, user experience, or compliance needs. These themes provide visibility to stakeholders by showing how their priorities translate into product features.

| **Product Theme**          | **Requirements**                                                                         |
|-----------------------------|-----------------------------------------------------------------------------------------|
| User Experience            | Seamless checkout experience, Multi-payment options                                     |
| Risk Management            | Fraud monitoring, Alerts and notifications                                              |
| Regulatory Compliance      | Compliance requirements, AML/KYC verification                                           |
| Performance Optimization   | Transaction retry mechanisms, Smart routing to payment processors                       |
| Personalization            | Personalized recommendations, Customer loyalty programs                                 |

```markmap
- Product Themes
  - User Experience
    - Seamless checkout experience
    - Multi-payment options
  - Risk Management
    - Fraud monitoring
    - Alerts and notifications
  - Regulatory Compliance
    - Compliance requirements
    - AML/KYC verification
  - Performance Optimization
    - Transaction retry mechanisms
    - Smart routing to payment processors
  - Personalization
    - Personalized recommendations
    - Customer loyalty programs
```

#### Technical Themes

Technical Themes group the underlying technical implementations needed to fulfill the product requirements. These themes allow implementation teams to streamline development efforts and focus on reusable solutions.

| **Technical Theme**        | **Requirements**                                                                         |
|-----------------------------|-----------------------------------------------------------------------------------------|
| Scalability                | Load balancing, Horizontal scaling                                                      |
| Fraud Detection            | Anomaly detection algorithms, Real-time data pipelines                                  |
| Data Security              | End-to-end encryption, Tokenization services                                            |
| Privacy                    | Data masking techniques, Consent management                                             |
| Real-Time Processing       | Event-driven architectures, Low-latency message queues                                  |
| Audit and Compliance       | Identity verification systems, Logging and monitoring                                   |
| Cloud-Native Architecture  | Distributed databases, Cloud-based architecture                                         |

```markmap
- Technical Themes
  - Scalability
    - Load balancing
    - Horizontal scaling
    - Distributed systems
  - Fraud Detection
    - Anomaly detection algorithms
    - Real-time data pipelines
  - Data Security
    - End-to-end encryption
    - Tokenization services
  - Real-Time Processing
    - Event-driven architectures
    - Low-latency message queues
  - Audit and Compliance
    - Identity verification systems
    - Logging and monitoring
```

The focus is on flexibility. Themes provide structure but do not impose rigid boundaries, making them adaptable to various contexts.

### Implementation Mapping

The final step is Implementation Mapping, where we unify the previously consolidated product and technical themes into actionable, detailed requirements. These unified requirements represent the distilled essence of what the system needs to achieve and provide a bridge between high-level business needs and practical engineering efforts.

By refining these requirements into implementation strategies and mapping them to possible tools and products, we ensure stakeholders and implementation teams have a shared understanding of the system’s deliverables. This process eliminates duplication, reduces ambiguity, and aligns technical efforts with strategic goals.

| **Requirement**                                  | **Implementation**                        | **Tools & Products**                                                        |
|--------------------------------------------------|-------------------------------------------|-----------------------------------------------------------------------------|
| Fraud monitoring                                 | Real-time fraud detection system          | AWS Fraud Detector, Snowflake, Splunk                                      |
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


For instance, the theme of "Scalability" translates into implementations like load balancing and distributed systems. These implementations can be achieved using tools such as Kubernetes, Redis, or AWS Elastic Load Balancing. Providing a range of tools ensures teams can choose solutions that align with their specific needs and constraints.

This mapping is not about prescribing a single "right" tool but about offering a menu of options. Teams should evaluate these options based on factors such as cost, scalability, and integration with existing syste

## Why Mapping Matters

The mapping exercises are critical to ensuring alignment between business and technical teams because they:

- Help stakeholders and engineers visualize the connection between business needs and technical implementations.
- Provide clarity on trade-offs between building custom solutions versus leveraging existing tools and products.
- Foster a shared language for prioritizing features and understanding the impact of technical decisions on business outcomes.

By leveraging these mappings, teams can make more informed decisions, align their efforts, and ensure the software system delivers its intended purpose while staying adaptable for future needs.