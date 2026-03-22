# Day-85-100-Days-challenge-in-cybersecurity
### Day 85: Case Study - Software Supply Chain Failures ⛓️💥

#### 📖 Overview
Today’s study explored the mechanics of Supply Chain Attacks, where attackers target widely-used third-party libraries to gain access to thousands of downstream applications simultaneously.

#### 🔍 The "Transitive Dependency" Problem
- **App A** trusts **Library B**.
- **Library B** relies on **Helper C**.
- If **Helper C** is compromised, **App A** is breached, often without the developer ever knowing Helper C existed.

#### 🛡️ Mitigation Strategies
| Strategy | Action Item |
| :--- | :--- |
| **Audit** | Perform regular SCA (Software Composition Analysis) scans. |
| **Patching** | Automate dependency updates (e.g., Dependabot, Renovate). |
| **Integrity** | Verify Checksums and Digital Signatures before deployment. |
| **Monitoring** | Fail CI/CD builds if critical CVEs are detected in dependencies. |

#### 💡 Key Lesson
> "Security isn't only about your own code; it's about every dependency you use. You are responsible for the integrity of the final product."
