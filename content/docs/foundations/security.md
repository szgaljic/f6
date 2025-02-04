---
title: Security
weight: 3
---

## Overview

_“How do we protect assets?”_

Security is often taken for granted until something goes wrong. It’s a complex field, filled with intricate frameworks, processes, and terminology. While all of these elements are valuable and serve a purpose, only a select few deeply understand them. The challenge, however, is that security isn’t just a technical concern—it’s a fundamental business necessity that safeguards data, systems, and trust.

In modern software systems, **security is a shared responsibility**—not solely owned by IT or security teams, but by leadership, developers, and even end users. A security breach doesn’t just result in technical issues—it leads to financial loss, reputational damage, and legal consequences.

The **Security** foundation addresses the important role of protecting data, systems, and user trust in achieving business goals. It’s about viewing security not as an afterthought or a mere compliance checkbox but as an integral part of the entire implementation process.

Unlike [**Features**](/docs/foundations/features) or [**Optimizations**](/docs/foundations/optimizations), **Security** isn’t about building something new; it’s about ensuring that everything already built remains safe, functional, and resilient.

## What is Security?

At its core, **Security** is about safeguarding the confidentiality, integrity, and availability of information and systems—a concept often referred to as the CIA Triad.

- **Confidentiality** ensures that sensitive information is accessible only to authorized individuals. Think of it as locking away valuable documents in a secure vault, where only those with the right key can access them.
- **Integrity** means maintaining the accuracy and consistency of data, preventing unauthorized modifications or tampering. It’s like having a tamper-proof seal on a product, guaranteeing that it hasn't been altered since it left the factory.
- **Availability** ensures that systems and data are accessible when needed. Imagine a power grid that can withstand outages and continue to deliver electricity reliably—that's availability in action.

These three elements work together to form the bedrock of a robust security posture. For example, a banking system must keep customer account details confidential, ensure that transaction records are accurate (integrity), and be available 24/7 for customers to access their funds (availability).

### Proactive vs. Reactive Security

Security is not a one-time task but a continuous process of improvement. It's not enough to simply react to security incidents as they occur. A proactive approach is essential—anticipating potential threats and building defenses before an attack takes place. This requires a shift in mindset, from viewing security as a cost center to seeing it as a strategic investment in the long-term health and resilience of the business.

A proactive approach is always preferable. Consider the [**WannaCry ransomware attack in 2017**](https://en.wikipedia.org/wiki/WannaCry_ransomware_attack). Organizations that had proactively patched their systems were unaffected, while those that hadn’t faced devastating consequences.

Here is a table that helps illustrate the difference in response strategy for various security risks:

| Threat                  | Proactive Action                                                        | Reactive Action                                              |
|-------------------------|------------------------------------------------------------------------|--------------------------------------------------------------|
| [Phishing Attacks](https://en.wikipedia.org/wiki/Phishing)       | Train employees, implement advanced email filtering, and use MFA.     | Investigate, reset credentials, notify users, and enhance security. |
| [Ransomware](https://en.wikipedia.org/wiki/Ransomware)            | Use endpoint protection, back up data (3-2-1 rule), and segment networks. | Isolate systems, engage response team, restore backups, assess ransom. |
| [Insider Threats](https://en.wikipedia.org/wiki/Insider_threat)       | Apply least privilege access, monitor activity, and conduct audits.    | Investigate, revoke access, assess damage, and tighten controls. |
| [Denial of Service (DoS)](https://en.wikipedia.org/wiki/Denial-of-service_attack) | Use DDoS mitigation, a CDN, and an incident response plan.            | Filter traffic, apply rate limiting, and scale infrastructure. |
| [Data Breaches](https://en.wikipedia.org/wiki/Data_breach)        | Encrypt data, use DLP, and conduct security assessments.               | Investigate, notify affected parties, and enhance security.  |
| [Supply Chain Attacks](https://en.wikipedia.org/wiki/Supply_chain_attack) | Vet vendors, monitor dependencies, and use code signing.              | Investigate, remove compromised software, and strengthen security. |
| [Malware](https://en.wikipedia.org/wiki/Malware)             | Use endpoint protection, block malicious sites, and educate users.      | Remove malware, identify the source, and improve protection. |


[**Threat modeling**](https://en.wikipedia.org/wiki/Threat_model) is a key technique in proactive security. It involves identifying potential vulnerabilities in a system and the threats that could exploit them. By thinking like an attacker, organizations can better understand their weaknesses and prioritize their security efforts.

### Common Vulnerabilities

Software systems often contain weaknesses, known as vulnerabilities, that attackers can exploit. The [OWASP Top 10](https://owasp.org/www-project-top-ten/) is a widely recognized list of the most critical web application security risks, regularly updated to reflect the evolving threat landscape.

Trained security professionals continuously monitor the ecosystem, analyze emerging attack techniques, and develop strategies to mitigate them. Additionally, various security tools can be integrated into your system to automatically update with the latest threat intelligence, scan for vulnerabilities, and alert teams to potential risks.

## Security Considerations

https://gemini.google.com/u/1/app/0e445a9cd21cee5e
https://chat.deepseek.com/a/chat/s/58eaa7ed-ec90-46cd-be53-f04bcee07036
https://chatgpt.com/c/679ae48b-538c-8011-9a25-9451297e610c