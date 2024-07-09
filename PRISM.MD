## Background
Building high-performance, resilient teams is no accident. It requires the right foundational capabilities, behaviors, and processes to produce the best outcomes. Regrettably, there is no definitive playbook for building high-performing teams.

DevOps Research and Assessment (DORA) has attempted to measure software delivery performance using a few metrics. While these metrics provide some insights, they focus narrowly on software delivery aspects, potentially overlooking other crucial factors in building, collaborating, delivering, and operating software in production.

Having worked with diverse organizations—including product companies, startups, large banks, and governments—I have seen the common challenges they face. Drawing on this experience, I developed a framework to evaluate development teams' maturity and introduce foundational practices to build high-performing teams.

Introducing PRISM: Performance and Resilience Index for Software-delivery Maturity.

## Introduction

PRISM is a comprehensive framework designed to evaluate and enhance the maturity and performance of software delivery teams. It stands on seven key pillars: Team Organization, Developer Enablement, Delivery Flow, Rugged Score, Chaos Tolerance, Ops Capability, and Elasticity Score. 

By assessing these core areas, PRISM can provide actionable insights and metrics to guide teams toward achieving high performance and resilience in software delivery.

PRISM comes with:

A framework to guide the incorporation of foundational capabilities
A scorecard to assess team maturity
A set of metrics for ongoing team performance evaluation

These components work together to generate a comprehensive PRISM Score.

### The Seven Pillars of PRISM
### 1. Team Organization

Effectiveness in managing work from requirements to delivery, with a clear engagement model, appropriate governance, and ensure balance between burn and value delivered is acceptable.

How work is managed from requirements to delivery. The focus is on whether the team is equipped with a clear engagement model, how delivery is managed and governed, and whether the balance between burn and value delivered is acceptable.

- **Engagement Model**: Established front door for internal/external customers to reach out for services.
- **Service Catalog**: Clear service catalog describing the services offered with SLAs, pricing defined where applicable.
- **Flow Management**: Processes for managing work using Agile, Lean, or other frameworks.
- **Visibility & Alignment**: Approach for making work visible to stakeholders and ensuring alignment with organizational goals using methods like OKRs, Quarterly Business Reviews, Value Stream Mapping, or Program Increments.
- **Team Communication**: Clearly established channels for internal & external team communication.

KPIs:

- Customer satisfaction scores for service delivery.
- Percentage of work items delivered on time.
- Number of escalations or missed SLAs.
- Frequency and quality of stakeholder updates.
- Team communication effectiveness survey results.
<br>

### 2. Developer Enablement

Availability of the right tools, environments, safety guardrails, standards, and procedures.

- **Tools & Gears**: Availability of right tools that are accessible and performant for the team’s job at hand.
- **Environments**: Automated, repeatable dev, build, and test environments including using modern approaches like Devcontainers, Codespaces, Nix, etc
- **Standards & Procedures**: Clear, documented standards and processes to assist developers in performing day-to-day activities, from creating a new repo to raising a change to production.
- **Safety Guardrails**: Established guardrails, preferably automated, to prevent developers from affecting general safety, functionality, and introducing vulnerabilities in deliverables
- **Developer Surveys:** Periodic surveys to enable open communication, gather feedback on the ways of working, aspects causing burnouts and facilitate for actions to improve identified issues and opportunities

KPIs:

- Time to set up a new development environment.
- Percentage of human errors could have been addressed through guardrails / checkpoints.
- Number of critical vulnerabilities detected before production.
- Developer onboarding time.

### 3. Delivery Flow

Friction on the assembly line directly impacts teams productivity.

- **Automated Pipelines**: Standardized, automated build & deployment, rollback process enabled through pipelines with necessary controls for governance.
- **Change Process Efficiency & Agility**: maturity of an organization's change management process, ranging from non-existent to highly efficient and automated
- **Change Impact Assessment**: Ability to objectively assess and communicate the potential impact of changes using data-driven methods through such as dependency graphs, code mininig etc
- **Service interruption**: Ability to deploy changes to production with no / minimal disruption for external as well as internal teams

KPIs:

- Downtime of the developer infra such as build system, source control repository, etc
- Lead time for changes.
- Number of failed changes in production

