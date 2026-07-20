# LAB | Post-project Review — Stakeholders & Real-world Scope

## Part 1 – Project Snapshot

### Project: MoveFlow

# LAB | Post-project Review — Stakeholders & Real-world Scope

**Project:** MoveFlow

---

# Part 1 – Project Snapshot

## Project Overview

MoveFlow is an AI-powered active learning companion that transforms educational documents and YouTube videos into personalized walking podcasts. Instead of spending long periods reading or watching videos, users can upload learning material, and the AI generates a podcast designed to be listened to while walking.

The intended users are students, professionals, and lifelong learners who want a more engaging and healthier way to learn. Our MVP allows users to upload PDF, DOCX, or TXT files, or paste a YouTube link, and receive an AI-generated podcast with background music through a Gradio interface.

---

# Part 2 – Stakeholder Impact

| Stakeholder | Role / Relationship | What They Need | Risk if Ignored | Influence | Interest |
|-------------|--------------------|----------------|-----------------|-----------|----------|
| End Users | Primary users | Accurate summaries, easy interface, reliable podcast generation | Low adoption and poor user experience | High | High |
| Client / Organization | Project sponsor | Product that meets business goals | Product may not solve the intended problem | High | High |
| Development Team | Builds and maintains the application | Clear requirements and documentation | Technical debt and maintenance issues | High | High |
| AI API Providers | External service providers | Proper API usage and secure authentication | API failures and service interruptions | High | Medium |
| Data Privacy Team | Compliance and governance | Secure handling of uploaded files and GDPR compliance | Privacy violations and legal issues | High | Medium |
| Customer Support | Supports end users | Documentation and troubleshooting procedures | Increased support workload | Medium | High |
| Accessibility Users | Users with accessibility needs | Accessible interface and controls | Some users cannot effectively use the application | Low | High |
| Finance Department | Controls project budget | Predictable infrastructure and API costs | Unexpected operating expenses | Medium | Medium |

---

# Part 3 – From Demo to a Real Project

## Operations

Our classroom demo assumed that developers would manually restart or fix the application if something went wrong. There was no monitoring, logging, or backup strategy.

For a production deployment, we would implement monitoring dashboards, automated backups, application logging, and clear maintenance responsibilities to ensure reliability.

---

## Security & Compliance

The MVP stored API keys in environment variables and accepted uploaded files without extensive security validation. User authentication was not implemented.

A production system would require encrypted storage, secure authentication, role-based access control, secure secret management, and full GDPR compliance because users upload personal documents.

---

## Data Lifecycle

The prototype processed uploaded files only during the session and did not include a formal retention policy.

For production, we would establish clear policies for storing, deleting, and protecting uploaded files. Users should be able to request deletion of their data, and personally identifiable information should be protected throughout processing.

---

## Handoff & Support

The documentation focused mainly on developers and the classroom presentation. There was no long-term maintenance or support plan.

A production project would include technical documentation, administrator guides, user manuals, training materials, and support procedures so future teams can maintain the application.

---

## Scope Beyond the Demo

The prototype assumed ideal conditions, including successful API responses and standard input files. Accessibility and multilingual support were limited.

A production-ready application would include robust error handling, accessibility improvements, multilingual support, fallback behavior when AI services fail, and testing with different file types and user scenarios.

---

# Part 4 – Revision Brief

## Before

At the beginning of the project, success meant creating a working prototype capable of transforming learning materials into AI-generated podcasts. Our primary objective was demonstrating that the concept worked within the project timeframe.

## After

After reviewing the project from a stakeholder perspective, success means much more than demonstrating technical functionality. A production-ready application must also provide secure data handling, reliable infrastructure, accessibility, documentation, maintainability, and long-term user support. Future development should balance new features with operational quality and user trust.

---

# Checklist

- [x] Recognize: Named the project and identified the intended beneficiary.
- [x] Apply: Stakeholder table includes more than six stakeholders with needs, risks, influence, and interest.
- [x] Integrate: Demo-to-production section covers five dimensions with concrete improvements.
- [x] Verify: Before and After sections clearly show how project scope and success criteria evolved.
- [x] Stretch: Included Finance Department as an additional stakeholder.