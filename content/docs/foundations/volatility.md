---
title: Volatility
weight: 1
---

## Overview

_Navigating the contours of change with curiosity and precision._

It’s been said that the only constant in life is **change**. Software is no different; it’s a depreciating asset that must be updated, altered, and maintained to stay effective.

The **Volatility** foundation emphasizes the balance between rapid progress and thoughtful precision. It acknowledges the duality of software development: the need to deliver impactful results quickly while ensuring those results are built with the care and precision required for their intended lifetime. 

This aspect recognizes a sliding scale: are you building for the "here and now," accepting the potential for more significant rewrites later, or investing in a foundation that supports seamless evolution over time? Both approaches have their place, depending on the solutions goals, constraints, and maturity. [Software is never truly "done," and every decision made today influences how effectively it can evolve tomorrow.](https://insights.jahnelgroup.com/software-is-a-depreciating-asset-why-your-software-is-never-done)

## What is Volatility?

**Volatility** refers to the degree of uncertainty and change over the lifetime of a solution. It encompasses both internal factors, such as evolving requirements, and external influences, such as market shifts, customer demands, or integration with third-party systems.

{{% callout note %}}
Uncertainty is the most significant factor influencing the success of a project. It drives both over-engineering and the failure to meet expectations.
{{% /callout %}}

Anticipating change is difficult. Stakeholders often stuggle with future uncertainties, and without clear guidance, implementation teams will either spend excessive time creating costly, overengineered solutions or default to overly rigid, generic designs that fail to meet actual needs.

By exploring "what if" scenarios and applying structured techniques, teams can make better decisions on where flexibility is needed and where it isn’t.

### Examples of Volatility

Volatility, or change, manifests in various ways depending on the context of the project. Here are a few common examples:

- **Evolving Business Requirements:** A product team might initially prioritize one set of features, only to shift focus based on customer feedback or market trends. For example, a platform that starts as a B2C tool might later pivot to support B2B workflows, requiring major changes to permissions, reporting, and integrations.
- **Integration with External Systems:** A system reliant on third-party APIs or SaaS platforms might face frequent updates, deprecations, or vendor changes. For instance, a payment processing integration might require adapting to new compliance standards or API upgrades every year.
- **Regulatory or Compliance Changes:** In industries like healthcare or finance, new laws or regulations can force substantial redesigns, such as adding audit trails, encryption, or new data retention policies.
- **Scaling for Growth:** An e-commerce application initially designed for a small customer base might need to handle ten times the traffic during a holiday season, requiring changes to database design, caching strategies, or load balancing.

## Anticipating Change

Change is not inherently good or bad—it’s a reality of software development. The key to managing it lies in identifying areas where change is likely or uncertain. 

Identifying requires curiosity and active participation. Cross-functional groups must come together and have open-minded discussions. This collaborative curiosity often uncovers insights and sparks epiphanies, driven by diverse perspectives.

Every business faces unique challenges, yet certain themes tend to emerge consistently:

| **Area**                   | **Description**                                                                                           | **Impacts**                                                                                 |
|----------------------------|-----------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------|
| **Market Dynamics**         | Shifting competitive landscapes and rising customer expectations demand continuous adaptation.            | Necessitates frequent enhancements to outperform competitors and meet user demands.         |
| **Environmental Changes**   | Regulatory updates and evolving security threats necessitate proactive updates.                          | Failure to adapt can lead to compliance risks, legal exposure, and system vulnerabilities.  |
| **Organizational Needs** | Business growth, new workflows, and scaling demands reshape software requirements.                     | Drives the need for process optimization, scalability upgrades, and cost-effective solutions. |
| **Technological Advancements** | Emerging programming languages, frameworks, tools, and hardware innovations drive opportunities and challenges. | Requires updates to leverage efficiencies, maintain competitiveness, and prevent obsolescence. |
| **User-Centric Changes**     | User feedback, modern UI trends, and usability expectations highlight areas for improvement.              | Enhances customer satisfaction and system adoption through regular updates and redesigns.   |

Encouraging everyone to think about "what if" scenarios helps surface areas of volatility that might not otherwise be apparent. Here are some example questions that can guide this process:

| **Question**                                                   | **Reasoning**                                                                                     |
|----------------------------------------------------------------|---------------------------------------------------------------------------------------------------|
| What are the core goals of this solution?                    | Understanding the business’s top priorities can reveal where flexibility might be essential.      |
| What is most likely to change in the next 6 to 12 months?     | Identifies potential shifts in user needs, integrations, or scalability that could impact design. |
| What are the known unknowns?                               | Highlights areas of ambiguity or deferred decisions that could pose risks or opportunities.       |
| What external factors could impact this solution?            | Considers market trends, customer feedback, regulatory changes, or vendor dependencies.           |
| What would happen if this solution needed to double its capacity? | Uncovers architectural limitations or scalability requirements that need addressing.             |
| What happens if this solution needs to integrate with new tools or platforms? | Highlights potential design or compatibility concerns for future integrations.                    |
| What would happen if the budget or timeline were reduced significantly? | Assesses how constraints might shift priorities or require adaptability in delivering outcomes.    |

The key to success lies in embracing the shared responsibility between business and technology for identifying areas of change. Equally important is having a collaborative mindset when change arises—rather than assigning blame for why a solution falls short, teams should work together to understand what was overlooked and use those insights to better prepare for inevitable future changes.

### Communicating Change

Building for immediate needs prioritizes speed and simplicity, delivering results quickly. Future-proofing, on the other hand, aims to design solutions that evolve gracefully over time. Too much focus on the short-term can lead to expensive refactoring later, while over-indexing on future-proofing can delay time-to-market and overcomplicate the system.

To effectively communicate "what ifs" and the impacts of trade-offs it's critical to frame it in terms that resonate with the business. This involves translating technical details into tangible business outcomes:

- **Cost of Flexibility:** Explain how adding flexibility in a volatile area (e.g., building an extensible API) will increase initial development time but reduce costs and disruption when future changes are needed.
- **Impact of Rigidity:** If a solution is designed without accounting for volatility, highlight the risks, such as expensive refactoring, downtime, or delayed market response when changes inevitably arise.
- **Balancing Short-Term and Long-Term Goals:** Demonstrate how thoughtful investments in change management—like modular design or abstraction—can align with business timelines while avoiding technical debt.
- **Realistic Expectations for Change:** Frame volatility as an expected and manageable reality, emphasizing that flexibility requires trade-offs but reduces risk over the system’s lifetime. For example:
    - _“If we don’t account for the potential of pivoting to a B2B model, implementing those features later will cost 3x as much and delay delivery by 6 months.”_
    - _“Building in flexibility now adds 10% to development time but ensures we can handle third-party API changes without a full rewrite.”_

## Trade-Offs

Success requires balancing short-term goals with long-term sustainability, particularly when managing change. Decisions made today can influence flexibility, maintainability, and operational efficiency for years to come. Here are a few real world examples of volatility and possible trade-offs.

### Market Shift from B2B to B2C

Businesses sometimes expand from serving B2B customers to pursuing opportunities in the B2C market. While this shift can unlock significant growth, it introduces change that can ripple through the entire system design, particularly in security and permissions.

In a B2B context, workflows often rely on implied trust, where users are part of a trusted organization, and permissions structures are relatively simple—for example, distinguishing between "admin" and "regular user." However, a B2C model introduces a much broader and more dynamic user base, requiring more granular permissions and robust security measures to protect sensitive personal data.

Consider a SaaS company that has historically served corporate clients (B2B), offering employee management tools with a simple admin/user permission structure. Upon discovering strong demand from small businesses and freelancers (B2C), the company launched a version for individual users. However, without adapting the security model, personal data like billing details and usage histories would not be adequately protected. To mitigate these risks, the team has to overhaul the permissions system to support features like guest access, role-based permissions, and tighter controls over sensitive information.

- **Option 1 - Retain the Existing B2B Security Model:** Stick with the current design, keeping simplicity and reducing immediate development time. However, this approach risks exposing sensitive data or failing to meet the expectations of a diverse B2C audience, leading to reputational damage or regulatory issues.

- **Option 2 - Redesign the Security Model for B2C Needs:** Invest in a more sophisticated security and permissions framework to support the B2C use case. This ensures robust protection for personal data and better user experience but requires significant time, effort, and potentially re-engineering core workflows.

- **Option 3 - Implement Incremental Changes:** Gradually adapt the security model, focusing first on critical areas while maintaining parts of the original structure. This balances the need for immediate action with longer-term goals, but the hybrid nature might lead to inconsistencies or gaps in security during the transition.

Should the implementation team have foreseen this impending customer base shift? Would the increased complexity and development time required for pervasive permissioning throughout the application have been justified, or dismissed as over-engineering at the time? Did the business fail to anticipate this future market opportunity, neglecting to allocate funding early enough to make the system nimble and ready to capitalize on it quickly? 

### Multi-Tenancy (SaaS Example)

[Multi-tenancy](https://en.wikipedia.org/wiki/Multitenancy) is a fundamental architectural decision in SaaS platforms that significantly impacts scalability, operational costs, and security. As businesses grow and their user base diversifies, these decisions become even more critical, as they determine how effectively the system can evolve and handle new demands.

Consider a SaaS platform designed for small businesses, where the team initially chose a shared database model for its simplicity and cost-efficiency. As the platform gains traction, larger enterprise customers join, demanding more rigorous data isolation, customized features, and guaranteed performance. The original model starts to show strain, leading the team to evaluate new approaches.

- **Option 1 - Shared Database Model:** A single database serves all tenants, segregating data using identifiers. This approach is cost-effective and simpler to manage but comes with increased risks around data isolation and performance issues.
- **Option 2 - Database-Per-Tenant Model:** Each tenant has its own database, providing better data isolation and customization options. However, this increases operational complexity and costs.
- **Option 3 - Hybrid Approach:** A hybrid model combines aspects of both, such as grouping smaller tenants into a shared database while providing high-value tenants with dedicated databases.

Could the team have anticipated the need for enterprise-level features during the early stages of development? Would implementing a more flexible, hybrid architecture from the outset have been seen as forward-thinking or over-engineering? Did business leaders understand the importance to invest in scaling infrastructure, or lead the team to reactive changes instead of proactive planning? 

### Workflow Change and Database Access Patterns

Changes in business workflows can introduce significant volatility into the design of underlying technologies, often requiring reevaluation of earlier decisions. A common example involves databases, where changes in access patterns can drastically impact performance and cost.

Consider, a logistics company initially using DynamoDB, an extremely fast yet rigid database, for quick point lookups, such as retrieving the status of individual shipments. Over time, the company introduced analytics features allowing customers to view trends across all shipments. This required broader queries that scanned the entire database, causing costs to skyrocket and performance to degrade. The team faced a decision: stick with DynamoDB and optimize queries, migrate to a relational database like PostgreSQL, or use both databases for their respective strengths.

- **Option 1 - Shared Database Model:** A single database for all tenants segregates data using tenant identifiers. This is cost-effective and easier to implement initially but increases risks around data isolation and scalability as the tenant base grows.
- **Option 2 - Database-Per-Tenant Model:** Each tenant has its own database, offering strong isolation and tailored performance but introducing significant operational complexity and higher costs.
- **Option 3 - Hybrid Approach:** A hybrid model involves using shared databases for smaller tenants while dedicating separate databases to high-value or demanding clients. This balances cost and scalability but adds complexity to architecture and operational management.

Could the team have anticipated this shift in workflow when initially selecting the database? Was the focus on immediate cost-efficiency short-sighted, or was it the right choice based on the information available at the time? Did business stakeholders clearly communicate the potential for evolving analytics needs, or did the technology team miss early indicators of future requirements? 

## Impact

Predicting change is inherently difficult. High-level trends (e.g., market shifts) are often discussed, but anticipating how those changes cascade into technical decisions—from feature adaptability to data migration strategies—requires both foresight and agility.

Volatility often acts as a headwind for other F6 Foundations, as uncertainty complicates planning, execution, and maintenance. Here’s how it interacts:

| **Foundation**                                                   | **Impact**                                                                                     |
|----------------------------------------------------------------|---------------------------------------------------------------------------------------------------|
| Capability | High volatility can make it harder to achieve feature-rich, reliable solutions, as requirements may shift during development. |
| Dependency | Frequent change strains the entire underlying eco-system, increasing risk across the board. |
| Security | Adapting to volatility often introduces new attack surfaces or vulnerabilities, requiring constant vigilance. |
| Resilience | Unanticipated changes can undermine a system's design and stability, increasing the likelihood of failure or downtime. |
| Investment | Higher uncertainty often means higher costs, as adapting to change requires more resources. |

Tailwinds? Volatility rarely makes other foundations easier to address. The closest "benefit" is that embracing volatility forces teams to prioritize adaptability, which can create solutions better suited to long-term evolution.