# Run JMeter Tests for Sitecore

This GitHub Actions workflow runs Apache JMeter load tests against Sitecore environments and generates performance reports.

## 🔧 Environments

- **UAT**  
  - URL: `ractest-com-au`  
  - Runner: `digital-npe-ubuntu-latest`

- **PRD**  
  - URL: `sitecore-prd-cd.azurewebsites.net`  
  - Runner: `digital-prd-windows-latest`

## 🚀 Features

- Installs Apache JMeter in the workflow runner
- Runs load tests against the selected environment
- Generates results in both CSV and HTML formats
- Uploads the test results as workflow artifacts

## 📂 Output Files

- `results.csv` – Raw JMeter result data
- `HTML/index.html` – Full HTML report with metrics and graphs

## ▶️ How to Use

1. Trigger the workflow manually or via push/merge to a branch.
2. Select the appropriate environment (UAT or PRD) if using manual dispatch.
3. Wait for the workflow to complete.
4. Download the artifacts from the GitHub Actions run.
