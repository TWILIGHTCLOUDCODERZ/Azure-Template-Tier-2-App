# 🚀 Azure Tier-2 App Deployment

This repository contains an ARM template that provisions a **Tier-2 Azure application**, including:

- 🌐 Azure App Service (Web App)
- 🗄️ Azure SQL Database
- 🔐 Azure Key Vault for secure secret management

---

## 📦 What's Deployed

| Resource               | Purpose                                              |
|------------------------|------------------------------------------------------|
| **App Service Plan**   | Hosting infrastructure for the Web App              |
| **Web App**            | Application runtime with system-assigned identity   |
| **SQL Server & DB**    | Backend relational data storage                     |
| **Key Vault**          | Stores SQL admin password securely                  |
| **Access Policies**    | Grants Web App identity access to Key Vault secrets |

---

## 🧰 Parameters Used

| Parameter             | Description                              |
|------------------------|------------------------------------------|
| `webAppName`          | Name for the Web App                     |
| `appServicePlanName`  | Hosting plan for the Web App             |
| `sqlServerName`       | Logical SQL Server name                  |
| `sqlAdminUser`        | SQL Server administrator login           |
| `sqlAdminPassword`    | SQL Server administrator password (secret) |
| `sqlDatabaseName`     | SQL Database name                        |
| `keyVaultName`        | Key Vault to store SQL credentials       |
| `location`            | Azure region for deployment              |

---

## ✅ Deploy Now

Click the button below to deploy the Tier-2 Web + SQL App into your Azure environment via the Azure Portal:

[![Deploy to Azure](https://aka.ms/deploytoazurebutton)](https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2FTWILIGHTCLOUDCODERZ%2FAzure-Template-Tier-2-App%2Fmain%2Fazuredeploy.json)

> 📝 Make sure to provide secure values (like the SQL admin password) during deployment.

---

## 🔒 Security

- Secrets like the SQL admin password are stored securely in **Azure Key Vault**
- Web App is granted access to fetch secrets via **Managed Identity**

---

## 📤 Outputs After Deployment

- `webAppUrl`: Access URL of the deployed Web App
- `keyVaultUri`: URI to your deployed Key Vault

---

## 📁 Folder Structure

