# Team-A-Morning-
IT Services web application project. 
Team Lead/Cloud Architect: Robert Roberts
App & Front End Engineer: Jesus Ortiz
Security & Network Engineer: Jose Leon
DevOps & Backend Engineer: Eric Green
https://mretgreen.github.io/Team-A-Morning-/

  
# Backend Documentation (Azure)

This folder contains all documentation for the planned backend hosted on Microsoft Azure.

## Contents
- [Architecture Overview](architecture-overview.md)
- [Azure Services](azure-services.md)
- [API Design](api-design.md)
- [Deployment Plan](deployment-plan.md)
- [Security](security.md)


---
**Last Updated:** YYYY-MM-DD


# Architecture Overview

## High-Level Diagram
```mermaid
graph TD
    ClientApp[Frontend] --> API[Azure App Service API]
    API --> DB[Azure SQL Database]
    API --> Blob[Azure Blob Storage]
    API --> Queue[Azure Service Bus]
    Queue --> Worker[Azure Functions]


---

## **📄 azure-services.md**
```markdown
# Azure Services Inventory

| Service Name         | Type                  | Purpose                               | SKU / Tier | Region  | Notes |
|----------------------|-----------------------|----------------------------------------|------------|---------|-------|
| Backend API          | Azure App Service     | Hosts REST API backend                 | P1V2       | East US | Node.js 18 |
| Database             | Azure SQL Database    | Stores application data                | S2         | East US | Geo-redundant backup |
| Storage              | Azure Blob Storage    | File and static asset storage          | Hot Tier   | East US | Private endpoint enabled |
| Messaging            | Azure Service Bus     | Message queue for async processing     | Standard   | East US | |
| Authentication       | Azure AD B2C          | Identity and access management         | N/A        | Global  | |
| Secrets Management   | Azure Key Vault       | Secure storage of API keys & secrets   | Standard   | East US | |

---
**Last Updated:** YYYY-MM-DD
