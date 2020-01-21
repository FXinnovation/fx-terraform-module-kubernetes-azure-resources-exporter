# terraform-module-kubernetes-azure-resources-exporter
Terraform module for azure-resources-exporter

## Usage
See `examples` folders for usage of this module.

<!-- BEGINNING OF PRE-COMMIT-TERRAFORM DOCS HOOK -->
## Inputs

| Name | Description | Type | Default | Required |
|------|-------------|:----:|:-----:|:-----:|
| annotations | Additionnal annotations that will be merged on all resources. | map | `{}` | no |
| client\_id | Client ID that will be used by the azure-resources-exporter. | string | n/a | yes |
| client\_secret | Client secret that will be used by the azure-resources-exporter. | string | n/a | yes |
| config\_map\_annotations | Additionnal annotations that will be merged for the config map. | map | `{}` | no |
| config\_map\_labels | Additionnal labels that will be merged for the config map. | map | `{}` | no |
| config\_map\_name | Name of the config map that will be created. | string | `"azure-resources-exporter"` | no |
| configuration | Configuration to use for azure-resources-exporter \(must be a map\). | map | `{}` | no |
| deployment\_annotations | Additionnal annotations that will be merged on the deployment. | map | `{}` | no |
| deployment\_labels | Additionnal labels that will be merged on the deployment. | map | `{}` | no |
| deployment\_name | Name of the deployment that will be create. | string | `"azure-resources-exporter"` | no |
| enabled | Whether or not to enable this module. | string | `"true"` | no |
| image\_pull\_policy | Image pull policy on the main container. | string | `"IfNotPresent"` | no |
| labels | Additionnal labels that will be merged on all resources. | map | `{}` | no |
| namespace | Namespace in which the module will be deployed. | string | `"default"` | no |
| port | Port to be used for the service. | string | `"80"` | no |
| replicas | Number of replicas to deploy. | string | `"1"` | no |
| secret\_annotations | Additionnal annotations that will be merged for the secret. | map | `{}` | no |
| secret\_labels | Additionnal labels that will be merged for the secret. | map | `{}` | no |
| secret\_name | Name of the secret that will be created. | string | `"azure-resources-exporter"` | no |
| service\_annotations | Additionnal annotations that will be merged for the service. | map | `{}` | no |
| service\_labels | Additionnal labels that will be merged for the service. | map | `{}` | no |
| service\_name | Name of the service that will be create | string | `"azure-resources-exporter"` | no |
| subscription\_id | Subscription ID that will be used by the azure-resources-exporter. | string | n/a | yes |
| tenant\_id | Tenant ID that will be used by the azure-resources-exporter. | string | n/a | yes |

## Outputs

| Name | Description |
|------|-------------|
| config\_map\_name | Name of the config\_map created by this module. |
| deployment\_name | Name of the deployment created by this module. |
| namespace | Namespace in which the module is deployed. |
| port | Port on which the service listens. |
| secret\_name | Name of the secret created by this module. |
| service\_name | Name of the service created by this module. |

<!-- END OF PRE-COMMIT-TERRAFORM DOCS HOOK -->
