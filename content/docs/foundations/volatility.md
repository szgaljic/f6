---
title: Volatility
weight: 1
---

## Overview

_Navigating change with precision and purpose._

It’s been said that the only constant in life is change. Software is no different; it’s a depreciating asset that must be updated, altered, and maintained to stay effective.

The **Volatility** foundation emphasizes the balance between rapid progress and thoughtful precision. It acknowledges the duality of software development: the need to deliver impactful results quickly while ensuring those results are built with the care and precision required for their intended lifetime. 

This aspect recognizes a sliding scale: are you building for the "here and now," accepting the potential for more significant rewrites later, or investing in a foundation that supports seamless evolution over time? Both approaches have their place, depending on the system’s goals, constraints, and maturity. [Software is never truly "done," and every decision made today influences how effectively it can evolve tomorrow.](https://insights.jahnelgroup.com/software-is-a-depreciating-asset-why-your-software-is-never-done)

Operating with intention involves trade-offs, as acting without thoughtful deliberation or clear purpose can create misalignment between stakeholders and the tech team. 

## What Is Volatility?

Volatility in software refers to the degree of uncertainty and change expected over the lifecycle of a system. It encompasses both internal factors, such as evolving requirements, and external influences, such as market shifts, customer demands, or integration with third-party systems.

To align stakeholders and developers, the concept of volatility serves as a translation vocabulary—a way to articulate where change is expected, and how it will impact the system. Developers must understand that business needs often evolve quickly, but stakeholders must also appreciate that without clear communication, engineers are left to make assumptions about what parts of the system will remain stable and what will need to adapt.

### Trade-Offs

Software solutions are often built on a sliding scale between delivering for the “here and now” and planning for the “what ifs” of the future. Building for immediate needs prioritizes speed and simplicity, delivering results quickly. However, such solutions may become brittle and costly to change as volatility increases.

Future-proofing, on the other hand, aims to design systems that evolve gracefully over time. This approach anticipates potential changes through strategies like modular architectures, abstractions, and extensibility, but it comes with a cost—higher complexity, longer development timelines, and increased effort to manage edge cases that may never materialize.

The challenge lies in striking the right balance. Too much focus on the short-term can lead to expensive refactoring later, while over-indexing on future-proofing can delay time-to-market and overcomplicate the system.

## Anticipating Change

Volatility is not inherently good or bad—it’s a reality of software development. The key to managing it lies in identifying areas where change is likely or uncertain. This starts with curiosity and open conversations between stakeholders and developers. Stakeholders may not always know exactly what will change, but exploring potential areas of volatility allows teams to prepare for the future while delivering in the present.

Without these conversations, engineers are left guessing where volatility lies, often defaulting to generic solutions or over-engineered designs that don’t align with actual business needs. When volatility is identified, teams can focus their efforts on the parts of the system most likely to evolve, creating a more thoughtful and balanced solution.

### Examples of Volatility

Volatility manifests in various ways depending on the context of the project. Here are a few common examples:

- **Evolving Business Requirements:** A product team might initially prioritize one set of features, only to shift focus based on customer feedback or market trends. For example, a platform that starts as a B2C tool might later pivot to support B2B workflows, requiring major changes to permissions, reporting, and integrations.
- **Integration with External Systems:** A system reliant on third-party APIs or SaaS platforms might face frequent updates, deprecations, or vendor changes. For instance, a payment processing integration might require adapting to new compliance standards or API upgrades every year.
- **Regulatory or Compliance Changes:** In industries like healthcare or finance, new laws or regulations can force substantial redesigns, such as adding audit trails, encryption, or new data retention policies.
- **Scaling for Growth:** An e-commerce application initially designed for a small customer base might need to handle ten times the traffic during a holiday season, requiring changes to database design, caching strategies, or load balancing.

### Identifiy areas of Volatility 

Identifying volatility requires structured inquiry, curiosity, and effective techniques to surface areas of potential change. Stakeholders and engineers must engage in collaborative activities to tease out workflows, user interactions, feature sets, and system events. These industry-standard techniques can help:

- **Event Storming:** A collaborative workshop technique for mapping out system events, workflows, and domain boundaries, enabling teams to visualize where changes are likely to occur.
- **Story Mapping:** A visual method to break down user journeys and feature sets, focusing on user needs and identifying areas of uncertainty or variability.
- **Journey Mapping:** Mapping the end-to-end customer experience to uncover key interactions and dependencies, especially useful in customer-facing systems.
- **Mind Mapping:** Brainstorming and organizing ideas around workflows or features to identify relationships and areas that may evolve.
- **Domain-Driven Design (DDD):** Identifying bounded contexts and domains to align software architecture with business operations, revealing areas of volatility tied to domain boundaries.

Engaging in open-ended conversations are also great ways to surface potential areas of change. Here are some example questions that can guide this process:

- **What are the core goals of this system?**
    - Understanding the business’s top priorities can highlight where flexibility might be needed to achieve them.
- **What is most likely to change in the next 6-12 months?**
    - For example, will user needs evolve, will integrations shift, or will the system scale significantly?
- **What are the known unknowns?**
    - Identify areas where requirements are unclear, or where decisions are being deferred.
- **What external factors could impact this system?**
    - Consider market conditions, customer feedback, regulations, or vendor updates.
- **What would happen if this system needed to double its capacity?**
    - This question often uncovers architectural limitations or areas needing flexibility.

Encouraging stakeholders to think about "what if" scenarios helps surface areas of volatility that might not otherwise be apparent. These conversations can also prompt the team to prioritize clarity around areas of uncertainty, ensuring assumptions are well-understood and documented.

## Communicating Volatility

Once areas of volatility are identified, it’s crucial to communicate their implications in terms that resonate with the business. This involves translating technical trade-offs into tangible outcomes:

- **Cost of Flexibility:** Explain how adding flexibility in a volatile area (e.g., building an extensible API) will increase initial development time but reduce costs and disruption when future changes are needed.
- **Impact of Rigidity:** If a system is designed without accounting for volatility, highlight the risks, such as expensive refactoring, downtime, or delayed market response when changes inevitably arise.
- **Balancing Short-Term and Long-Term Goals:** Demonstrate how thoughtful investments in volatility management—like modular design or abstraction—can align with business timelines while avoiding technical debt.
- **Realistic Expectations for Change:** Frame volatility as an expected and manageable reality, emphasizing that flexibility requires trade-offs but reduces risk over the system’s lifetime. For example:
    - _“If we don’t account for the potential of pivoting to a B2B model, implementing those features later will cost 3x as much and delay delivery by 6 months.”_
    - _“Building in flexibility now adds 10% to development time but ensures we can handle third-party API changes without a full rewrite.”_

## Why This Matters

Identifying volatility early allows teams to design systems that align with the business’s current goals while remaining adaptable for the future. By fostering curiosity, asking the right questions, and communicating impacts clearly, volatility becomes a shared responsibility—one that stakeholders and developers navigate together.

This alignment helps ensure that volatility doesn’t derail the project but instead becomes an opportunity for collaboration, foresight, and ultimately, success.