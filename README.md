# terraform-aws-eks-nodegroup

[![build](https://img.shields.io/github/workflow/status/nalbam/terraform-aws-eks-nodegroup/build?label=build&style=for-the-badge&logo=github)](https://github.com/nalbam/terraform-aws-eks-nodegroup/actions/workflows/push.yaml)
[![release](https://img.shields.io/github/v/release/nalbam/terraform-aws-eks-nodegroup?style=for-the-badge&logo=github)](https://github.com/nalbam/terraform-aws-eks-nodegroup/releases)

<!--- BEGIN_TF_DOCS --->
## Requirements

| Name | Version |
|------|---------|
| terraform | >= 1.1 |
| aws | >= 4.1.0 |

## Providers

| Name | Version |
|------|---------|
| aws | >= 4.1.0 |

## Inputs

| Name | Description | Type | Default | Required |
|------|-------------|------|---------|:--------:|
| ami\_type | n/a | `string` | `"AL2_x86_64"` | no |
| associate\_public\_ip\_address | n/a | `bool` | `false` | no |
| cluster\_name | Name of the cluster. | `string` | n/a | yes |
| ebs\_optimized | n/a | `bool` | `true` | no |
| enable\_monitoring | n/a | `bool` | `true` | no |
| enable\_spot | n/a | `bool` | `false` | no |
| enable\_taints | n/a | `bool` | `false` | no |
| instance\_types | n/a | `list(string)` | `[]` | no |
| key\_name | n/a | `string` | `"eks_user"` | no |
| max | n/a | `number` | `5` | no |
| max\_unavailable\_percentage | n/a | `number` | `20` | no |
| min | n/a | `number` | `1` | no |
| name | Name of the worker. e.g: worker | `string` | n/a | yes |
| node\_labels | n/a | `map(string)` | `{}` | no |
| node\_role\_arn | n/a | `string` | n/a | yes |
| security\_groups | n/a | `list(string)` | `[]` | no |
| subname | Subname of the worker, e.g: a | `string` | `""` | no |
| subnet\_ids | n/a | `list(string)` | n/a | yes |
| tags | n/a | `map(string)` | `{}` | no |
| vername | Version of the worker, e.g: v1 | `string` | `""` | no |
| volume\_size | n/a | `string` | `"50"` | no |
| volume\_type | n/a | `string` | `"gp2"` | no |

## Outputs

No output.

<!--- END_TF_DOCS --->
