---
title: Getting Started
weight: 1
sidebar:
  open: true
---

## Introduction

The **F6 Framework** provides a structured lens to evaluate and plan software projects, acting as a communication bridge between stakeholders and implementation teams. Its primary audience includes:

- **Stakeholders (C-Suite, business owners):** Helping them understand the strategic "knobs" they can turn and the impact of their decisions.
- **Implementation teams (BAs, PMs, developers):** Offering a shared language to translate technical considerations into business-relevant terms.

F6 does not replace methodologies like Agile, Scrum, or Lean. Instead, it layers onto these processes, enhancing them by addressing key trade-offs across six foundational aspects:

| **Foundation** | **Description**                                            | **Example**                                                                                     |
|-----------------|------------------------------------------------------------|-------------------------------------------------------------------------------------------------|
| **Capability** | Defines functional requirements.                           | "What should the system do?" A feature-rich e-commerce platform requires well-defined workflows and functionality. |
| **Volatility** | Accounts for change over time.                             | "What might shift, and how do we adapt?" In a startup, rapidly changing market demands may necessitate flexible architecture. |
| **Dependency** | Evaluates external reliance.                               | "What do we build, buy, or integrate?" Choosing a third-party payment gateway can reduce development effort but introduce long-term risks. |
| **Security**   | Safeguards data and systems.                               | "How do we protect assets?" Compliance with regulations like GDPR or SOC 2 is crucial for systems handling sensitive user data. |
| **Resiliency** | Prepares for failures.                                     | "What happens when things go wrong?" Ensuring uptime during server outages via redundancy strategies. |
| **Investment** | Allocates resources.                                       | "What’s the time and cost?" Balancing budget constraints with project goals.                     |

Decisions in one foundation often affect others. For instance:

- A system with high **Capability** (many features and workflows) and high **Volatility** (frequent changes) faces highly uncertain future demands. Without sufficient **Investment** to accommodate these changes, the system risks diminished quality of capabilities and compromised **Security** effectiveness over its lifespan.
- A system with high external **Dependency** (tools and products), while benefiting from faster speed to market and less early **Investement**, may become vulnerable if those integrations fail, reducing **Resiliency** (uptime and quality-of-service).

The F6 Framework’s strength lies in illuminating these interconnections, enabling informed, intentional decision-making.

## F6 Discovery Process

F6 enhances the most critical phase of any project—the beginning. This is the time when stakeholders are working to articulate their needs but often lack clarity about what they will receive in return. The F6 Discovery Process addresses this gap, offering an enhanced approach to requirements gathering and goal-setting that ensures alignment and reduces ambiguity.

The **F6 Discovery Process** is a structured approach for uncovering critical details about each of the six foundations during the project formative stages. Its purpose is to identify foundational priorities, highlight potential risks, and evaluate trade-offs early, paving the way for informed decision-making and clear expectations.

- **Volatility**: "What assumptions might change?"
- **Capability**: "What are the must-have features?"
- **Dependency**: "What third-party tools are required?"
- **Security**: "What compliance requirements apply?"
- **Resiliency**: "What happens if X fails?"
- **Investment**: "What’s the timeline and budget?"

This process ensures alignment and clarity, setting the stage for informed decision-making.

## Gradient of Complexity

Each foundation has a unique gradient of complexity—some are more intuitive, while others require deeper thought to fully grasp. Within each foundation, there are levels of understanding that build on one another.

- **Straightforward Foundations:**
    - **Capability:** At its core, defining functional requirements is straightforward: "What does the system need to do?" However, complexity arises in balancing user expectations, feature prioritization, and scalability.
    - **Investment:** High-level considerations such as budget and timeline are easy to grasp, but challenges emerge when stakeholders must evaluate long-term costs versus short-term gains.
- **Moderate Complexity:**
    - **Dependency:** High-level decisions like "build vs. buy" are easy to comprehend, but understanding the implications of integrating software frameworks, libraries, and third-party tools requires technical expertise. Managing versioning, support lifecycles, and external updates adds depth.
    - **Security:** Compliance frameworks (e.g., GDPR, SOC 2) are broadly understood, but granular aspects such as roles, permissions, and encryption mechanisms demand specialized knowledge.
- **Challenging Foundations:**
    - **Resiliency:** Stakeholders often overlook "rainy day" scenarios. While high-level ideas like redundancy and backups are easy to explain, crafting fault-tolerant systems involves complex trade-offs in architecture, monitoring, and recovery strategies.
    - **Volatility:** Predicting change is inherently difficult. High-level trends (e.g., market shifts) are often discussed, but anticipating how those changes cascade into technical decisions—from feature adaptability to data migration strategies—requires both foresight and agility.

Straightforward foundations like Capability and Investment provide immediate clarity and are natural starting points for discussion. However, abstract foundations like Volatility and Resiliency carry the most long-term impact. For example:

- Ignoring **Volatility** may result in rigid systems that are costly to adapt as requirements shift.
- Underestimating **Resiliency** can lead to catastrophic failures in production environments.

## Next Steps

Understanding the F6 Framework begins with recognizing the "knobs" available to influence project outcomes. Each decision related to the foundational aspects directly shapes the project's trajectory. For example, stakeholders can start by reflecting on high-level questions to clarify their priorities and constraints, such as:

- What do we want the system to achieve? (**Capability**)
- What future changes are likely? (**Volatility**)
- What’s our risk tolerance, both in terms of potential failures (**Resiliency**) and security threats (**Security**)?

These questions set the stage for effective collaboration. Stakeholders gain a clearer picture of the trade-offs inherent in their decisions, while implementation teams can translate these insights into actionable strategies. For instance, when considering system architecture, implementation teams might explain trade-offs like this:

- "To enable rapid feature updates (**Volatility**), we’ll need to prioritize a modular architecture, which increases both up-front **Investment** and ongoing maintenance costs."

By framing decisions in terms of their impact on the foundational priorities, teams can have productive conversations that align technical strategies with stakeholder expectations. 

Next, explore the in-depth material on each of the six foundations. Once familiar with these concepts, proceed to the **F6 Discovery Process** section to learn how to apply this framework to uncover priorities, risks, and trade-offs in the early stages of your project.

{{< cards >}}
  {{< card url="/docs/foundations/volatility/" title="Volatility" icon="bolt" >}}
  {{< card url="/docs/foundations/capability/" title="Capability" icon="puzzle-piece" >}}
  {{< card url="/docs/foundations/dependency/" title="Dependency" icon="link" >}}
  {{< card url="/docs/foundations/security/" title="Security" icon="shield-check" >}}
  {{< card url="/docs/foundations/resiliency/" title="Resiliency" icon="server" >}}
  {{< card url="/docs/foundations/investment/" title="Investment" icon="chart-pie" >}}
{{< /cards >}}
