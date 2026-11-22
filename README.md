# PAIMANA Sentinel

**A data-driven project monitoring and investigation dashboard.**

PAIMANA Sentinel transforms project-level monitoring data into a unified analytical workspace for tracking progress, identifying attention areas, exploring historical changes, and investigating project evidence.

> Built for the Smart India Hackathon (SIH) — PAIMANA VANTAGE.

## Overview

PAIMANA Sentinel is a backend-first monitoring platform featuring a command-centre interface, portfolio-level visualization, historical project tracking, and evidence-aware assessment.

The frontend acts as a client to the backend, keeping the core analytical logic centralized.

## Features

- **Executive Readout** — A high-level overview of project attention, reported movement, commitment revisions, and assessment coverage.
- **Portfolio Map** — Geographic visualization of projects with contextual map clustering.
- **Project Investigation** — Explore individual projects, their signals, status, and supporting information.
- **Historical Tracking** — Compare project snapshots across reporting periods.
- **Integrity & Trajectory Analysis** — Deterministic assessment logic and project trajectory calculations.
- **Evidence & Provenance** — Trace analytical outputs back to their supporting source context.
- **Intervention Workflow** — Track interventions and maintain an audit trail.
- **Historical Cohort Analysis** — Compare projects against historical cohorts.
- **Analyst Query Interface** — Structured queries for project-level analysis.
- **CSV Export** — Export data for further analysis.

## Tech Stack

| Layer | Technologies |
|---|---|
| Frontend | React, Vite, TypeScript |
| Visualization | Recharts, Leaflet |
| Icons | Lucide |
| Backend | Python, FastAPI |
| Data Processing | PDFPlumber |
| Database | SQLite |
| API | REST |

## Architecture

```text
┌─────────────────────────────┐
│      React Dashboard      │
│   Vite · Charts · Maps    │
└──────────────┬──────────────┘
               │ API Requests
               ▼
┌─────────────────────────────┐
│       FastAPI Backend      │
│ Analytics · Integrity      │
│ Historical · Evidence     │
└──────────────┬──────────────┘
               │
               ▼
┌─────────────────────────────┐
│        SQLite Data         │
│ Projects · Sources ·       │
│ Monthly Snapshots          │
└─────────────────────────────┘
```

## Data Coverage

The bundled dataset includes historical monthly project snapshots from **July 2025 through April 2026**, with April 2026 used as the active assessment snapshot.

The repository includes a SQLite database, source manifest, and bundled report files for local use.

## Getting Started

### Prerequisites

- Windows
- Python
- Node.js and npm
- Git

### Quick Start

1. Clone the repository:

   ```bash
   git clone https://github.com/Afx-Morpheus/PAIMANA-VANTAGE-SIH-26103.git
   ```

2. Navigate into the project directory:

   ```bash
   cd PAIMANA-VANTAGE-SIH-26103/PAIMANA-VANTAGE-main
   ```

3. Start the application using the Windows startup script:

   ```bat
   START_SENTINEL.bat
   ```

The startup script prepares the local environment, launches the backend and frontend, performs health checks, and opens the dashboard.

To stop the application, use:

```bat
STOP_SENTINEL.bat
```

## Project Structure

```text
PAIMANA-VANTAGE-main/
├── backend/
│   ├── app/
│   │   ├── api.py
│   │   ├── db.py
│   │   ├── config.py
│   │   └── ingestion/
│   ├── data/
│   └── tests/
├── frontend/
├── docs/
├── scripts/
├── START_SENTINEL.bat
└── STOP_SENTINEL.bat
```

## Project Goals

- Improve visibility into project progress and status.
- Make historical reporting easier to explore.
- Surface signals that warrant further investigation.
- Connect analytical outputs with source evidence.
- Provide an accessible monitoring interface for complex project portfolios.

## Disclaimer

PAIMANA Sentinel is an analytical and monitoring prototype. Its outputs should be interpreted alongside source reports and contextual review. Automated assessments are intended to support investigation, not replace human judgment.

---

**PAIMANA Sentinel · PAIMANA VANTAGE · SIH 26103**
