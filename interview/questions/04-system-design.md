# System Design for Managers

System design interviews for EMs test architectural judgment, not implementation detail. The focus is on how you guide technical decisions, structure teams around systems, and balance operational concerns with feature development.

Companies with dedicated system design rounds for EMs include Google, Meta, Amazon, and most infrastructure-focused companies. The format differs from IC system design: EMs are expected to discuss team ownership, operational readiness, and cross-team coordination alongside the architecture.


## Format

Typically 45-90 minutes. You drive the conversation through:

- Clarify the requirements, constraints, and user needs
- Propose a high-level architecture with clear component boundaries
- Discuss team ownership and operational concerns
- Address trade-offs, failure modes, and scaling challenges
- Describe how you would sequence the implementation across sprints

Time allocation:

- 5-10 min clarifying requirements and constraints
- 15-20 min high-level architecture and component design
- 10-15 min team ownership, operational concerns, and deployment strategy
- 10-15 min trade-offs, failure modes, and scaling
- 5-10 min implementation sequencing and team coordination


## Questions

### Architecture at the Leadership Level

- Design a notification system that supports multiple channels (push, email, SMS, in-app). How would you structure the team ownership?
- You are the EM for a team building a real-time analytics pipeline. Walk through the architecture and how you would organize the team to build and operate it.
- Design a content moderation system. How do you balance automation with human review? How do you structure the engineering team?
- Your team needs to build a multi-tenant SaaS platform from an existing single-tenant application. How do you plan the migration and organize the work?
- Design a feature flag system for a large engineering organization. How do you handle rollout, monitoring, and cleanup?

### Operational Excellence

- You are taking over a service with no monitoring, no runbooks, and an average incident response time of 2 hours. How do you improve it?
- How do you design an on-call rotation for a team of 6 engineers? What policies do you put in place?
- Your service has an SLO of 99.95% availability. You missed it last quarter. How do you investigate and improve?
- Walk through how you would run a post-mortem for a major outage that affected customers for 4 hours.
- How do you decide when a system is reliable enough to stop investing in reliability?

### Scaling Systems and Teams

- Your service handles 10K requests per second. Product says it needs to handle 100K by next year. How do you plan the technical and organizational scaling?
- You inherit a team that owns 3 services but has only 5 engineers. How do you prioritize and manage scope?
- How do you handle a situation where your team's service is a dependency for 10 other teams? How do you manage the coordination burden?

### Build vs Buy

- Your team needs a CI/CD pipeline. Do you build custom tooling or adopt an existing platform? How do you decide?
- Product wants to add search functionality. Do you build it on top of Elasticsearch or buy a managed search service? Walk through your analysis.
- How do you evaluate third-party dependencies? What criteria do you use?


## What Interviewers Look For

- Architectural breadth, not depth. EMs are not expected to specify database schemas or write API contracts. They are expected to discuss component boundaries, data flow, and trade-offs at a high level.
- Team ownership thinking. How systems map to team boundaries. Who owns what. How ownership boundaries affect velocity and on-call burden.
- Operational maturity. Monitoring, alerting, incident response, and reliability investment are EM responsibilities.
- Sequencing and delivery planning. How you break down a large system build into shippable increments that a team can deliver.
