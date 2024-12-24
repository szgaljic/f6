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

## Mapping Exercises

The core of the Capability foundation revolves around two critical mapping exercises: Product Design and Architecture Design. Together, these exercises provide a structured way to bridge business requirements with technical solutions, fostering alignment and clarity across teams.

### Product Design

The Product Design Mapping exercise begins by identifying high-level Business Needs, which represent the core drivers of value for the solution. These are then mapped to Product Requirements, which define the features and behaviors the software must exhibit to meet those needs. Finally, these product requirements are translated into actionable Technical Requirements that can be implemented by the engineering team.

| **Business Need**                 | **Product Requirement**                                                  | **Technical Requirement**                                                |
|-----------------------------------|---------------------------------------------------------------------------|---------------------------------------------------------------------------|
| Actors and Integrations           | User Role Definitions & Permissions, Organizational Access               | Identity and Access Management, Authentication Flows, Authorization APIs |
| Data-Driven Decision Making       | Reporting Capabilities (real-time or scheduled), Dashboards              | Data Pipelines, Reporting Modules, Query Engines                         |
| User Details & Events             | User Profiles, Notifications, and Custom Settings                        | User Data Storage, Event Trigger Systems, Notification APIs              |
| Advanced User Engagement          | Personalized Content, Recommendations based on user behavior             | User Tracking, Recommendation Engines, AI Models                         |
| Consistent & Predictable Experience | Consistent Visual Design, Reliable Performance                          | API Design Standards, UI/UX Libraries, Consistent Response Times         |

This mapping ensures alignment between business goals and the product's functionality while providing engineers with the context they need to implement the technical requirements effectively.

### Architecture Design

Once the technical requirements are defined, the Architecture Design Mapping exercise focuses on translating them into specific implementation strategies and evaluating tools and products that can support those strategies. This process allows teams to explore whether to build custom solutions or leverage existing tools, ensuring each decision aligns with the system’s core identity and long-term strategy.

| **Technical Requirement**        | **Implementation**                                     | **Tools & Products**                             |
|----------------------------------|-------------------------------------------------------|-------------------------------------------------|
| Identity and Access Management   | Identity Provider & OAuth Flows, RBAC, JWT & Delegation | Okta, Clerk                                    |
| API Design                       | OpenAPI standards, Paging/Sorting, Validation          | OpenAPI, API Gateway                           |
| System Observability             | Usage Monitoring, Logs and Metrics, Budget Tracking    | DataDog, NewRelic                              |
| Customer Data Platform           | Data Enrichment, Behavior Tracking                    | Segment.io, Heap.io, Google Analytics          |
| Environments and Configs         | Infrastructure as Code, Config Management             | Terraform, Pulumi, AWS Configurations          |

By focusing on implementations and tools, this mapping ensures engineers have the resources to make informed decisions about what to build versus what to buy.

## Why Mapping Matters

The mapping exercises are critical to ensuring alignment between business and technical teams. They:

- Help stakeholders and engineers visualize the connection between business needs and technical implementations.
- Provide clarity on trade-offs between building custom solutions versus leveraging existing tools and products.
- Foster a shared language for prioritizing features and understanding the impact of technical decisions on business outcomes.

By leveraging these mappings, teams can make more informed decisions, align their efforts, and ensure the software system delivers its intended purpose while staying adaptable for future needs.