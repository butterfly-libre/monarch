# Getting Started with Monarch

This guide walks through the basics of launching a new service on Monarch.

## Prerequisites

- Docker (or another container runtime)
- Git for version control
- A database supported by Monarch, such as PostgreSQL

## Steps

1. **Clone this repository** and install Monarch's CLI tools.
2. **Initialize a new service** using `monarch init`.
3. **Run locally** with `monarch run` which loads configuration from version control.
4. **Commit your IDL files**. Monarch detects changes and prepares migrations automatically.
5. **Deploy to staging** using `monarch deploy`.

These steps are intentionally brief. Future documents will include detailed tutorials and reference configurations.

