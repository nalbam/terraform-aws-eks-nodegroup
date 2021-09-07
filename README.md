# terraform-aws-eks-nodegroup

<!--- BEGIN_TF_DOCS --->
## Requirements

| Name | Version |
|------|---------|
| terraform | >= 0.13 |
| aws | >= 3.30.0 |

## Providers

| Name | Version |
|------|---------|
| aws | >= 3.30.0 |

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
