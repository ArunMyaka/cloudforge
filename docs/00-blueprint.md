# CloudForge

CloudForge is an Internal Developer Platform (IDP) that automates application deployment, monitoring, and operations so developers can focus on writing code instead of manually managing infrastructure.

## Architecture Decision #1

CloudForge will initially start as a monolith because it is the simplest architecture that solves our current problem. Microservices will only be considered when real business and operational problems justify the additional complexity and trade-offs.

## Product Principles

- Architecture follows business needs.
- Solve today's problems with today's complexity. Add complexity only when new business problems justify it.
- Projects belong to the organization, not an individual developer. If a developer leaves, the projects remain available and ownership can be transferred.

## CloudForge v1 Data Model (Draft)

### Tables

- Developers
- Projects
- Deployments
- Logs

### Relationships

- One Developer can own many Projects.
- One Project can have many Deployments.
- One Deployment can generate many Logs.
## Vision

Enable developers to focus on building software instead of infrastructure.

## Mission

Automate the software delivery lifecycle through a single, consistent platform.

## North Star

Reduce developer effort and cognitive load through automation.

## Product Philosophy

Every feature in CloudForge must reduce manual work for developers and automate part of the software delivery lifecycle.

If a feature does not contribute to this goal, it should not be included in CloudForge.
