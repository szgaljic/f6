---
linkTitle: Documentation
title: The F6 Framework
---

## Introduction

**The F6 Framework** provides a structured, holistic approach to building software with intention, fostering thoughtful communication and alignment across six foundational aspects of software development.

Each foundational aspect—Volatility, Capability, Dependency, Security, Resiliency, and Investment—has been chosen because decisions made within these domains hold substantial weight in determining the success of a project. These are the areas where trade-offs are made, where challenges emerge, and where alignment between stakeholders and implementation teams becomes critical.

The framework is designed to illuminate key questions and decisions within each foundation. Decisions in one area often create headwinds or tailwinds for others, impacting the overall trajectory of the project. Some examples are:

- If you seek high **Capability** (many features and workflows) while anticipating high **Volatility** (frequent changes), the future demands of the system is then highly uncertain, potentially lowering the quality of the capabilities, as well as impacting the effectiveness of the **Security** and most likely demanding higher **Investment** over the life-time of the system.
- In a system with low **Volatility** (relatively stable requirements) but high **Dependency** (many external dependencies and integrations), there’s a risk that external tools or services will evolve faster than the system itself, creating misalignment. 
- When a system relies on extensive **Dependency** (third-party tools, cloud services, or libraries), the complexity of external dependencies can introduce vulnerabilities. Without adequate **Security** measures, these integrations might expose the system to attacks or data breaches.
- A low **Investment** magnifies the trade-offs between all other foundations—the more you focus on one, the less you can afford the other.

The interplay between these foundations is at the heart of F6. By understanding the importance of each foundation, the key questions and decisions they encompass, and the relationships between them, teams can align priorities and navigate challenges more effectively.

Ultimately, F6 serves as a "translation vocabulary" between stakeholders and implementation teams. It provides a shared language to discuss and evaluate trade-offs, ensuring that every decision is informed, intentional, and aligned with the project’s goals. With this framework, organizations can unlock the potential trapped in communication stalemates, enabling teams to build systems that are not only functional but deeply impactful.

{{< cards >}}
  {{< card url="/docs/foundations/volatility/" title="Volatility" icon="bolt" >}}
  {{< card url="/docs/foundations/capability/" title="Capability" icon="puzzle-piece" >}}
  {{< card url="/docs/foundations/dependency/" title="Dependency" icon="link" >}}
  {{< card url="/docs/foundations/security/" title="Security" icon="shield-check" >}}
  {{< card url="/docs/foundations/resiliency/" title="Resiliency" icon="server" >}}
  {{< card url="/docs/foundations/investment/" title="Investment" icon="chart-pie" >}}
{{< /cards >}}