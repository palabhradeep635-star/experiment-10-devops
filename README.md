<!-- Premium project README for Experiment 10: Cloud DevOps & CI/CD -->

<div align="center">

# ⚡ Experiment 10 · Cloud DevOps

### Build. Deploy. Automate.

A clean, responsive static website demonstrating the fundamentals of **Continuous Integration and Continuous Deployment (CI/CD)** with GitHub Actions and Azure Static Web Apps.

<br/>

[![Azure Static Web Apps](https://img.shields.io/badge/Live%20Demo-Azure%20Static%20Web%20Apps-0078D4?style=for-the-badge&logo=microsoftazure&logoColor=white)](https://icy-grass-023f90f00.5.azurestaticapps.net)
[![GitHub Actions](https://github.com/palabhradeep635-star/experiment-10-devops/actions/workflows/azure-static-web-apps.yml/badge.svg)](https://github.com/palabhradeep635-star/experiment-10-devops/actions/workflows/azure-static-web-apps.yml)
[![HTML](https://img.shields.io/badge/Built%20with-HTML%2C%20CSS%20%26%20JavaScript-E34F26?style=flat&logo=html5&logoColor=white)](https://github.com/palabhradeep635-star/experiment-10-devops)

<br/>

**[🌐 Visit Live Website](https://icy-grass-023f90f00.5.azurestaticapps.net) · [📦 Browse Source Code](https://github.com/palabhradeep635-star/experiment-10-devops) · [⚙️ View Actions](https://github.com/palabhradeep635-star/experiment-10-devops/actions)**

<br/>

**Created by Abhradeep Pal**  
UID: `25BAI70056`

</div>

---

## ✨ Project Overview

This experiment demonstrates how a static web application can be maintained in GitHub and deployed to the cloud through an automated CI/CD workflow.

Instead of manually uploading every website update, a push to the `main` branch triggers **GitHub Actions**, which runs the Azure Static Web Apps deployment action. When the workflow completes successfully, the updated site is published to the configured Azure Static Web Apps resource.

### Objectives

- Understand the purpose of cloud-based DevOps and CI/CD.
- Store and track website source code with Git and GitHub.
- Automate deployment using a GitHub Actions workflow.
- Host a static website on Azure Static Web Apps.
- Verify deployments through workflow run status and the live website.

## 🚀 Highlights

| Feature | Description |
| --- | --- |
| **Static website** | Lightweight HTML, CSS, and JavaScript application. |
| **Cloud hosting** | Public deployment on Azure Static Web Apps. |
| **Automated deployment** | GitHub Actions workflow triggered by pushes to `main`. |
| **Manual run option** | Workflow also supports `workflow_dispatch` from GitHub Actions. |
| **Responsive UI** | Designed to adapt to desktop and mobile screens. |
| **Student details** | Credits the project to Abhradeep Pal, UID `25BAI70056`. |

## 🔁 CI/CD Workflow

```text
Developer updates index.html
          │
          ▼
    Commit and push
       to GitHub
          │
          ▼
   GitHub Actions starts
          │
          ▼
 Checkout repository files
          │
          ▼
 Azure Static Web Apps
    deployment action
          │
          ▼
  Updated live website
```

The workflow is configured in `.github/workflows/azure-static-web-apps.yml`. It deploys the static files from the repository root and skips a separate application build step.

## 🧰 Technology Stack

- **HTML5** — website structure
- **CSS3** — layout, styling, responsive design, and visual effects
- **JavaScript** — client-side interactions
- **Git & GitHub** — source control and repository hosting
- **GitHub Actions** — workflow automation
- **Azure Static Web Apps** — static website hosting and deployment

## 📁 Repository Structure

```text
experiment-10-devops/
├── .github/
│   └── workflows/
│       └── azure-static-web-apps.yml  # Active GitHub Actions deploy workflow
├── index.html                         # Website entry point
├── azure-pipelines.yml                # Azure Pipelines build-artifact example
├── buildspec.yml                      # AWS CodeBuild build specification
└── README.md                          # Project documentation
```

### About the deployment configuration files

- **`.github/workflows/azure-static-web-apps.yml`** — the workflow used for the GitHub Actions deployment route to Azure Static Web Apps.
- **`azure-pipelines.yml`** — a separate Azure Pipelines configuration. The current file archives repository files and publishes a build artifact; it does not independently deploy the site to Azure Static Web Apps.
- **`buildspec.yml`** — an AWS CodeBuild specification example. It is separate from the active GitHub Actions deployment route.

Keeping these configurations separate helps avoid confusing the CI/CD tools used by different cloud platforms.

## 🖥️ Run Locally

No package manager or build tool is required for the static website.

1. Clone the repository:

   ```bash
   git clone https://github.com/palabhradeep635-star/experiment-10-devops.git
   ```

2. Open the project directory:

   ```bash
   cd experiment-10-devops
   ```

3. Open `index.html` in a browser, or use the Live Server extension in Visual Studio Code.

## ☁️ How Automatic Deployment Works

1. Confirm that the Azure Static Web Apps resource is connected/configured for this deployment route.
2. Add the Azure deployment token in GitHub under **Settings → Secrets and variables → Actions** with the name `AZURE_STATIC_WEB_APPS_API_TOKEN`.
3. Make your website changes and commit them to the `main` branch.
4. Push the commit to GitHub. The workflow runs automatically on pushes to `main`.
5. Open the **Actions** tab and wait for the run to finish.
6. After a successful run, visit the live URL and refresh the page.

> **Security note:** Never commit the Azure deployment token to the repository or place it in `index.html`. Store it only as a GitHub Actions secret.

### Useful links

- **Live site:** https://icy-grass-023f90f00.5.azurestaticapps.net
- **GitHub repository:** https://github.com/palabhradeep635-star/experiment-10-devops
- **GitHub Actions runs:** https://github.com/palabhradeep635-star/experiment-10-devops/actions
- **Deployment workflow:** https://github.com/palabhradeep635-star/experiment-10-devops/blob/main/.github/workflows/azure-static-web-apps.yml

## ✅ Expected Outcome

The experiment demonstrates a basic automated release process for a static website: source code is stored in GitHub, a workflow is triggered by changes on the main branch, and the deployment action publishes the site to Azure Static Web Apps. A successful workflow run is the primary deployment check; the live URL can then be used to confirm the updated page is accessible.

## 👨‍💻 Author

<div align="center">

### Abhradeep Pal

**UID:** `25BAI70056`  
Cloud DevOps · CI/CD · Static Web Deployment

[GitHub Profile](https://github.com/palabhradeep635-star) · [Project Repository](https://github.com/palabhradeep635-star/experiment-10-devops) · [Live Demo](https://icy-grass-023f90f00.5.azurestaticapps.net)

</div>

---

<div align="center">

*Experiment 10 · Cloud Computing & DevOps*

</div>
