<!-- BEGIN_TF_DOCS -->
# This module does NOT create a tenant, the tenant needs to already be present
# This Module WILL deploy additional components into the tenant name referenced
# These components should be passed as lists or structs and are all optional

To run this example you need to execute:
```bash
$ terraform init
$ terraform plan
$ terraform apply
```
Note that this example will create resources. Resources can be destroyed with `terraform destroy`.
```hcl
module "aci_tenant" {
  source  = "qzx/tenant/aci"
  version = "1.0.0"

  tenant_name = "example"
}
```
<!-- END_TF_DOCS -->