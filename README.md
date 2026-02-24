# Pathology-HIMF-Tracking-App

clinical-inventory-digital-transformation

*HIMF refers to Health Item Masterfile

Pathology Reagent Lifecycle & HIMF Tracking App

[View Project →](https://apps.powerapps.com/play/e/default-a687a7bf-02db-43df-bcbb-e7a8bda611a2/a/321567a2-b676-4a58-97e0-8fa4910dd64e?tenantId=a687a7bf-02db-43df-bcbb-e7a8bda611a2&hint=52f07e2a-b9fb-44b2-9a71-2dceda0e97f5&sourcetime=1771880669790)

Overview

A Power Apps–based clinical inventory management solution designed to digitise reagent intake, track HIMF numbers, monitor expiry dates, and reduce wastage across pathology laboratories.
Built to support ISO 15189-compliant workflows and scalable across multi-site lab networks.
________________________________________
Problem

Pathology laboratories frequently rely on manual logs or fragmented Excel systems to:
* Track reagent lot numbers and HIMF identifiers
* Monitor expiry dates
* Capture supplier data
* Record intake timestamps
* Prevent reagent wastage

This creates:
*	Data inconsistency
* Compliance risk
* Increased manual workload
* Reduced audit transparency

________________________________________

Solution
A Power Apps application integrated with SharePoint that enables:
* Barcode-based reagent lookup
* HIMF auto-population
* Expiry date tracking
* Supplier and category dropdown logic
* Multi-lab scalability
* SharePoint backend data storage
* Audit-friendly structured data capture

________________________________________


Architecture
* Frontend: Microsoft Power Apps (Canvas App)
* Backend: SharePoint List (tblInventory)
* Optional Automation: Power Automate expiry alerts
* Deployment: Teams / Web browser / Managed iPad device

________________________________________

Key Features
* Reagent intake form with structured validation
* Conditional dropdown visibility
* Barcode scanner integration
* Expiry threshold alerts
* Dynamic filtering by lab/site
* Change-item override functionality
* Scalable site-level architecture

________________________________________

Impact
* Reduced manual entry errors
* Improved reagent visibility
* Enhanced compliance readiness
* Standardised digital intake process
* Designed for state-level pathology scalability

________________________________________

Compliance Context
* Designed within ISO 15189 and NATA/NPAAC operational frameworks.

__________________________________________


Technical Design
Data Model

The application is powered by a SharePoint list (tblInventory) structured to support clinical-grade traceability.

Core fields include:

  1. Item Name
  2. HIMF Number
  3. Lot Number
  4. Supplier
  5. Category
  6. Received Date
  7. Expiry Date
  8. Site / Lab Location
  9. Quantity
  10. Status (Active / Expired / Consumed)

The schema was designed to ensure:

  * Standardised structured data entry
  * Audit traceability
  * Compatibility with Power BI reporting
  * Scalability across multiple laboratory sites

_________________________________________________________________________


Business Logic

The application includes embedded logic to support safe clinical workflows:

  * Conditional dropdown population based on selected category
  * HIMF auto-lookup using barcode scan
  * Change-item override reset variables
  * Expiry threshold flagging
  * Site-level filtering capability
  * Validation rules prevent incomplete or non-compliant entries.
  * Deployment Model

The application is deployed via:

  * Microsoft Teams
  * Web browser access
  * Managed iPad device

Backend data is stored in SharePoint to ensure:

  * Organisational control
  * Role-based permissions
  * Centralised governance
  * Audit traceability

____________________________________________________________________

Use Case Scenario

A reagent shipment is received at a pathology laboratory.

  1. Staff scan the barcode on the reagent box.
  2. HIMF and item data auto-populate.
  3. Lot number and expiry date are entered.
  4. The entry is validated and stored in SharePoint.
  5. Expiry tracking logic flags reagents nearing threshold.
  6. Data becomes immediately available for reporting or compliance audit.

This replaces manual Excel logging and reduces transcription error risk.

_______________________________________________________________________

Scalability Strategy

The application architecture supports state-level expansion by:

  * Allowing each laboratory to operate with site-level filtering
  * Using a centralised SharePoint structure
  * Supporting future migration to Azure SQL
  * Enabling Power BI integration for cross-site reporting
    
The model is designed to scale from single-site deployment to multi-laboratory network environments.

_________________________________________________________________________________

Governance & Risk Mitigation

  * Structured data capture reduces compliance risk.
  * Expiry tracking reduces reagent wastage.
  * Centralised storage supports audit readiness.
  * Standardised fields prevent inconsistent naming conventions.
  * Role-based access ensures data integrity.
    
Designed in alignment with ISO 15189 quality management principles.

____________________________________________________________________________________
Lessons Learned

  * User adoption improves when workflow friction is minimised.
  * Dropdown standardisation reduces downstream reporting errors.
  * Barcode integration significantly reduces manual transcription mistakes.
  * Early architecture decisions impact scalability.

__________________________________________________________________________

Future Enhancements
 * OCR-based label scanning
 * Azure SQL backend migration
 * Power BI real-time dashboard integration
 * Predictive reagent ordering model
 * State-wide multi-site deployment
