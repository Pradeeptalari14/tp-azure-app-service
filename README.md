# Azure App Service Deployer

This repository contains the target configuration and SRE runtime files compiled by the **Azure App Service Deployer** dashboard module.

## 🚀 Description
Configure highly available Azure App Service plans. Generate slot deployments configurations, custom domain binds, dynamic logging profiles, and scaling templates.

## 🛠️ Specification Matrix
- **Primary Configuration File**: `/infra/appservice/webapp_config.tf`
- **Execution Command**: `terraform init && terraform apply -auto-approve`
- **Validation Command**: `terraform show`

## 📋 How to Run & Validate

1. **Clone the repository:**
   ```bash
   git clone https://github.com/Pradeeptalari14/tp-azure-app-service.git
   cd tp-azure-app-service
   ```

2. **Run Execution Target:**
   ```bash
   terraform init && terraform apply -auto-approve
   ```

3. **Verify Runtime Stability:**
   ```bash
   terraform show
   ```

## 🔐 Security & Best Practices
* **Secret Isolation**: Use organization-level secrets (or SSM parameter hooks) rather than hardcoded environment variables inside files.
* **Pull Request Lifecycles**: Protect default branch merges with validation checks before merging code changes.
