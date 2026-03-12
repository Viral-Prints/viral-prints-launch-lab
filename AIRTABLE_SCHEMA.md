# Airtable Schema

## Purpose

This file defines the recommended Airtable structure for managing Viral Prints operations.

The goal is to support the Phase 1 workflow while leaving room for future client portal, reporting, and multi-location features.

---

## Core Tables

### 1. Customers
Suggested fields:
- Customer ID
- full name
- business name
- email
- phone
- website
- address
- preferred contact method
- notes

### 2. Projects
Suggested fields:
- Project ID
- linked customer
- project status
- package tier
- design path
- wall type
- location type
- dimensions
- install preferences
- target date
- disruption notes
- internal notes

### 3. Payments
Suggested fields:
- linked project
- deposit required
- deposit paid
- final balance due
- final balance paid
- Stripe link or invoice reference
- donation added
- payment notes

### 4. Proofs
Suggested fields:
- linked project
- proof version
- sent date
- proof file
- approval status
- revision requested
- revision notes
- final approval date

### 5. Referrals
Suggested fields:
- linked project
- referral link
- QR code file
- QR placement notes
- scans
- referred leads
- referral notes

---

## Suggested Status Fields

### Project Status
- new inquiry
- under review
- quote pending
- awaiting deposit
- in design
- proof sent
- revisions requested
- approved
- install scheduled
- completed
- closed

### Approval Status
- not sent
- sent
- approved
- revision requested

### Payment Status
- not sent
- deposit sent
- deposit paid
- final invoice sent
- paid in full

---

## Future-Proofing Notes

The schema should be structured so later features can be added without rebuilding, including:
- client portal
- admin dashboards
- analytics
- role permissions
- multi-location support
- franchise workflows

---

## Build Notes

The schema should prioritize:
- linked records
- clean status logic
- easy filtering
- simple reporting
- scalable project organization
