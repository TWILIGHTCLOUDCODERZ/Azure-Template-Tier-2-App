# 🚀 Azure Tier-2 App Deployment

Provision a full **Tier-2 Azure Application Architecture** in minutes using this automated deployment template.

> ✅ Deploys an App Service + SQL Database + Key Vault with secure configuration and managed identity.

---

## 📦 What’s Included:

| Resource               | Purpose                                              |
|------------------------|------------------------------------------------------|
| **App Service Plan**   | Hosts the Web App workload                          |
| **Web App**            | Publicly accessible application with managed identity |
| **SQL Server & DB**    | Backend data layer                                  |
| **Key Vault**          | Securely stores SQL admin password                  |
| **Access Policies**    | Enables the Web App to retrieve secrets securely    |

---

## 🧰 Parameters

| Parameter             | Description                              |
|------------------------|------------------------------------------|
| `webAppName`          | Name of the Web App                      |
| `appServicePlanName`  | Name of the App Service Plan             |
| `sqlServerName`       | Logical SQL Server name                  |
| `sqlAdminUser`        | SQL administrator username               |
| `sqlAdminPassword`    | SQL administrator password (secured)     |
| `sqlDatabaseName`     | Name of the SQL database                 |
| `keyVaultName`        | Key Vault resource name                  |
| `location`            | Azure region (default: West Europe)     |

---

## 🚀 Deploy This Architecture to Azure

<div align="center">
  <a href="https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2FTWILIGHTCLOUDCODERZ%2FAzure-Template-Tier-2-App%2Fmain%2Fazuredeploy.json" target="_blank">
    <img src="https://img.shields.io/badge/Deploy%20to%20Azure-Click%20Here-blue?style=for-the-badge&logo=microsoftazure" alt="Deploy to Azure"/>
  </a>
</div>

---

## 🤖 Need Help Designing Your Architecture?

Launch the **AI Architect Assistant** below to get tailored guidance for your cloud architecture needs:

<div align="center">
  <a href="https://twilightcloudcoderz.github.io/AI-ARCHITECT-ASSISTANT/" target="_blank">
    <img src="https://img.shields.io/badge/Launch%20AI%20Architect%20Assistant-Open%20Tool-green?style=for-the-badge&logo=githubpages" alt="Launch AI Assistant"/>
  </a>
</div>

---

## 🔒 Security Highlights

- 🔐 SQL Admin credentials are stored in **Azure Key Vault**
- 🆔 Web App is assigned a **System-Assigned Managed Identity** for secure access
- 🔑 Key Vault access policy is configured dynamically for the Web App identity

---

## 📤 Outputs

| Output Key    | Description                          |
|---------------|--------------------------------------|
| `webAppUrl`   | URL of the deployed Web App          |
| `keyVaultUri` | URI of the deployed Key Vault        |

---


