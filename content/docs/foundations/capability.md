---
title: Capability
weight: 1
---

## Overview

_Ensuring technology delivers its intended purpose with excellence._

At its core, software exists to solve problems, meet needs, and deliver value to users and stakeholders. **Capability represents the foundation of functionality**—the workflows, features, and solutions that define the software’s purpose. 

The Capability foundation is about carefully considering the purpose of the software and underscores the importance of intentionality. Adding unnecessary features or poorly implementing required ones can dilute focus, introduce technical debt, and create frustration for users. 

It also provides a powerful means for business stakeholders to understand how their needs cascade down to impact product features and technical implementation.

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

### Everything is Capability

As you'll see... TBD

## Priorities

MVP, Roadmap

## Capability Mapping

Central to the Capability foundation is **Capability Mapping**. It provides a structured approach to align business goals with technical execution by creating clear mappings between high-level objectives and implementation strategies. 

This process focuses on mapping and alignment. It does not directly address trade-offs, project planning, or risk evaluation, which are covered in other aspects of the F6.

The steps are as follows:

1. **Business to Product:** TBD.
2. **Product to Technical:** TBD.
3. **Implementation:** TBD.

### Business to Product Requirements

Every solution starts with trying to understand its purpose and the problems it aims to solve. For illustration, we will use a **FinTech payment processing system** as an example to show how business goals translate into execution.

Imagine a strategy meeting where stakeholders are sharing their vision for the new platform. They aren’t speaking in technical terms; they’re articulating broad goals that matter to the business and its customers. For instance, two of their statements might be:

- _"We need to proactively detect and prevent fraudulent transactions to protect our customers and our reputation."_
- _"Compliance with financial regulations like AML and KYC is non-negotiable."_

On the surface, these seem straightforward. Fraud detection, prevention, and compliance—how hard can it be? But as we dive deeper, these statements unravel into a complex web of needs that the product must address.

1. **Fraud Detection:** Identifying potentially fraudulent transactions before they are completed.
2. **Fraud Prevention:** Blocking or mitigating fraudulent activity in real time.
3. **Reputation Protection:** Ensuring trust by managing fraud risks proactively.
4. **Regulatory Compliance:** Meeting AML (Anti-Money Laundering) and KYC (Know Your Customer) standards.
5. **Auditability:** Providing detailed records for compliance audits.
6. **Customer Verification:** Implementing workflows to verify user identities.

These refined business needs are still abstract but give us a clearer picture of what the platform must achieve. The next step is to translate these into **Product Requirements**—the tangible workflows and features the platform must offer.

| **Business Need(s)**            | **Product Requirement**                | **Description**                                                                       |
|-------------------------------|----------------------------------------|---------------------------------------------------------------------------------------|
| Fraud Detection               | Real-Time Fraud Monitoring             | Continuously track transactions for suspicious patterns.                              |
| Fraud Detection               | Risk Scoring Workflow                  | Assign risk scores to transactions based on fraud indicators.                        |
| Fraud Detection, Fraud Prevention | Alerts and Notifications           | Trigger alerts or workflows for flagged transactions.                                |
| Fraud Prevention              | Transaction Blocking                   | Prevent high-risk transactions from being processed.                                 |
| Fraud Prevention              | Fraud Mitigation Tools                 | Enable manual review and intervention for flagged activity.                          |
| Fraud Detection, Fraud Prevention | Adaptive Rules Engine              | Allow dynamic updates to fraud detection rules.                                      |
| Fraud Prevention, Reputation Protection | Customer Transparency        | Provide users with updates on flagged transactions.                                  |
| Fraud Prevention, Reputation Protection | Incident Reporting            | Generate reports on fraud incidents to build accountability.                         |
| Regulatory Compliance         | AML Checks                             | Automate Anti-Money Laundering screenings.                                           |
| Regulatory Compliance         | KYC Verification                       | Verify customer identity during onboarding.                                          |
| Regulatory Compliance         | Transaction Reporting                  | Submit required reports to regulators.                                               |
| Auditability                  | Activity Logging                       | Maintain detailed, immutable records of all system activities.                       |
| Auditability, Regulatory Compliance | Compliance Dashboards           | Provide visual tools for compliance officers to track adherence.                     |
| Customer Verification         | Onboarding Workflow                    | Guide users through a seamless identity verification process.                        |
| Customer Verification         | Document Upload and Validation         | Allow customers to upload identification documents for verification.                 |
| Customer Verification         | Ongoing Verification                   | Re-verify customer identities periodically to ensure continued compliance.           |

