---
title: Getting Started
weight: 1
sidebar:
  open: true
---

## Introduction

The **F6 Framework** provides a structured lens to evaluate and plan technology projects, acting as a communication bridge between business leaders and implementation teams. Its primary audience includes:

- **Stakeholders (C-Suite, business leaders):** Helping them understand the strategic "levers" they can pull in their projects and the impacts of their decisions.
- **Implementation teams (Analysts, Project Managers, Engineers, etc):** Offering a shared language to translate technical considerations into business-relevant terms.

F6 does not replace methodologies like Agile, Scrum, or Lean. Instead, it layers onto these processes, enhancing them by addressing key trade-offs across six foundational aspects:

| **Foundation** | **Description**                             | **Example**                                                                                     |
|-----------------|--------------------------------------------|-------------------------------------------------------------------------------------------------|
| **Features** | Defines functional requirements.              | "What should the solution do?" A feature-rich e-commerce platform requires well-defined workflows and functionality. |
| **Dependencies** | Evaluates external reliance.              | "What do we build, buy, or integrate?" Choosing a third-party payment gateway can reduce development effort but introduce long-term risks. |
| **Security**   | Safeguards data and systems.                | "How do we protect assets?" Compliance with regulations like GDPR or SOC 2 is crucial for systems handling sensitive user data. |
| **Risk** | Accounts for uncertainty over time.                 | "What risks might we face, and how do we manage them?" In a startup, rapidly changing market demands may necessitate flexible architecture. |
| **Optimizations** | Focuses on efficiency and performance.   | "How can we maximize output and minimize waste?" Implementing automation strategies to reduce downtime and improve quality. |
| **Investments** | Allocates resources.                       | "What’s the time and cost?" Balancing budget constraints with project goals.                     |

Decisions in one foundation often affect others, for example:

- A solution with many **Features** (functions and workflows) and many **Risk** (frequent changes) faces highly uncertain future demands. Without sufficient **Investment** to accommodate these changes, the solution risks diminished quality of capabilities and compromised **Security** effectiveness over its lifespan.
- A solution heavily reliant on external **Dependencies** (tools and products) may offer faster speed to market but can become vulnerable if those integrations fail. Without adequate **Investment** in **Optimizations**, this could lead to decreased uptime and a decline in quality of service.

The F6 Framework’s strength lies in illuminating these interconnections, enabling informed, intentional decision-making.

## F6 Discovery

F6 enhances the most critical phase of any project—the beginning. This is the time when stakeholders are working to articulate their needs but often lack clarity about what they will receive in return. The **F6 Discovery Process** addresses this gap, offering an enhanced approach to requirements gathering and goal-setting that ensures alignment and reduces ambiguity.

It is a structured approach for uncovering critical details about each of the six foundations during the project formative stages. Its purpose is to identify foundational priorities, highlight potential risks, and evaluate trade-offs early, paving the way for informed decision-making and clear expectations.

- **Features**: "What are the must-have functions and workflows?"
- **Dependencies**: "What should we own vs. rely on?"
- **Security**: "What compliance requirements apply?"
- **Risk**: "What assumptions might change?"
- **Optimizations**: "What do we focus perfecting?"
- **Investment**: "What’s the timeline and budget?"

## Gradient of Complexity

Each foundation has a unique gradient of complexity—some are more intuitive, while others require deeper thought to fully grasp. Within each foundation, there are levels of understanding that build on one another.

- **Straightforward Foundations:**
    - **Features:** At its core, defining functional requirements is straightforward: "What does the solution need to do?" However, complexity arises in balancing user expectations, feature prioritization, and feature completeness.
    - **Investments:** High-level considerations such as budget and timeline are easy to grasp, but challenges emerge when stakeholders must evaluate long-term costs versus short-term gains.
- **Moderate Complexity:**
    - **Dependencies:** High-level decisions like "build vs. buy" are easy to comprehend, but understanding the impact of integrating low-level software components and third-party tools requires technical expertise. Managing versioning, support lifecycles, and external updates adds depth.
    - **Security:** Compliance frameworks (e.g., GDPR, SOC 2) are broadly understood, but granular aspects such as roles, permissions, and encryption mechanisms demand specialized knowledge.
- **Challenging Foundations:**
    - **Risk:** Predicting change is inherently difficult. High-level trends (e.g., market shifts) are often discussed, but anticipating how those changes cascade into technical decisions—from feature adaptability to data migration strategies—requires both foresight and agility.
    - **Optimizations:** Stakeholders often focus end-user features and "happy day" scenarios. While high-level ideas like automation, redundancy and backups are easy to explain, orchestrating automation workflows and  crafting fault-tolerant systems involves complex low-level trade-offs in architecture, monitoring, and recovery strategies.

Straightforward foundations like **Features** and **Investment** provide immediate clarity and are natural starting points for discussion. However, abstract foundations like **Risk** and **Optimizations** carry the most long-term impact. For example:

- Ignoring **Risk** may result in rigid solutions that are costly to adapt as requirements shift.
- Underestimating **Optimizations** can lead to catastrophic failures in production environments—impacting businesses when they least expect it.

## Trade-offs

Trade-offs are an inherent part of software development, where every decision involves balancing competing priorities. These decisions occur at both high and low levels, influencing everything from system architecture to individual features. High-level trade-offs, such as choosing a fast/simple design for a feature versus loger-term/complex design, are often visible and easier to grasp. However, low-level trade-offs, like selecting a specific software component, can have cascading impacts that require technical expertise to fully understand.

For **stakeholders and business leaders**, it’s on you to be curious and attentive to these trade-offs. Ask questions, probe for clarity, and seek to understand the implications of decisions being made. Doing so helps uncover potential risks and ensures alignment with broader goals.

For **implementation team members**, remember that you are not alone in making these trade-offs. It is your responsibility to translate the technical nuances and potential impacts of these decisions into terms that stakeholders can understand. By bridging this gap, you help improve collaboration and ensure that trade-offs are intentional and aligned with the project’s objectives.

## Next Steps

Understanding the F6 Framework begins with recognizing the levers available to influence project outcomes. Each foundation provides a means to discuss these levers, emphasizing how each decision imapacts the project's trajectory.

Stakeholders gain a clearer understanding of the trade-offs inherent in their decisions, while implementation teams can turn these insights into actionable strategies. For instance, when evaluating system architecture, implementation teams might explain trade-offs like this:

- "To enable rapid **Feature** updates, we’ll need to prioritize a modular architecture to reduce refactoring **Risk**, which increases both up-front **Investment** and ongoing maintenance costs."

By framing decisions in terms of their impact on the foundational priorities, teams can have productive conversations that align technical strategies with stakeholder expectations. 

Next, explore the in-depth material on each of the six foundations. Once familiar with these concepts, proceed to the [F6 Discovery Process](/docs/f6-discovery/) section to learn how to apply this framework to uncover priorities, risks, and trade-offs in the early stages of your project.

{{< cards >}}
  {{< card url="/docs/foundations/features/" title="Features" icon="puzzle-piece" >}}
  {{< card url="/docs/foundations/dependencies/" title="Dependencies" icon="link" >}}
  {{< card url="/docs/foundations/security/" title="Security" icon="shield-check" >}}
  {{< card url="/docs/foundations/risk/" title="Risk" icon="bolt" >}}  
  {{< card url="/docs/foundations/optimizations/" title="Optimizations" icon="server" >}}
  {{< card url="/docs/foundations/investments/" title="Investments" icon="chart-pie" >}}
{{< /cards >}}