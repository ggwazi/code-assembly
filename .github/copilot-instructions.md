# Copilot Instructions for code-assembly

## Project Overview
This repository is intended to be a **Turborepo monorepo** containing Next.js web applications and React Native mobile applications. Currently in early planning phase with minimal implementation.

## Intended Architecture (Based on Git History)
- **Monorepo Structure**: Turborepo-based workspace for shared tooling and dependencies
- **Web Apps**: Next.js applications for web interfaces  
- **Mobile Apps**: React Native applications for mobile platforms
- **Shared Packages**: Common utilities, components, and configurations

## Expected Directory Structure
When implementing, follow this standard Turborepo pattern:
```
apps/
  web/           # Next.js web application
  mobile/        # React Native application
packages/
  ui/            # Shared UI components
  config/        # Shared configurations (ESLint, TypeScript, etc.)
  utils/         # Shared utilities
turbo.json       # Turborepo configuration
package.json     # Root package.json with workspaces
```

## Development Workflow (To Be Established)
- Use `pnpm` as package manager for monorepo efficiency
- Turborepo for build orchestration and caching
- Shared tooling configurations across all packages

## Key Implementation Guidelines
1. **Workspace Setup**: Configure workspaces in root `package.json` pointing to `apps/*` and `packages/*`
2. **Shared Dependencies**: Place common dependencies in root, app-specific ones in respective apps
3. **Build Pipeline**: Use Turborepo tasks for coordinated builds across packages
4. **Code Sharing**: Extract reusable components and utilities to shared packages

## Current State
- Repository contains only basic README.md
- Previous Copilot agent planned turbo mono-repo structure (see branch `origin/copilot/create-turbo-mono-repo`)
- Ready for full implementation of the planned architecture

## Next Steps for AI Agents
1. Set up basic Turborepo structure with `turbo.json`
2. Initialize Next.js app in `apps/web/`
3. Initialize React Native app in `apps/mobile/`
4. Create shared packages for UI components and utilities
5. Configure package.json workspaces and dependencies
6. Set up development scripts and build pipeline

## Branch Context
- `main`: Current minimal state
- `origin/copilot/create-turbo-mono-repo`: Contains initial planning phase

When working on this codebase, prioritize establishing the monorepo foundation before building individual applications.