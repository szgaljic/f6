---
title: Capability
weight: 2
---

## Overview

_Ensuring the software delivers its intended purpose with precision and value._

At its core, software exists to solve problems, meet needs, and deliver value to users and stakeholders. **Capability** represents the foundation of functionality—the workflows, features, and solutions that define the software’s purpose. 

This foundation emphasizes delivering the right functionality, at the right time, to the right users. It's about carefully considering the purpose of the software and prioritizing it's feature sets. Capability also underscores the importance of intentionality. Adding unnecessary features or poorly implementing required ones can dilute focus, introduce technical debt, and create frustration for users. 

A system that fulfills its purpose with precision and clarity becomes not just functional, but invaluable. 

## Discovery and Analysis

Understanding Capability starts with deep discussions during discovery sessions, where stakeholders and engineers collaborate to align on requirements. These sessions involve exploring the current state of the system, defining the future state, and identifying gaps between the two.

During these conversations, the mapping exercises—Product Design and Architecture Design—help provide structure, ensuring that discussions result in actionable insights. While this section introduces the importance of discovery, detailed guidance on conducting these sessions is covered in the F6 Discovery section.

## Capability Mapping

Central to the Capability foundation is the **Capability Mapping Exercise**. It provides a structured approach to align business goals with technical execution by creating clear mappings between high-level objectives and implementation strategies. This exercise ensures alignment, avoids redundancy, and provides clarity for decision-making.

{{% callout warning %}}
This process focuses on mapping and alignment. It does not address trade-offs, project planning, or risk evaluation, which are covered in other foundational aspects of the F6 Framework.
{{% /callout %}}

The steps are as follows:

1. **Product Design Mapping:** Identify Business Needs and map them to Product Requirements and Technical Requirements. This step ensures a clear understanding of the "what" behind the product.
2. **Technical Themes:** Group the Technical Requirements into logical themes to manage complexity and highlight overlaps.
3. **Architecture Design Mapping:** Refine Technical Themes into specific implementations and map them to tools, platforms, or products.

### Product Design Mapping

The **Product Design Mapping** exercise begins by identifying high-level **Business Needs**, which represent the core drivers of value for the solution. These are then mapped to **Product Requirements**, which define the features and behaviors the software must exhibit to meet those needs. Finally, these product requirements are translated into actionable **Technical Requirements** that can be implemented by the engineering team.

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

This step ensures that technical teams understand the connection between business objectives and their work. For example, "Fraud Prevention and Detection" translates into a set of tools and techniques that proactively identify and mitigate risks. The emphasis here is on capturing the "what" without diving into specific tools or solutions.

### Technical Themes

After defining the Technical Requirements, the next step is grouping them into themes. Themes help abstract and organize the requirements into manageable clusters. These groupings reduce redundancy and provide a clear structure for implementation strategies.

| **Technical Requirement**                             | **Proposed Technical Theme(s)**                    |
|-------------------------------------------------------|---------------------------------------------------|
| Load balancing, Horizontal scaling                   | Scalability                                       |
| Payment processor routing algorithms, Failure-handling mechanisms | Workflow Engine, State Management                |
| Anomaly detection algorithms, Real-time data pipelines | Fraud Detection, Real-Time Processing            |
| End-to-end encryption, Tokenization services         | Data Security, Privacy                           |
| Identity verification systems, Logging and monitoring | Identity Management, Audit and Compliance        |
| Logging and monitoring, Data archival systems        | Audit and Compliance, Data Retention             |
| Distributed databases, Cloud-based architecture      | Scalability, Cloud-Native Architecture           |
| User state management, Recommendation engines      | Personalization, User Experience                 |
| Payment gateway integration, Mobile SDKs             | API Management, User Experience                  |
| Failure-handling mechanisms, Data aggregation and reporting tools | Workflow Engine, Observability                  |
| Cost modeling systems, Cloud cost optimization tools | Cost Optimization                                |
| Tokenization services, Data masking techniques       | Data Security, Privacy                           |
| Event-driven architectures, Low-latency message queues | Real-Time Processing, Scalability               |
| API management platforms, Protocol translation layers | Interoperability                                 |

In this example, requirements like "Load balancing" and "Horizontal scaling" naturally fit under the theme of "Scalability." Similarly, "Payment processor routing algorithms" align with themes like "Workflow Engine" and "State Management." Allowing overlaps ensures that teams recognize areas where solutions might serve multiple purposes.

