# n8n Zoom Documentation Lifecycle Automation

This project demonstrates an **end-to-end documentation lifecycle automation** built using **n8n**.

The workflow automatically generates structured documentation, routes it through review and approval stages, and manages document lifecycle using a **status-driven workflow model**.

The system was designed to prepare **clean and reliable knowledge base documentation**, which can later be used for **RAG-based AI assistants**.

---

## Problem

In many teams documentation is:

- manually written  
- inconsistently reviewed  
- difficult to track  
- often outdated  

There is usually **no structured lifecycle** controlling how documents move from draft to approval.

This workflow solves that problem using **automation and status-driven routing**.

---

## Solution Overview

The workflow uses **Google Sheets as the control plane**.

Each document topic moves through a defined lifecycle:

Automation handles:

- draft generation
- document creation
- routing for review
- approval workflows
- document organization

---

## Workflow Architecture

Main components:

### 1. Google Sheets Trigger
Detects new or updated document topics.

### 2. AI Content Generator
Generates structured documentation drafts automatically.

### 3. Google Docs Automation
Creates and updates documentation files.

### 4. Review Workflow
Reviewer validates document quality and accuracy.

### 5. Approval Workflow
Approver confirms the final version before publishing.

### 6. Folder-based Lifecycle Management

Documents are automatically organized into lifecycle folders:

- **Draft**
- **Review**
- **Published**

---

## Repository Structure

Contains generated documentation examples.

Zoom_Knowledgebase/
### Workflow Exports
Zoom Docs - Begin Review.json
Zoom Docs - Content Generator.json
Zoom Docs - Process Approval.json
Zoom Docs - Process Review.json


### Workflow Visual References
Zoom Docs - Begin Review.PNG
Zoom Docs - Content Generator.PNG
Zoom Docs - Process Approval.PNG
Zoom Docs - Process Review.PNG



These files represent the individual automation modules used in the lifecycle.

---

## Key Design Concepts

This workflow follows several important automation principles:

- **Single source of truth (Google Sheets)**
- **Status-driven routing**
- **Human-in-the-loop review gates**
- **Folder-based lifecycle visibility**
- **Separation of system and human actions**

---

## Technologies Used

- n8n  
- Google Sheets  
- Google Docs  
- AI text generation  
- Workflow automation  

---

## Future Enhancements

Possible improvements:

- Publishing to internal knowledge portals
- RAG ingestion pipeline
- Slack / Teams approval notifications
- Version tracking
- automated summarization


