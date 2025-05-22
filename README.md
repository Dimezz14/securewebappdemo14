# Secure Web App Demo - Azure Static Web Apps

[![Azure Static Web Apps](https://img.shields.io/badge/Azure%20Static%20Web%20Apps-Free-blue)](https://azure.microsoft.com/en-us/services/app-service/static/)
[![GitHub](https://img.shields.io/github/license/Dimezz14/securewebappdemo14)](https://github.com/Dimezz14/securewebappdemo14/blob/main/LICENSE)

## Project Overview

This project demonstrates how to deploy a **secure static web app** using **Azure Static Web Apps**. The app consists of a simple **HTML** page and is hosted in the **Central US** region with the **free tier** of Azure Static Web Apps. It is designed for use as a sample project showcasing **CI/CD** deployment through GitHub Actions, and is intended for demonstrating basic **Azure Static Web App** functionality for small-scale personal or professional web projects.

### Key Features:
- **Static Web App Deployment**: Uses Azure Static Web Apps to deploy an HTML site with no backend.
- **CI/CD Pipeline**: Automates deployment with GitHub Actions directly from a GitHub repository.
- **Free Tier Hosting**: Deployed using Azure’s **Free Tier**, ensuring cost-free hosting for small projects.

## Technologies Used:
- **Azure Static Web Apps** for fast, secure, and scalable web hosting.
- **GitHub Actions** for automated CI/CD pipeline integration.
- **HTML5**, no backend required.

## Project Setup & Deployment

### Prerequisites:
1. **Azure CLI** installed on your local machine.
2. A **GitHub** account to host your repository and configure the pipeline.
3. A **Personal Access Token (PAT)** for GitHub authentication (if needed).

### Deploying Your Own Static Web App:

1. Clone or fork this repository:
   ```bash
   git clone https://github.com/YOUR_USERNAME/securewebappdemo14.git
2. Push your project to GitHub if you haven't already.
3. Push your project to GitHub if you haven't already.

az staticwebapp create \
  --name securewebappdemo14 \
  --resource-group secure-webapp-rg \
  --location "Central US" \
  --source https://github.com/YOUR_USERNAME/securewebappdemo14 \
  --branch main \
  --app-location "/" \
  --output-location "/" \
  --sku Free

4. Visit your live URL after the deployment is complete:
https://YOUR_APP_NAME.azurestaticapps.net