Notice how much detail emerges from just two statements. For example, stakeholders didn’t explicitly ask for a **Compliance Dashboard**, but it’s an essential feature to help compliance officers manage and track regulatory requirements effectively. Similarly, **Transaction Blocking** wasn’t mentioned outright, but it’s a critical part of fraud prevention that aligns with the goal of protecting customers and the business.

The product team has filled in the gaps, revealing needs that might not have been obvious initially. It also underscores how business needs cascade and expand with each conversation. 

{{% callout note %}}
As a stakeholder, it’s crucial to pay close attention to how your statements are being interpreted. At the same time, sharing detailed insights about the system’s long-term vision is equally important, as it equips the team to plan for the system’s evolution and more effectively achieve future goals. This concept is explored further in the **Volatility** foundation.
{{% /callout %}}

### Product to Technical Requirements

The conversation now shifts to deriving the **Technical Requirements**—broad characteristics that define what the underlying architecture and system must achieve. 

We'll focus on three specific product requirements: **Real-Time Fraud Monitoring**, **KYC Verification**, and **Alerts and Notifications**. These examples demonstrate how functional and non-functional needs are considered and how the technical team begins to define the architecture's fundamental capabilities.

Much like how the product team "fills in the gaps" for stakeholders, technical teams are "filling in the gaps" for the product team—considering scalability, data flows, processing needs, and other foundational technical factors. 

- **Real-Time Fraud Monitoring**
    - How to handle large volumes of transactional data in real time.
    - How to implement detection algorithms that can operate with minimal latency.
    - How to design the system to scale with transaction growth.
- **KYC Verification**
    - How to securely collect, store, and manage customer identity information.
    - How to integrate with external systems for identity verification (e.g., government databases or third-party services).
    - How to ensure compliance with data retention policies and regulatory standards.
- **Alerts and Notifications**
    - How to trigger notifications based on predefined events or thresholds.
    - How to deliver notifications across multiple channels (e.g., email, SMS, app alerts).
    - How to ensure notifications are reliable and scalable.

Notice how in addition to the obvious functional requirements, they consider factors like performance, scalability, and security—critical elements that stakeholders might not explicitly articulate. Without guidance, technical teams will draw their own conclusions about how to address key aspects like **Resiliency** (performance and reliability), **Dependency** (dependencies and compatibility), or **Security** (data protection and compliance).

{{% callout note %}}
The F6 Framework offers stakeholders a chance to influcence the design of Capabilities at key low-level requirements through aspects such as **Resiliency**, **Dependency**, and **Security**—areas that might otherwise be overlooked.
{{% /callout %}}

The outcome is a set of Technical Requirements that provide a high-level blueprint for the system. 

| **Product Requirement**      | **Technical Requirements**                                                    |
|-------------------------------|-------------------------------------------------------------------------------|
| Real-Time Fraud Monitoring    | Real-time event processing systems                                            |
| --                            | Scalable data pipelines                                                       |
| --                            | Low-latency anomaly detection algorithms                                      |
| --                            | High-throughput transaction processing                                        |
| --                            | Continuous system monitoring and alerting                                     |
| KYC Verification              | Secure data storage and encryption                                            |
| --                            | API integrations for external identity verification                           |
| --                            | Identity validation workflows                                                 |
| --                            | Regulatory-compliant data retention policies                                  |
| --                            | Logging and audit trails for all KYC-related actions                          |
| Alerts and Notifications      | Event-driven notification system                                              |
| --                            | Multi-channel notification delivery                                           |
| --                            | Reliable message queuing and processing                                       |
| --                            | Dynamic configuration of notification rules                                   |
| --                            | Monitoring and logging of notification workflows                              |

