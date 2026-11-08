<div align="center">

# Param ERP

**Project accounting ERP for a construction and infrastructure contractor.**

![Java 21](https://img.shields.io/badge/Java%2021-ED8B00?style=flat-square&logo=openjdk&logoColor=white) ![Spring Boot](https://img.shields.io/badge/Spring%20Boot-6DB33F?style=flat-square&logo=springboot&logoColor=white) ![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white) ![Flyway](https://img.shields.io/badge/Flyway-CC0200?style=flat-square&logo=flyway&logoColor=white) ![Firebase](https://img.shields.io/badge/Firebase-DD2C00?style=flat-square&logo=firebase&logoColor=white)

</div>

> [!NOTE]
> **Showcase repository.** This is client work built at Runtime Solutions, and its source code is private. This page documents the product, my role and the engineering behind it.

## Overview

Param runs the finance side of large construction projects: tenders and EMDs, bank guarantees, purchases and deliveries, rental, transport, sub-contractor and service bills, staff and site expenses, salaries, and the accounting views (job charts, trial balance, debtor ageing) the finance team closes the books with.

## My role

**Backend developer**: about 85 commits on bills and payments, accounting reports, staff modules and performance.

## Tech stack

| Layer | Technologies |
|---|---|
| Backend | Java 21, Spring Boot, Spring Security, Spring Data JPA, Hibernate Envers |
| Data | MySQL, Flyway |
| Documents | iText, Apache POI, RFC 4180 CSV |
| Platform | Firebase push, Sentry, S3-compatible storage, GitHub Actions |

## What I built

- **Bill payments** across rental, car rental, sub-contractor, service and transportation bills: advance/direct payments, credit/debit notes, RCM fields and filtering by bill and party.
- **Accounting**: job charts, project charts, fixed assets, expenses and receipts, trial-balance accessory breakdowns with linked logs, and debtor ageing with multi-project filters.
- **Purchasing**: purchase invoices with item-wise GST and TDS (including on inspection charges), railway bills, and multiple call letters and IC details per item.
- **Staff & sites**: staff authentication, project/site assignment, salary data and office-staff bifurcation.
- **Exports**: RFC 4180-compliant CSV exports for expenses and staff payments.

## Engineering highlights

- **Eliminated N+1 queries** in bills, staff accounting and expenses with pagination-first batch loading.
- **Faster dashboards**: sections load in parallel, and full table scans were replaced with lean SQL count/sum aggregates.
- **Dynamic enums** for banks and guarantee types so business users can extend options without a deployment.

---

<div align="center">

**Priyansu Chowdhury**: Backend-leaning full-stack developer (Java / Spring Boot · Next.js / TypeScript)

[LinkedIn](https://linkedin.com/in/priyansu-chowdhury) · [GitHub](https://github.com/Pr1yansu)

</div>
