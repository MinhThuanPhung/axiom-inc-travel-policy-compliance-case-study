

# Axiom Inc. Corporate Travel Cost Optimization (BA Case Study)

## Overview
End-to-end Business Analyst case study covering requirement gathering, 
process redesign (BPMN), and BI dashboard analysis for corporate travel spend.

## Business Problem
Axiom Inc. has no point-of-booking control to prevent premium class 
policy violations (>35% threshold), leading to reactive-only cost oversight.

## What's Included
- 📊 Tableau Dashboard: Cost efficiency analysis (2015-2024)
- 📄 Business Requirements Document (BRD)
- 🔄 As-Is / To-Be Process Diagrams (BPMN)
- 📋 User Stories & Prioritization (MoSCoW)

## Key Findings
- Premium Class Rate increased 2.46% despite 53.19% drop in flight volume
- Routes DAL-LGA (47.83%) and DAL-ELP (50.00%) exceed policy threshold

## Tools Used
Tableau Desktop, Tableau Prep Builder, Draw.io, Jira, Excel

## Details


## Overview

This project simulates the role of a Business Analyst supporting Axiom Inc.'s Finance team in closing a critical control gap identified through prior cost analysis: employees can currently book premium class travel with no system-level check against corporate policy (maximum 35% premium class rate per department/route) until after the expense has already occurred.

The purpose of this project is to design an improved travel booking process that introduces a **point-of-booking compliance check**, shifting policy enforcement from *reactive* (detected months later via dashboard reporting) to *proactive* (blocked or routed for approval before the booking is confirmed).

## Business Problem

Although Axiom Inc. has a Tableau dashboard tracking travel cost efficiency, the company currently has no point-of-booking control to prevent employees from violating the premium class policy (>35% threshold). As a result, violations are only identified after the cost has already been incurred, particularly within the BD and AM departments and on routes DAL-LGA and DAL-ELP.

## Project Objectives

1. **Translate a data-driven business problem into formal requirements** — using findings from a prior Tableau analysis (Premium Class Rate exceeding 35% on routes DAL-LGA and DAL-ELP) as the evidence base for a Business Requirements Document (BRD).
2. **Model the current and improved business process** using BPMN, identifying exactly where a new decision gateway and approval step must be inserted into the existing booking workflow.
3. **Break down requirements into actionable, prioritised user stories** (MoSCoW framework) with acceptance criteria, structured as a Jira-style backlog.
4. **Demonstrate the full BA lifecycle** — from problem discovery, to requirement documentation, to process design, to backlog-ready deliverables.

## What's Included

| Folder | Contents |
|---|---|
| `01-dashboard/` | Source Tableau report and dashboard screenshot (prior cost analysis) |
| `02-business-requirements/` | Business Requirements Document (BRD) |
| `03-process-diagrams/` | As-Is and To-Be BPMN process diagrams |
| `04-user-stories/` |  Backlog of user stories with acceptance criteria (backlog.xlsx), 
mirrored in Jira for sprint planning (jira-board-screenshot.png) |
| `05-prioritization/` | MoSCoW prioritization matrix |

## Key Findings (from prior analysis)

- Premium Class Rate increased by 2.46% in 2024 despite a 53.19% drop in total flight volume
- Route DAL-LGA reached a 47.83% premium class rate; DAL-ELP reached 50.00% — both well above the 35% policy threshold
- Departments BD and AM recorded the highest cost per trip and the largest increases in premium class usage

## Proposed Solution

### As-Is Process

<img width="1423" height="454" alt="AsIs_Process" src="https://github.com/user-attachments/assets/96c32f3a-50ff-489f-a31a-e80dd0efff98" />

Employee searches flight → selects travel class → confirms booking directly, with no system check against policy thresholds.

### To-Be Process
<img width="2165" height="1259" alt="AsIs_Process (1)" src="https://github.com/user-attachments/assets/37b67ee2-581d-4348-96b7-375f63ae6289" />

Employee searches flight → selects travel class → **system checks premium class rate against 35% threshold** → if compliant, booking auto-confirms; if non-compliant, booking routes to Line Manager for approval before confirmation.

### Sample User Story
> As a Line Manager, I want to be notified and asked to approve any booking that would push my department's premium class rate above 35%, so that policy violations are prevented before the cost is incurred rather than discovered afterward.

## Tools Used

- **Tableau Desktop / Tableau Prep Builder** - dashboard and data preparation (prior phase)
- **Lucidchart** - BPMN process diagrams
- **Microsoft Word** - Business Requirements Document
- **Excel** - MoSCoW prioritization matrix
- **Jira** - user story backlog structure
