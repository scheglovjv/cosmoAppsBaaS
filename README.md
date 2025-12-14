CosmoApps Runtime

This repository contains the open-source runtime and API layer for CosmoApps.

The runtime executes applications generated from metadata models and exposes a unified HTTP API for data access and execution.

Important:
This repository does NOT include any visual designer, BI tools, or application constructor UI.
Those components are proprietary and maintained in separate private repositories.

Scope

Included:

Runtime execution layer

HTTP API (single POST-based endpoint pattern)

Metadata-driven data access

Integration with Azure services

Explicitly excluded:

Visual designers

BI / analytics UI

Admin or modeling tools

Any proprietary UI components

Technology Stack

Platform: Azure Functions v4

Language: TypeScript

Module system: ESM

Runtime: Node.js 18+

Database: Azure Cosmos DB (SQL API)

Hosting: Azure Static Web Apps + Azure Functions

Architectural Principles

Metadata-driven runtime (no hardcoded business logic)

Single unified HTTP API for:

select

upsert

delete

Stateless server functions

Authorization handled at the project level

Designed for future BaaS / multi-tenant usage

Repository Structure (initial)

The exact structure is intentionally minimal at this stage and will evolve:

/src
  /functions        # Azure Functions entry points
  /runtime          # Core runtime logic
  /services         # Infrastructure integrations
  /models           # Metadata models and contracts

Development Notes

This repository starts from a clean implementation.

Legacy implementations may be used as conceptual references only and are not copied here.

All code in this repository is original and written specifically for this runtime.

License

This project is licensed under the MIT License.
See the LICENSE file for details.

Status

🚧 Work in progress
Initial structure and core runtime are under active development.
