---
# generated by https://github.com/hashicorp/terraform-plugin-docs
page_title: "tfepatch Provider"
subcategory: ""
description: |-
  Terraform provider to patch/work alongside the TFE for resources/data sources that are yet to be implemented
---

# tfepatch Provider

Terraform provider to patch/work alongside the TFE for resources/data sources that are yet to be implemented

## Example Usage

```terraform
provider "tfepatch" {
  hostname        = "https://app.terraform.io"
  token           = "abcde12345"
  organization    = "gruntwork-corp"
  ssl_skip_verify = false
}
```

<!-- schema generated by tfplugindocs -->
## Schema

### Required

- `hostname` (String) The Terraform Enterprise hostname to connect to. Defaults to app.terraform.io.
- `organization` (String) The organization to apply to a resource if one is not defined on the resource itself.
- `token` (String, Sensitive) The token used to authenticate with Terraform Enterprise. We recommend omitting the token which can be set as credentials in the CLI config file.

### Optional

- `ssl_skip_verify` (Boolean) Whether or not to skip certificate verifications.
