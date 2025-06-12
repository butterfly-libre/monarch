# Monarch
Monarch is an enterprise application platform. It packages the patterns and
tooling needed to run reliable services so that teams can focus on business
logic rather than rebuilding infrastructure.

The project collects lessons learned from real deployments and offers a
repeatable way to configure, deploy, and monitor applications. By adopting
Monarch you get a foundation that encourages best practices from day one.

## Motivation
Organizations frequently rebuild the same scaffolding to manage configuration,
deployments, and service communication. This duplication wastes time and leads
to inconsistent solutions. Monarch was created to consolidate these common
concerns into one cohesive platform.

## Problems solved
* Provides a uniform approach to service runtime management and configuration.
* Automates deployment tasks, including rolling updates and rollbacks.
* Ships with integrated observability so monitoring is built in from the start.
* Defines data structures and APIs through a common IDL to avoid drift.
* Generates migrations automatically as those definitions evolve via version
  control.
* Maintains an immutable record of every state change for auditability.

## Key features
- Opinionated service runtime with health checks and configuration management.
- Deployment tooling that supports rolling updates and rollbacks out of the box.
- Integrated observability stack for logging and metrics collection.
- Immutable historical modeling architecture that records every change.
- Interface description language (IDL) for declaring data structures and service
  endpoints.
- Version control integration that automates migrations as the IDL evolves.

## Architecture
At its core Monarch ships a small runtime and a set of tools for packaging and
deploying services. Data is modeled using an immutable historical approach so
any state can be reproduced from prior events. Service schemas and external APIs
are defined using Monarch's IDL. Migration tooling watches those definitions in
version control and automatically prepares the necessary migrations. While the
default assumes containerized workloads, the concepts apply to many runtimes.

## Getting started
See [docs/getting-started.md](docs/getting-started.md) for a minimal walk-through
of how to launch a new service using Monarch. The documentation will expand over
time with more examples and best practices.

## Additional documentation
More background and details about the project can be found in
[docs/overview.md](docs/overview.md) and [docs/motivation.md](docs/motivation.md).
As the project evolves, new documents will be added under the `docs/` directory.

## License
Monarch is released under the terms of the GNU General Public License version 2.
Refer to the [LICENSE](LICENSE) file for details.

