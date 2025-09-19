# CISY 5183 2025 Guided Lab 1 - Onboarding and Storage Essentials

This repository contains the exported ARM template from my Azure resource group deployment for **Lab 1**.

## Resource Group
- **Name:** `rg-lab01-ek`
- **Export Method:** Azure Portal → Resource Group → Export template (Automation Script)

## Included
- Storage account (Standard_LRS) configuration  
- Secure settings (TLS 1.2, HTTPS required, public blob access disabled)  
- Lifecycle management rule (move base blobs to Cool tier after 30 days)

## Not Included
- Blob data (e.g., `hello.txt`)
- Container-level settings such as container creation, immutability policy (may not be captured by Azure export)

## Purpose
This export documents the resource configuration for auditing, reproducibility, and re-deployment.  
It also serves as a baseline for Infrastructure as Code (IaC) practices, aligning with **AZ-104** exam objectives.

---

> **Note:** This repository is for educational purposes as part of CISY 5183 Lab 1.  
> All resources have been deleted from Azure after export to avoid unnecessary charges.