```markmap
- Workflow Engine
  - Payment processor routing algorithms
  - Failure-handling mechanisms
  - Data aggregation and reporting tools
- Fraud Detection
  - Anomaly detection algorithms
- Real-Time Processing
  - Anomaly detection algorithms
  - Real-time data pipelines
  - Event-driven architectures
  - Low-latency message queues
- Personalization
  - User state management
  - Recommendation engines
- Cost Optimization
  - Cost modeling systems
  - Cloud cost optimization tools
- Interoperability
  - API management platforms
  - Protocol translation layers
```

The focus is on flexibility. Themes provide structure but do not impose rigid boundaries, making them adaptable to various contexts.

### Architecture Design Mapping

The final step refines the Technical Themes into actionable implementation strategies. These strategies are then linked to tools, platforms, or products that can fulfill them.

| **Technical Theme**         | **Implementation**                                    | **Tools & Products**                                                            |
|------------------------------|------------------------------------------------------|---------------------------------------------------------------------------------|
| Scalability                 | Load balancing, Horizontal scaling, Distributed systems | AWS Elastic Load Balancing, Kubernetes, Redis, Amazon DynamoDB, Google Cloud Spanner |
| Workflow Engine             | Task orchestration, State transitions, Retry mechanisms | Apache Airflow, Temporal, Camunda, AWS Step Functions                           |
| State Management            | State synchronization, Transaction consistency         | Apache Kafka, RabbitMQ, Redis Streams                                           |
| Fraud Detection             | Anomaly detection algorithms, Rule-based fraud detection | Databricks, Snowflake, Splunk, AWS Fraud Detector                               |
| Real-Time Processing        | Event-driven architecture, Low-latency message queues  | Apache Kafka, AWS Kinesis, Google Pub/Sub                                       |
| Data Security               | End-to-end encryption, Tokenization, Secure data storage | AWS KMS, HashiCorp Vault, Google Cloud Key Management, Okta                     |
| Privacy                     | Consent management, Data anonymization, Masking sensitive information | Privitar, Informatica, Immuta                                                   |
| Identity Management         | Authentication, Authorization, Role-based access control | Okta, Auth0, AWS Cognito, Azure Active Directory                                |
| Audit and Compliance        | Logging, Monitoring, Audit trails                     | Splunk, Elastic Stack, AWS CloudTrail, Azure Monitor                            |
| Data Retention              | Archival systems, Long-term storage                   | AWS S3 Glacier, Google Cloud Storage, Azure Blob Storage                        |
| Cloud-Native Architecture   | Containerization, Serverless architecture             | Kubernetes, Docker, AWS Lambda, Azure Functions                                 |
| Personalization             | Recommendation engines, User behavior analytics       | TensorFlow, AWS Personalize, Google AI Recommendations                          |
| User Experience             | Seamless integrations, Mobile-friendly SDKs           | Stripe SDKs, Braintree, Flutter, React Native                                   |
| API Management              | API gateways, Protocol mediation                      | Kong, Apigee, AWS API Gateway, MuleSoft                                         |
| Interoperability            | Cross-platform integration, Message format standardization | MuleSoft, Zapier, Postman, Apache Camel                                        |
| Cost Optimization           | Cost monitoring, Batch processing, Resource allocation | AWS Cost Explorer, Google Cloud Billing, Spot.io, Kubecost                      |

For instance, the theme of "Scalability" translates into implementations like load balancing and distributed systems. These implementations can be achieved using tools such as Kubernetes, Redis, or AWS Elastic Load Balancing. Providing a range of tools ensures teams can choose solutions that align with their specific needs and constraints.

This mapping is not about prescribing a single "right" tool but about offering a menu of options. Teams should evaluate these options based on factors such as cost, scalability, and integration with existing syste

## Why Mapping Matters

The mapping exercises are critical to ensuring alignment between business and technical teams because they:

- Help stakeholders and engineers visualize the connection between business needs and technical implementations.
- Provide clarity on trade-offs between building custom solutions versus leveraging existing tools and products.
- Foster a shared language for prioritizing features and understanding the impact of technical decisions on business outcomes.

By leveraging these mappings, teams can make more informed decisions, align their efforts, and ensure the software system delivers its intended purpose while staying adaptable for future needs.