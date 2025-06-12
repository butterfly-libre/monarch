# Monarch Overview

Monarch is an enterprise application platform with a single mission: provide a reusable foundation for running services so teams can deliver business value faster. By standardizing configuration, deployment, and data modeling, Monarch removes much of the boilerplate that typically surrounds new applications.

## Core Components

- **Service Runtime** – Manages lifecycle, configuration and health of services.
- **Deployment Tools** – Opinionated tooling that packages services and supports rolling updates and rollbacks.
- **Observability Stack** – Built-in metrics and logging integrations to simplify monitoring.
- **Historical Modeling Layer** – Stores all changes immutably so any state can be reconstructed from event history.
- **Interface Description Language** – Used to declare data structures and external service endpoints.
- **VCS-Driven Migrations** – Automatically applies migrations whenever IDL definitions change.

## How Monarch Works

Applications interact with Monarch's runtime, which reads configuration from version control and orchestrates each service. Data is modeled as a stream of events; new IDL definitions trigger migrations that keep data stores and APIs in sync. The result is predictable deployments and traceable state changes.

## Goals

1. Consolidate proven techniques from real-world deployments.
2. Offer defaults that can be customized as projects evolve.
3. Provide documentation and examples that help teams ship quickly.

For additional background on why the project exists, see [motivation.md](motivation.md).
