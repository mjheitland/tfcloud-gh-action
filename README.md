# tfcloud-gh-action

This workflow is GitHub's standard template for Terraform.

It installs the latest version of Terraform CLI and configures the Terraform CLI configuration file with an API token for Terraform Cloud (app.terraform.io). On pull request events, this workflow will run `terraform init`, `terraform fmt`, and `terraform plan` (speculative plan via Terraform Cloud). On push events to the "main" branch, `terraform apply` will be executed.