### 4. Rugged Score

Team's ability to produce cyber-safe, reliable, resilient software that customers can use confidently

- **Safety Culture**: Safety and security requirements identified from the beginning and system  is designed, built, and tested accordingly through the life cycle.
- **Vulnerability Management**: Ability to react quickly to zero-day vulnerabilities and roll out fixes to production. Having active system / process in place to monitor for threats.
- **Safety and Security Testing**: Capability to verify accuracy, security, and robustness through reliable testing methodologies.
- **Security Incident Recovery Plan**: Clear action plan for communicating with stakeholders, establishing action teams, and identifying recovery plans and kill switches on the event of a security incident / data breach
- **Off Boarding** - Systamatic removal of access to systems / assets for the outgoing member

KPIs:

- Time to identify and remediate vulnerabilities.
- Frequency of security drills and testing.
- Number of security incidents and response times.
- Percentage of systems passing security audits.
- Data breach incidents
- Data breaches prevented

### 5. Chaos Tolerance

Ability to handle chaos - losing a key member, introducing a new tool, process change, or requirements change.

- **Attrition Management**: How well the team can cope with the loss of a key member and how knowledge is accumulated and shared.
- **Process Change**: Ease of changing or introducing new processes in the team.
- **Technology Disruption Resilience**: Culture of grasping and adapting to changes in their space, experimenting, and adapting proactively.

KPIs:

- Time to recover from the loss of a key team member.
- Frequency and impact of process changes.
- Number of new tools/technologies successfully adopted.
- Percentage of team members trained in new processes/tools.

### 6. Ops Capability

Managing systems in production requires its own process, tools, and skills. Is the team capable of running systems in production?

- **Observability**: Equipped with necessary tools to observe the system in production and quickly identify issues before customers are impacted.
- **Production Incident Management**: Clearly documented process, tools for issue triaging, external team engagement, escalation, communication, and postmortem.
- **Automation**: Runbooks and standard operating procedures to manage systems in production.
- **Production Guardrails**: Prevent human errors through necessary review processes enforced through people or automation.
- **Reliability and Cost Management**: Continual improvement of availability, security, performance, and observability, with systems to monitor usage and identify cost-saving opportunities.

KPIs:

- Mean time to detect (MTTD) and mean time to resolve (MTTR) incidents.
- Percentage of incidents detected before customer impact.
- Frequency and effectiveness of incident postmortems.
- Operational cost savings identified and implemented.

### 7. Team Elasticity

Team's ability to scale to manage delivery requirements. How long does it take for a new member to become productive? How good is the experience of the new member before becoming productive?

- **Developer Onboarding & offboarding**: Clearly documented onboarding documents to help new members quickly come up to speed, and offboarding procedures for necessary knowledge handovers
- **Interview Process**: Clear interview process to recruit ideal candidates using structured methods and practices.

KPIs:

- Time to onboard new team members to productivity.
- Satisfaction scores from new hires on the onboarding process.
- Time to offboard team members.
- Interview-to-hire ratio.<br><br><br>

## **Scorecard**

Here is an example scorecard created to demonstrate how this framework can be used to measure the current maturity and performance of a team.

### Squad Name:  Alpha 1

### **1:  Team Organization**

**Overall Score: 🟢 4**

| Subitem | Score | Description |
| --- | --- | --- |
| Engagement Model | 🟢 5 | Well-established front door for internal/external customers to request services. |
| Service Catalog | 🟢 4 | Clear catalog of services with defined SLAs and pricing, minor updates needed. |
| Flow Management | 🟢 4 | Efficient Agile process for managing work, with room for optimization. |
| Visibility & Alignment | 🟡 3 | OKRs in place, but alignment with organizational goals could be improved. |
| Team Communication | 🟢 4 | Clear channels established, but external engagement could be enhanced. |

### **2:  Developer Enablement**

**Overall Score: 🟡 3**

| Subitem | Score | Description |
| --- | --- | --- |
| Tools & Gears | 🟢 4 | Most necessary tools are available and accessible. |
| Environments | 🟡 3 | Dev and test environments are in place, but automation could be improved. |
| Standards & Procedures | 🟡 3 | Documentation exists but is not consistently followed or updated. |
| Safety Guardrails | 🟠 2 | Basic guardrails in place, but more comprehensive automation needed. |
| Developer Surveys | 🟢 4 | Regular surveys conducted with good follow-up on feedback. |