This stage offers a checkpoint where any misalignments between product and technical teams can be resolved. 

### Implementation

The last step is to bridge the gap between technical requirements and the practical technologies and architectures that bring them to life. At this stage, decisions are made about how the solution will be built—down to the frameworks, tools, and platforms. While stakeholders might see only the end results of these decisions, the underlying choices directly impact the solution's adaptability and alignment with business goals for years to come. 

#### The Base Foundation

A critical, often invisible, part of this process is the **base foundation**—the initial setup and architectural blueprint that underpins the entire system. This base foundation determines how other layers of the solution are developed and interacts with the business needs through technical requirements.

For example, consider the setup of cloud environments, deployment pipelines, or the selection of a programming language. These decisions aren't directly tied to a specific business need but are critical for enabling all technical requirements to be met.

{{% callout note %}}
Base foundations often reflect the expertise and experience of the technical team involved. Without structured evaluation or guidance, these decisions will default to what the team knows best—whether or not it’s the best fit for the business goals.
{{% /callout %}}

It takes an experienced leader with both technical and business acumen to evaluate multiple options and ensure the chosen foundation aligns with both technical requirements and business priorities.

#### Implementation Mapping

To illustrate how base foundations influence implementation, consider two fictional experienced tech leads:

- **Alex**, an expert in GCP/Containers, proposes a foundation based on Google Cloud Platform, Kubernetes, and Java/Spring Boot.
- **Jessica**, proficient in AWS/Serverless, suggests a foundation leveraging AWS Lambda, DynamoDB, and Node.js.

Select six of the technical requirements from the previous step, two from each product requirement, we can demonstrate mapping them into different base foundations.

| **Technical Requirement**            | **GCP/Containers**                                                              | **AWS/Serverless**                                                                 |
|--------------------------------------|---------------------------------------------------------------------------------|----------------------------------------------------------------------------------|
| Real-Time Event Processing Systems   | Pub/Sub for streaming; scalable Kubernetes services                             | EventBridge for orchestration; Lambda-based real-time processing pipelines       |
| Continuous System Monitoring & Alerting | Stackdriver integration for logging and alerting                                | CloudWatch dashboards and custom alarms                                         |
| Secure Data Storage & Encryption     | Encrypted Cloud SQL instances and managed encryption keys                       | DynamoDB encryption at rest; KMS-managed keys for additional security           |
| API Integrations for Identity Verification | RESTful APIs built with Spring Boot, hosted on Kubernetes                      | Lambda functions for API requests, integrating with Cognito for identity        |
| Multi-Channel Notification Delivery  | Cloud Functions for email/SMS; Pub/Sub for asynchronous notification workflows | SNS for SMS/email; Lambda for dynamic notification rule handling                |
| Dynamic Configuration of Notification Rules | ConfigMaps in Kubernetes for dynamic rule management                           | Parameter Store and Lambda for dynamic updates                                  |

Both of these foundations can end up satisfying the technical requirements, yet there non-obvious impacts of their decisons. 

#### Capability Chain

To understand the mapping chain in action, let’s examine one specific example: Real-Time Event Processing Systems.

- **Business Need:** Detect and prevent fraudulent transactions.
- **Product Requirement:** Real-time fraud monitoring.
- **Technical Requirement:** Real-time event processing systems.
    - **Implementation (GCP/Containers):** Pub/Sub is used to process streaming data, with Kubernetes scaling services as needed.
    - **Implementation (AWS/Serverless):** EventBridge orchestrates event-driven workflows, triggering Lambda functions to process data in real time.

This example showcases how the entire chain—from high-level business objectives to low-level implementation—is informed by both technical expertise and strategic decision-making.