---
title: Features
weight: 1
---

## Overview

_“What should the solution do?”_

At its core, software exists to solve problems and deliver value to users and stakeholders. **Capability represents the foundation of functionality**—the workflows, features, and solutions that define the software’s purpose. 

The **Capability** foundation is about carefully considering the purpose of the software and underscores the importance of intentionality through **Capability Mapping**. It provides a powerful means for business stakeholders to understand how their needs cascade down to impact product features and technical implementation. Adding unnecessary features or poorly implementing required ones can dilute focus, introduce technical debt, and create frustration for users. 

Capability also bring attention to [**the base foundation**](/docs/foundations/capability/#the-base-foundation)—the initial setup and architectural blueprint that underpins the entire system. This often invisibile step is critical to implementation that is frequently overlooked. 

### Out-of-Scope

This foundation focuses on defining and delivering functionalities aligned with business and user needs. It does not cover broader considerations such as resource allocation, prioritization, or timelines. These aspects are addressed in the [**Investment**](/docs/foundations/investment) foundation and the [**F6 Discovery Process**](/docs/f6-discovery/).

Similarly, this foundation does not provide a comprehensive review of technical implementation strategies or architectural designs. While the Implementation Mapping section offers examples to illustrate the concept of base foundations, detailed architectural exploration is left to technical teams and leaders, supported by established methodologies.

## What is Capability?

**Capability** is captured through in-depth discussions where stakeholders describe their needs, and the implementation team translates these into functional and non-functional requirements. 

**Functional requirements** define the specific behaviors, features, or workflows the system must deliver to meet user and business needs, as distinct from **Non-Functional requirements**, which address performance, scalability, or other operational characteristics.

The process typically involves capturing the current state, defining the desired future state, and identifying the gaps between the two. These gaps represent the project scope. While this is a standard industry practice, F6 enhances it by applying **Capability Mapping** to clearly correlate requirements into business needs.

### Examples of Capability

In an ideal world, capabilities would always align directly with specific business needs, delivering exactly what stakeholders and users require. However, the reality is often more complex. Some capabilities exist to directly serve business goals, while others function to enable or support those higher-level capabilities.

Here are some examples: 

- **Core Workflow Efficiency:** A fintech platform may prioritize seamless transaction flows, such as enabling one-click payment for customers while ensuring real-time fraud checks in the background. This capability streamlines user experience while maintaining robust security.

- **Regulatory Compliance Enablement:** A healthcare application must integrate features that ensure compliance with HIPAA, such as audit trails, secure data sharing, and patient consent management. These capabilities are foundational to operating in a regulated industry.

- **Scalability for Growth:** An e-commerce site designed for a small customer base must be capable of scaling to handle seasonal spikes, like Black Friday traffic, with features such as dynamic resource allocation and robust caching mechanisms.

It’s perfectly acceptable—and even expected—for certain capabilities to be technical in nature. Doing so will highlight the elevated importance of those capabilities.

## Foundational Impacts

Highly technical teams often consider enabling capabilities naturally such as those related to [**Dependency**](/docs/foundations/dependency), [**Resiliency**](/docs/foundations/resiliency), or [**Security**](/docs/foundations/security). For those who may not initially account for these areas, F6 identifies them as distinct foundations, ensuring they are properly addressed and cross-checked within the solution’s requirements.

Capabilities are the main reason why the solution exists and heavily leads all other foundations. Here’s how it interacts:

| **Foundation**               | **Impact of Capability**                                                                        |
|------------------------------|-------------------------------------------------------------------------------------------------|
| Volatility                   | Business needs are constantly evolving and is usually the primary driver of change. |
| Dependency                   | Capabilities guide the underlying systems interdependencies, which must be built and maintained. |
| Security                     | Capabilities either address or require security, such as encryption or compliance mechanisms. |
| Resilience                   | Supporting capabilities often underpin system stability, ensuring reliability and performance under stress. |
| Investment                   | Capabilities can be enhanced or reduced, directly affecting cost, time, and resource trade-offs.  |

## Capability Mapping

Central to the Capability foundation is **Capability Mapping**. It provides a structured approach to align business goals with technical execution by creating mappings between high-level objectives and implementation strategies. 

This process focuses on mapping and alignment, serving as a foundation for making trade-offs, planning projects, and evaluating risks, which are further supported by other aspects of F6.

The steps are as follows:

1. **Business to Product Requirements:** Translate high-level business needs into product requirements.
2. **Product to Technical Requirements:** Define the technical requirements needed to achieve the product's functionality.
3. **Implementation:** Develop the systems using architectures, tools, and techniques aligned with the technical requirements.

### Business to Product Requirements

Every solution starts with trying to understand its purpose and the problems it aims to solve. For illustration, we will use a **FinTech payment processing system** as an example to show how business goals translate into execution.

Imagine a strategy meeting where stakeholders are sharing their vision for the new platform. They aren’t speaking in technical terms; they’re articulating broad goals that matter to the business and its customers. For instance, two of their statements might be:

- _"We need to proactively detect and prevent fraudulent transactions to protect our customers and our reputation."_
- _"Compliance with financial regulations like AML and KYC is non-negotiable."_

On the surface, these seem straightforward. Fraud detection, prevention, and compliance—how hard can it be? But as we refine these statments, they unravel into a complex web of needs that the product must address:

1. **Fraud Detection:** Identifying potentially fraudulent transactions before they are completed.
2. **Fraud Prevention:** Blocking or mitigating fraudulent activity in real time.
3. **Reputation Protection:** Ensuring trust by managing fraud risks proactively.
4. **Regulatory Compliance:** Meeting AML (Anti-Money Laundering) and KYC (Know Your Customer) standards.
5. **Auditability:** Providing detailed records for compliance audits.
6. **Customer Verification:** Implementing workflows to verify user identities.

These refined business needs are still abstract but give us a clearer picture of what the platform must achieve. The next step is to translate these into **Product Requirements**—the tangible workflows and features the platform must offer:

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

Notice how much detail emerges from just two statements! For example, stakeholders didn’t explicitly ask for a **Compliance Dashboard**, but it’s an essential feature to help compliance officers manage and track regulatory requirements effectively. Similarly, **Transaction Blocking** wasn’t mentioned outright, but it’s a critical part of fraud prevention that aligns with the goal of protecting customers and the business.

The product team has filled in the gaps, revealing needs that might not have been obvious initially. It also underscores how business needs cascade and expand with each conversation. 

{{% callout note %}}
As a stakeholder, it’s crucial to pay close attention to how your statements are being interpreted. At the same time, sharing detailed insights about the system’s long-term vision is equally important, as it equips the team to plan for the system’s evolution and more effectively achieve future goals. This concept is explored further in the [**Volatility**](/docs/foundations/volatility) foundation.
{{% /callout %}}

### Product to Technical Requirements

The conversation now shifts to deriving the **Technical Requirements**—broad characteristics that define what the underlying architecture and system must achieve. 

We'll focus on three product requirements for illustration: **Real-Time Fraud Monitoring**, **KYC Verification**, and **Alerts and Notifications**. We can show how functional and non-functional needs are considered and how the technical team begins to define the architecture's enabling capabilities.

Much like how the product team "fills in the gaps" for stakeholders, technical teams are "filling in the gaps" for the product team—considering scalability, data flows, processing needs, and other enabling technical factors. 

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

Notice how in addition to the obvious functional requirements, they consider factors like performance, scalability, and security—critical elements that stakeholders might not explicitly articulate. Without guidance, technical teams will draw their own conclusions about how to address key aspects like [**Resiliency**](/docs/foundations/resiliency) (performance and reliability), [**Dependency**](/docs/foundations/dependency) (dependencies and compatibility), or [**Security**](/docs/foundations/security) (data protection and compliance).

{{% callout note %}}
F6 offers stakeholders a chance to influcence the design of Capabilities at key low-level requirements through aspects such as [**Resiliency**](/docs/foundations/resiliency), [**Dependency**](/docs/foundations/dependency), and [**Security**](/docs/foundations/security)—areas that might otherwise be overlooked.
{{% /callout %}}

The outcome is a set of Technical Requirements that provide a low-level needs list for the system. 

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

At this stage, the product and technical teams collaborate to refine the list further into a more cohesive description of the architecture. While this level of detail is outside the primary focus of F6, it’s important to note that another layer of translation takes place here.

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

We can demonstrate mapping six technical requirements into different base foundations by selecting two from each product requirement from the previous step.

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


To understand the mapping chain in action, let’s examine one technical requirement: **Real-Time Event Processing Systems**.

- **Business Need:** Detect and prevent fraudulent transactions.
- **Product Requirement:** Real-time fraud monitoring.
- **Technical Requirement:** Real-time event processing systems.
    - **Implementation (GCP/Containers):** Pub/Sub is used to process streaming data, with Kubernetes scaling services as needed.
    - **Implementation (AWS/Serverless):** EventBridge orchestrates event-driven workflows, triggering Lambda functions to process data in real time.

## Why This Matters

At the forefront of a solution are the visible business capabilities that directly deliver value for stakeholders. Supporting these are the enabling capabilities: the refined inner workflows often related to [**Dependency**](/docs/foundations/dependency), [**Resiliency**](/docs/foundations/resiliency), and [**Security**](/docs/foundations/security) that make those business capabilities possible. Beneath it all lies the foundational layer—[**the base foundation**](/docs/foundations/capability/#the-base-foundation) underpinning the entire solution.

The **Capability** foundation asks the main question: “What should the solution do?” It provides a structured approach to answering this question through **Capability Mapping** and offers a means for traceability. 

By explicitly connecting visible business goals to their enabling and foundational layers, it highlights the interconnectedness of the solution—from the high-level objectives down to the unseen but critical underpinnings.