### **3:  Delivery Flow**

**Overall Score: 🟢 4**

| Subitem | Score | Description |
| --- | --- | --- |
| Automated Pipelines | 🟢 4 | Standardized, automated build & deployment for most projects. |
| Change Process Efficiency & Agility | 🟢 4 | Efficient change management process with some manual steps. |
| Change Impact Assessment | 🟡 3 | Basic impact assessment in place, but not fully data-driven. |
| Service Interruption | 🟢 5 | Minimal disruption during deployments for both external and internal teams. |

### **4:  Rugged Score**

**Overall Score: 🟠 2**

| Subitem | Score | Description |
| --- | --- | --- |
| Safety Culture | 🟠 2 | Basic safety awareness, but not consistently applied throughout the lifecycle. |
| Vulnerability Management | 🟡 3 | Reactive approach to vulnerabilities, monitoring system in place. |
| Safety and Security Testing | 🟠 2 | Some testing methodologies in place, but not comprehensive. |
| Security Incident Recovery Plan | 🔴 1 | Minimal planning for security incidents or data breaches. |
| Off Boarding | 🟡 3 | Process exists but not consistently followed for all systems/assets. |

### **5:  Chaos Tolerance**

**Overall Score: 🟡 3**

| Subitem | Score | Description |
| --- | --- | --- |
| Attrition Management | 🟡 3 | Some knowledge sharing practices, but key person dependencies exist. |
| Process Change | 🟡 3 | Team can adapt to changes, but with some resistance and delay. |
| Technology Disruption Resilience | 🟢 4 | Good culture of experimentation and adaptation to new technologies. |

### **6:  Ops Capability**

**Overall Score: 🟢 4**

| Subitem | Score | Description |
| --- | --- | --- |
| Observability | 🟢 5 | Comprehensive tools and practices for system observation. |
| Production Incident Management | 🟢 4 | Well-documented process for issue triaging and management. |
| Automation | 🟡 3 | Some runbooks and SOPs in place, but more automation needed. |
| Production Guardrails | 🟢 4 | Good review processes and automation to prevent human errors. |
| Reliability and Cost Management | 🟡 3 | Regular system improvements, but cost management could be optimized. |

### **7:  Elasticity Score**

**Overall Score: 🟡 3**

| Subitem | Score | Description |
| --- | --- | --- |
| Developer Onboarding | 🟡 3 | Documented onboarding process, but not consistently applied. |
| Developer Offboarding | 🟠 2 | Minimal procedures for knowledge handover during offboarding. |
| Interview Process | 🟢 4 | Structured interview process, but could be more effective in candidate selection. |

Legend: 🔴 1 - Critical 🟠 2 - Needs Improvement 🟡 3 - Satisfactory 🟢 4 - Good 🟢 5 - Excellent

## Overall PRISM Score: 🟡 3 (Satisfactory)

| Pillar | Score |
|--------|-------|
| 1. Team Organization | 🟢 4 |
| 2. Developer Enablement | 🟡 3 |
| 3. Delivery Flow | 🟢 4 |
| 4. Rugged Score | 🟠 2 |
| 5. Chaos Tolerance | 🟡 3 |
| 6. Ops Capability | 🟢 4 |
| 7. Elasticity Score | 🟡 3 |

**Average Score: 3.29 (Rounded to 3)**

Legend: 🔴 1 - Critical   🟠 2 - Needs Improvement   🟡 3 - Satisfactory   🟢 4 - Good   🟢 5 - Excellent


Version 0.1


## **Areas for Improvement**

1. Enhance the safety culture and implement more proactive security measures, especially in incident recovery planning.
2. Improve knowledge sharing and documentation to increase chaos tolerance and reduce key person dependencies.
3. Streamline and standardize the onboarding and offboarding processes, particularly focusing on knowledge transfer during offboarding.
4. Strengthen the alignment of team activities with organizational goals and improve visibility of work to stakeholders.
5. Implement more comprehensive and automated safety guardrails in the development process.

