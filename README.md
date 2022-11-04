## Google lab to manage infra with tf scripts

* Creating s3 bucket so same state file
* Migrating local state file to s3 bucket
* Adding subnets, vpc, module from remote registry
* Passing variables to simple module.

## Requirements

| Name | Version |
|------|---------|
| <a name="requirement_google"></a> [google](#requirement\_google) | 3.55.0 |

## Providers

| Name | Version |
|------|---------|
| <a name="provider_google"></a> [google](#provider\_google) | 3.55.0 |

## Modules

| Name | Source | Version |
|------|--------|---------|
| <a name="module_instances"></a> [instances](#module\_instances) | ./modules/instances | n/a |
| <a name="module_network"></a> [network](#module\_network) | terraform-google-modules/network/google | 3.4.0 |
| <a name="module_storage"></a> [storage](#module\_storage) | ./modules/storage | n/a |

## Resources

| Name | Type |
|------|------|
| [google_compute_firewall.tf-firewall](https://registry.terraform.io/providers/hashicorp/google/3.55.0/docs/resources/compute_firewall) | resource |

## Inputs

| Name | Description | Type | Default | Required |
|------|-------------|------|---------|:--------:|
| <a name="input_project_id"></a> [project\_id](#input\_project\_id) | n/a | `string` | `"id"` | no |
| <a name="input_region"></a> [region](#input\_region) | n/a | `string` | `"europe-central2"` | no |
| <a name="input_vpc_name"></a> [vpc\_name](#input\_vpc\_name) | n/a | `string` | `"tf-vpc-707736"` | no |
| <a name="input_zone"></a> [zone](#input\_zone) | n/a | `string` | `"europe-central2-c"` | no |

## Outputs

No outputs.
