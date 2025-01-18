---
title: Risk
weight: 4
---

## Overview

_"What risks might we face, and how do we manage them?"_

In technology, risk is inevitable—whether it's tied to changing requirements, shifting market demands, or technical complexities. A solution that once fit perfectly can quickly become outdated. Adapting to these shifts requires viewing technology as a depreciating asset—one that must be continually updated, refined, and maintained to remain effective.

The **Risk** foundation emphasizes the balance between speed and sustainability. It explores the duality of delivering impactful results quickly while ensuring those results are built with the foresight and precision needed to support long-term goals.

This foundation highlights a critical decision-making spectrum: are you building for the "here and now," accepting the likelihood of larger adjustments later, or are you investing in a foundation that mitigates risk and allows for seamless evolution over time? Both approaches have their place, depending on the goals, constraints, and maturity of the solution. Every decision made today shapes how effectively a system can adapt and thrive tomorrow.

> [Software is never truly "done," and every decision made today influences how effectively it can evolve tomorrow.](https://insights.jahnelgroup.com/software-is-a-depreciating-asset-why-your-software-is-never-done)

## What is Risk?

**Risk** refers to the potential for unexpected outcomes or challenges over the lifetime of a solution. These risks can stem from internal factors, such as shifting priorities or technical decisions, as well as external forces, like market disruptions, regulatory changes, or dependencies on third-party systems. 

Identifying risks and anticipating change is difficult. Stakeholders often struggle to balance future uncertainties, prioritize effectively, and weigh risk mitigation against feature development. Without clear guidance, implementation teams may overengineer costly solutions or create rigid designs that fail to adapt or meet real needs.

{{% callout note %}}
**Uncertainty** is the most significant factor influencing a successful outcome. It drives both over-engineering and the failure to meet expectations.
{{% /callout %}}

By exploring "what if" scenarios and applying structured techniques, teams can make better decisions on where flexibility is needed and where it isn’t.

### Examples of Risk

Here are specific scenarios that illustrate different types of risks:

- **Evolving Business Requirements:** A product team might initially prioritize one set of features, only to shift focus based on customer feedback or market trends. For example, a platform that starts as a B2C tool might later pivot to support B2B workflows, requiring major changes to permissions, reporting, and integrations.
- **Integration with External Systems:** A system reliant on third-party APIs or SaaS platforms might face frequent updates, deprecations, or vendor changes. For instance, a payment processing integration might require adapting to new compliance standards or API upgrades every year.
- **Regulatory or Compliance Changes:** In industries like healthcare or finance, new laws or regulations can force substantial redesigns, such as adding audit trails, encryption, or new data retention policies.
- **Scaling for Growth:** An e-commerce application initially designed for a small customer base might need to handle ten times the traffic during a holiday season, requiring changes to database design, caching strategies, or load balancing.

## Anticipating Risk

Change is neither inherently good nor bad—it's the unpredictability of it that often causes the greatest challenges.

To be anticipate it requires curiosity and active participation. Cross-functional teams must come together and have open-minded discussions. Collaborative conversations often uncover insights and sparks epiphanies, driven by diverse perspectives.

Every business faces unique challenges, yet certain themes tend to emerge consistently: 

| **Category**         | **Risk**                                                                                              | **Example**                                                                                       |
|----------------------|------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------|
| **Strategic Risks**   | **Is our vision clear and understood?** Misalignment between the business strategy and technical solutions, leading to inefficiencies or missed opportunities. | A SaaS company focuses solely on enterprise clients, overlooking demand from small businesses, missing a key growth opportunity. |
| **Market Dynamics**   | **Are we aligned with market expectations?** Shifting competitive landscapes, changing customer expectations, or feedback that requires adaptation. | An e-commerce platform is slow to adopt same-day delivery, losing customers to more agile competitors. |
| **Regulatory Risks**  | **Are we tracking industry compliance trends?** Compliance with new laws, regulations, or standards that require redesigns or updates.              | A healthcare app must meet new patient privacy laws, adding encryption and audit trails to avoid fines or legal exposure. |
| **Operational Risks** | **Can we execute and deliver on our ideas?** Business growth or inefficiencies in day-to-day processes, lack of automation, or poor alignment between teams.         | A manual deployment process causes downtime during peak business periods, reducing customer trust and revenue. |
| **Technical Risks**   | **Do we have the know-how, expertise and means to do so?** Dependence on tools, APIs, or systems that may not scale, and architectural decisions or delays in adopting emerging technologies and frameworks, can hinder adaptability, competitiveness, and team productivity.                  | A company struggles to integrate a cutting-edge framework, delaying a critical product launch. |

Encouraging everyone to think about "what if" scenarios along these categories helps surface areas of risk that might not otherwise be apparent. Here are some additional example questions that can guide this process:

| **Question**                                                   | **Reasoning**                                                                                     |
|----------------------------------------------------------------|---------------------------------------------------------------------------------------------------|
| What are the core goals of this solution?                    | Understanding the business’s top priorities can reveal where flexibility might be essential.      |
| What is most likely to change in the next 6 to 12 months?     | Identifies potential shifts in user needs, integrations, or scalability that could impact design. |
| What are the known unknowns?                               | Highlights areas of ambiguity or deferred decisions that could pose risks or opportunities.       |
| What external factors could impact this solution?            | Considers market trends, customer feedback, regulatory changes, or vendor dependencies.           |
| What would happen if this solution needed to double its capacity? | Uncovers architectural limitations or scalability requirements that need addressing.             |
| What happens if this solution needs to integrate with new tools or platforms? | Highlights potential design or compatibility concerns for future integrations.                    |
| What would happen if the budget or timeline were reduced significantly? | Assesses how constraints might shift priorities or require adaptability in delivering outcomes.    |

The key to success lies in embracing the shared responsibility between business and technology for identifying areas of interest.

## Communicating Risk

To effectively communicate risk it helps to frame it in terms that resonate with the business.

**Strategic Alignment of Risk:** Highlight how risks align or conflict with the business’s strategic objectives. This includes evaluating whether current decisions support long-term growth, competitive positioning, or market differentiation.
- _“Delaying entry into the B2C market reduces immediate costs but risks losing market share to competitors already targeting that segment.”_

**Market Sensitivity to Risk:** Articulate risks tied to customer expectations, market trends, and competitive pressures. Emphasize the cost of missed opportunities or negative customer experiences.
- _“Delaying a redesign of the outdated user interface risks losing X% of users annually to competitors with more modern designs.”_

**Regulatory and Compliance Risk:** Frame regulatory risks in terms of compliance costs, legal exposure, and reputational harm. Show how proactive management reduces potential penalties and ensures business continuity.
- _“Adapting our data handling practices to meet new privacy regulations will cost $Y upfront but avoids potential fines of $Z.”_

**Operational Impact of Risk:** Explain how risks affect day-to-day processes, including team workflows, resource allocation, and system reliability. Operational risks often have compounding effects if not addressed early.
- _“Continuing manual deployments saves time now, but it increases the risk of downtime during peak periods, potentially costing $X per incident.”_

**Technical Flexibility and Scalability Risks:** Communicate the risks of technical decisions, such as choosing rigid systems, underestimating scalability needs, or adopting immature technologies.
- _“Using this database solution works for our current scale, but if demand doubles, it may require costly reengineering.”_

## Foundational Impacts

Risk acts as clear a headwind for other F6 Foundations, as uncertainty complicates planning, execution, and maintenance. Here’s how it interacts:

| **Foundation**                                                   | **Impact of Risk**                                                                                     |
|----------------------------------------------------------------|---------------------------------------------------------------------------------------------------|
| Capability | High risk can make it harder to achieve feature-rich, reliable solutions, as requirements may shift during development. |
| Dependency | Frequent change strains the entire underlying eco-system, increasing risk across the board. |
| Security | Risk often introduces new attack surfaces or vulnerabilities, requiring constant vigilance. |
| Resilience | Unanticipated changes can undermine a system's design and stability, increasing the likelihood of failure or downtime. |
| Investment | Higher uncertainty often means higher costs, as adapting to change requires more resources. |

Tailwinds? Risk rarely makes other foundations easier to address. The closest "benefit" is that embracing risk forces teams to prioritize adaptability, which can create solutions better suited to long-term evolution.

## Trade-Offs

Success requires balancing short-term goals with long-term sustainability, particularly when managing change. Decisions made today can influence flexibility, maintainability, and operational efficiency for years to come. Here are a few real world examples of risk and possible trade-offs.

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

Changes in business workflows can introduce significant risk into the design of underlying technologies, often requiring reevaluation of earlier decisions. A common example involves databases, where changes in access patterns can drastically impact performance and cost.

Consider, a logistics company initially using DynamoDB, an extremely fast yet rigid database, for quick point lookups, such as retrieving the status of individual shipments. Over time, the company introduced analytics features allowing customers to view trends across all shipments. This required broader queries that scanned the entire database, causing costs to skyrocket and performance to degrade. The team faced a decision: stick with DynamoDB and optimize queries, migrate to a relational database like PostgreSQL, or use both databases for their respective strengths.

- **Option 1 - Shared Database Model:** A single database for all tenants segregates data using tenant identifiers. This is cost-effective and easier to implement initially but increases risks around data isolation and scalability as the tenant base grows.
- **Option 2 - Database-Per-Tenant Model:** Each tenant has its own database, offering strong isolation and tailored performance but introducing significant operational complexity and higher costs.
- **Option 3 - Hybrid Approach:** A hybrid model involves using shared databases for smaller tenants while dedicating separate databases to high-value or demanding clients. This balances cost and scalability but adds complexity to architecture and operational management.

Could the team have anticipated this shift in workflow when initially selecting the database? Was the focus on immediate cost-efficiency short-sighted, or was it the right choice based on the information available at the time? Did business stakeholders clearly communicate the potential for evolving analytics needs, or did the technology team miss early indicators of future requirements? 

## Horizon Thinking

In technology solutions, the tension between short-term and long-term thinking plays out daily. Most projects begin with the push to achieve a Minimum Viable Product (MVP)—the fastest way to get to market, win customers, and learn what the market has to say about the offering. While this approach is essential for agility, it often exposes a critical communication gap between stakeholders and implementation teams.

This gap leads to three common scenarios, each with unique challenges and lessons. 

{{% callout note %}}
Each of these scenarios underscores the importance of clear, ongoing communication and collaboration between stakeholders and implementation teams. The key takeway—whether you pay the cost upfront or later, **the goal is to avoid surprises**. Success comes from aligning on a shared vision, understanding trade-offs, and making intentional decisions together.
{{% /callout %}}

### Unexpected Refactoring

A stakeholder requests a small MVP with the understanding that it can grow incrementally over time. They envision each new feature adding small impacts, seamlessly building on the initial product. But then, out of nowhere—the technical team announces that the architecture can no longer handle the additional features. Everything needs to be refactored, causing delays and skyrocketing costs.

<h4>Why It Happens:</h4>

Systems are built with assumptions in mind. If those assumptions—often based on incomplete or omitted information—prove incorrect, the entire architecture may need to change. Sometimes stakeholders omit critical details to save time or reduce costs, believing these details won’t matter yet. Other times, they simply don’t realize the relevance of those details.

<h4>How to Avoid It:</h4>

Stakeholders must communicate clearly and proactively about what they believe to be true and stable until specific milestones, such as the next six months, onboarding a major customer, or securing funding. They must also critically assess what features or capabilities they will—and will not—get within those milestones to avoid surprises down the road.

### Overengineered Solutions

A stakeholder provides vague or minimal details, perhaps due to time constraints, a lack of experience with technology solutions, or insufficient involvement and curiosity. Eager to anticipate future needs, the implementation team creates an elaborate, overly complex solution for a problem that doesn’t yet exist—or may never exist. Time and money are wasted, and the stakeholder grows frustrated as deadlines slip and no tangible product emerges.

<h4>Why It Happens:</h4>

Without clear direction, implementation teams may overcompensate by planning for hypothetical scenarios. While well-intentioned, these efforts often solve problems that are far in the future or unlikely to occur, diverting resources from immediate priorities.

<h4>How to Avoid It:</h4>

Stakeholders must communicate a clear vision of what is needed at each milestone, while also offering insights into long-term business goals. Collaboration is key: when technical teams explain the foundational groundwork required for future features, stakeholders must weigh the cost of doing it now versus incurring larger costs through future refactoring. Experienced stakeholders understand that delaying groundwork to validate the product is often a strategic choice, while inexperienced ones may be caught off guard when future costs arise.

### Balanced Collaboration

In the ideal case, stakeholders and implementation teams achieve alignment through shared curiosity, collaboration, and mutual understanding. The stakeholder is actively involved, learning enough about the technology to make informed decisions. The implementation team is equally engaged, learning enough about the business to understand its drivers and priorities. Together, they strike a balance between delivering an MVP and laying the groundwork for future needs.

<h4>Why It Works:</h4>

This approach is grounded in trust and transparency. Stakeholders and implementation teams recognize the shared goal of delivering a valuable product while managing risk and cost. By staying engaged and maintaining open communication, they avoid the pitfalls of both underplanning and overengineering.

- **Stakeholders** should remain curious and involved, asking questions to understand technical decisions and how they align with business goals.
- **Implementation teams** should prioritize understanding the “why” behind business drivers, ensuring their solutions align with the broader vision.

## Why This Matters

The key question of risk is: “What might shift, and how do we adapt?” While predicting the future is impossible, asking “what-if” helps uncover potential changes and align expectations. By exploring these possibilities, teams can strategically focus effort on areas most likely to evolve.

Success in navigating risk requires shared horizon thinking, where stakeholders and implementation teams work collaboratively to anticipate, communicate, and address potential shifts. This alignment ensures that resources are applied thoughtfully, enabling systems to adapt and thrive in an ever-changing landscape.