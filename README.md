# 🚀 Infracost GitHub Action

![Release](https://github.com/subhamay-bhattacharyya-gha/infracost-action/actions/workflows/release.yaml/badge.svg)&nbsp;
![Commit Activity](https://img.shields.io/github/commit-activity/t/subhamay-bhattacharyya-gha/infracost-action)&nbsp;
![Last Commit](https://img.shields.io/github/last-commit/subhamay-bhattacharyya-gha/infracost-action)&nbsp;
![Release Date](https://img.shields.io/github/release-date/subhamay-bhattacharyya-gha/infracost-action)&nbsp;
![Repo Size](https://img.shields.io/github/repo-size/subhamay-bhattacharyya-gha/infracost-action)&nbsp;
![File Count](https://img.shields.io/github/directory-file-count/subhamay-bhattacharyya-gha/infracost-action)&nbsp;
![Issues](https://img.shields.io/github/issues/subhamay-bhattacharyya-gha/infracost-action)&nbsp;
![Top Language](https://img.shields.io/github/languages/top/subhamay-bhattacharyya-gha/infracost-action)&nbsp;
![Custom Endpoint](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/bsubhamay/68d0048cc82fdd049535383c9b836ec7/raw/infracost-action.json?)

This GitHub Action downloads a Terraform plan artifact and runs [Infracost](https://www.infracost.io/) to generate a cost estimate. It supports workflows where the Terraform plan is created in a separate job or workflow, and reused across CI/CD stages.

It also supports dynamic cost thresholding (`max_cost`) using a GitHub Gist that maps environments and repositories to their cost budgets.

---

## 🧾 Inputs

| Name                | Description                                                                 |
|---------------------|-----------------------------------------------------------------------------|
| `terraform-dir`     | Relative path to the Terraform directory (e.g., `tf`, `infrastructure`).    |
| `release-tag`       | Git release tag to check out. If omitted, the latest commit is used.        |
| `ci-pipeline`       | If `true`, includes the commit SHA in the Terraform state key.              |
| `s3-bucket`         | Name of the S3 bucket used for the Terraform state backend.                 |
| `s3-region`         | AWS region where the S3 backend bucket is located (e.g., `us-east-1`).      |
| `tf-plan-name`      | Name of the Terraform plan artifact.                                        |
| `tf-plan-file`      | Base filename (without extension) for the Terraform plan output.            |
| `tf-vars-file`      | Optional Terraform variable file.                                           |
| `infracost-api-key` | Infracost API key.                                                          |
| `gist-id`           | Gist ID containing the Infracost configuration (e.g., repository/env → max cost). |
| `gist-filename`     | Gist filename (default: `infracost-config.json`).                           |
| `environment`       | GitHub environment name (e.g., `dev`, `test`, `prod`) used to look up max cost. |
| `max-cost`          | Optional fallback cost threshold. Used if not found in Gist (e.g., `100.00`).|

---

## 📤 Outputs

| Name            | Description                                                     |
|------------------|-----------------------------------------------------------------|
| `monthly-cost`   | Total monthly cost calculated by Infracost.                     |
| `max-cost`       | Resolved maximum cost threshold from Gist or fallback value.    |

---

## 💡 Example Usage

```yaml
name: Infracost Breakdown

on:
  workflow_dispatch:

jobs:
  infracost:
    runs-on: ubuntu-latest
    permissions:
      id-token: write
      contents: read
    steps:
      - name: Run Infracost Analysis
        uses: subhamay-bhattacharyya-gha/infracost-action@main
        with:
          terraform-dir: tf
          release-tag: ""
          ci-pipeline: "true"
          s3-bucket: my-terraform-state-bucket
          s3-region: us-east-1
          tf-plan-name: terraform-plan
          tf-plan-file: tfplan
          tf-vars-file: terraform.tfvars
          infracost-api-key: ${{ secrets.INFRACOST_API_KEY }}
          gist-id: ${{ secrets.infracost-gist-id }}
          gist-filename: ${{ secrets.gist-filename }}
          environment: devl
```

## 🧠 Gist JSON Format Example

```json
{
  "0002-terraform-template": {
    "ci": { "max_cost": 1.99 },
    "devl": { "max_cost": 1.00 },
    "test": { "max_cost": 20.00 },
    "prod": { "max_cost": 80.00 }
  },
  "data-lake": {
    "devl": { "max_cost": 4.00 },
    "test": { "max_cost": 10.00 },
    "prod": { "max_cost": 100.00 }
  }
}
```

---

## 🪪 License

MIT