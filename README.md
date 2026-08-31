# AI-Powered Invoice Approval Agent

UiPath · Document Understanding · AI Agent · RPA

An end-to-end invoice approval automation built with UiPath, Document Understanding, OCR, and AI Agents.

## Overview

- Processes invoice PDFs and extracts key information using **Document Understanding** and **OCR**.
- Uses **AI-based invoice analysis and approval rules** to automatically approve valid invoices or route exceptions for human review.
- Automates post-approval actions with **RPA workflows**, reducing manual effort and streamlining the invoice processing lifecycle.

## Structure

- **Agent 1/** — UiPath Agent project handling AI-based invoice analysis and approval decisions
- **Maestro BPMN/** — Maestro process definition (`Process.bpmn`) orchestrating the end-to-end flow
- **RPA Workflow/** — Core RPA automation (`Main.xaml`) handling extraction and post-approval actions
- **SimpleApprovalApp1/** — UiPath App providing an Approve/Reject interface for human-in-the-loop exception review
- **Solution.uipx** — Solution manifest tying all projects together
- **SolutionStorage.json** — Solution-level storage/configuration

## Requirements

- UiPath Studio / Studio Web
- UiPath Document Understanding
- UiPath Orchestrator (Cloud or on-prem) for deployment
- Access to Maestro for BPMN process execution

## Getting Started

1. Clone this repository.
2. Open `Solution.uipx` in UiPath Studio.
3. Configure Document Understanding project/taxonomy and any required credentials.
4. Publish the individual projects to your Orchestrator tenant.
5. Deploy the Maestro process and link the entry points to the published packages.
   

