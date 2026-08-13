# ADR-0001 — Initial Architecture

**Status:** Accepted  
**Date:** 2026-08-12

## Context

PERFILIA is at the pre-MVP stage. We need fast iteration without creating unnecessary operational complexity while preserving a path to scale.

## Decision

Start with a **modular monolith**:

- React + TypeScript frontend
- Python + FastAPI backend
- PostgreSQL database
- Provider-agnostic AI orchestration layer
- Local development first
- AWS introduced after functional validation

## Consequences

### Positive
- Fast development.
- Simple deployment model.
- Clear domain boundaries.
- Lower initial infrastructure cost.
- Easier debugging.

### Negative
- Some future scaling boundaries will initially share a deployment unit.
- Extraction into independent services may be required later if justified by load or organizational needs.

## Reconsider when

Introduce separate services only when there is a demonstrated requirement such as independent scaling, reliability isolation, deployment independence, or a clear organizational boundary.
