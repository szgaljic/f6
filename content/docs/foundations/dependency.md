---
title: Dependency
weight: 3
---

## Overview

_Harmonizing internal and external components to create cohesive, effective solutions._

No software system exists in isolation. Every application relies on an ecosystem of tools, libraries, platforms, and services, each playing a role in its capability and success. **Dependency** focuses on strategically managing this ecosystem—deciding what to build, what to buy, and how to seamlessly connect all the pieces.

This foundational aspect is about understanding the core identity of your software: what makes it unique and mission-critical? This identity informs decisions about ownership versus reliance. 

Each trade-off requires deep consideration—relying on third-party solutions can accelerate development and offload complexity but introduces risks, such as vendor lock-in, dependency vulnerabilities, or misalignment with future needs. 

Ultimately, Dependency challenges teams to think holistically about the ecosystem their software inhabits.

## Trade-Offs

### Build vs. Buy (CRM Example)

When deciding between building a custom CRM solution and adopting a commercial off-the-shelf (COTS) product like HubSpot, stakeholders face a classic trade-off. Both approaches have distinct advantages and risks, and the decision often hinges on factors like business goals, budget, timeline, and long-term flexibility. Hybrid solutions, which blend elements of both, offer a middle ground but come with their own set of challenges.

- **Option 1 - Build a Custom CRM Solution:** Building a CRM solution tailored to the specific needs of the organization provides unmatched customization and control. Teams can design workflows, data structures, and integrations precisely aligned with their business operations.
- **Option 2 - Adopt HubSpot as a COTS Solution:** HubSpot, as a COTS product, offers a robust, pre-built CRM solution with features designed to address a wide range of use cases. It is often favored for its simplicity and scalability.
- **Option 3 - Hybrid Approach:** A hybrid approach involves using HubSpot or another COTS CRM as a foundation while building custom extensions or workflows to address unique business needs.

| **Option**          | **Short-Term Advantage**                     | **Long-Term Advantage**                    | **Short-Term Risk**                  | **Long-Term Risk**                   |
|---------------------|---------------------------------------------|-------------------------------------------|--------------------------------------|--------------------------------------|
| **Build**           | Full control, tailored solution             | Seamless evolution with the business       | High cost and time investment        | Maintenance burden, internal reliance |
| **Buy (HubSpot)**   | Quick deployment, lower upfront cost         | Access to updates and vendor support       | Limited customization, vendor lock-in| Scaling limitations                  |
| **Hybrid**          | Faster deployment with partial customization | Balanced flexibility                       | Moderate effort and cost             | Integration and compatibility risks   |

### Software Library (Docker Base Image Example)

Modern software development often relies on containers, which are a lightweight and reliable way to run software. Containers can be compared to standardized shipping containers—they package everything needed to run an application in a predictable and portable format. Docker is a tool that simplifies the creation and management of these containers, ensuring they include all the necessary components for smooth operation.

A Docker base image serves as the starting point for these containers, providing a preconfigured environment upon which developers build their applications. While choosing a base image might seem like a minor technical detail, it can have a profound impact on a system’s performance, security, and maintainability. For example, Ubuntu is a widely trusted base image, supported by a large community, while Alpine is a minimalist image optimized for efficiency. Alternatively, niche, custom-built images offer tailored solutions but come with unique risks and challenges.

- **Option 1 - Use a Standard Image (e.g., Ubuntu):** Industry-standard images like Ubuntu offer reliability, compatibility, and extensive community support.
- **Option 2 - Use a Minimalist Image (e.g., Alpine):** Minimalist images like Alpine are smaller and faster but may introduce challenges with compatibility and debugging.
- **Option 3 - Use a Custom Niche Image:** Custom or obscure images can streamline the build process for specific use cases but often come with risks related to transparency, long-term support, and security.

| **Option**               | **Short-Term Advantage**                        | **Long-Term Advantage**                    | **Short-Term Risk**                      | **Long-Term Risk**                       |
|--------------------------|------------------------------------------------|-------------------------------------------|------------------------------------------|------------------------------------------|
| **Standard Image**       | Broad support, ease of use                     | Stable, widely understood, and secure     | Larger size, may include unnecessary dependencies | Limited optimization for specific use cases |
| **Minimalist Image**      | Smaller size, faster builds, reduced attack surface | Efficient and lightweight                 | Dependency conflicts, harder debugging   | May require frequent updates or fixes    |
| **Custom Niche Image**    | Tailored to project, optimized for specific needs | Highly streamlined for unique requirements| Lack of transparency, higher risk of issues | Abandonment, lack of long-term support    |
