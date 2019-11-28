# terraform-module-kubernetes-azure-resources-exporter
Terraform module for azure-resources-exporter

## Usage
See `examples` folders for usage of this module.

<!-- BEGINNING OF PRE-COMMIT-TERRAFORM DOCS HOOK -->
## Inputs

| Name | Description | Type | Default | Required |
|------|-------------|:----:|:-----:|:-----:|
| annotations | Additionnal annotations that will be merged on all resources. | map | `{}` | no |
| client\_id | Client ID that will be used by the snapshot-manager. | string | n/a | yes |
| client\_secret | Client secret that will be used by the snapshot-manager. | string | n/a | yes |
| config\_map\_annotations | Additionnal annotations that will be merged for the config map. | map | `{}` | no |
| config\_map\_labels | Additionnal labels that will be merged for the config map. | map | `{}` | no |
| config\_map\_name | Name of the config map that will be created. | string | `"azure-resources-exporter"` | no |
| image\_pull\_policy | Image pull policy on the main container. | string | `"IfNotPresent"` | no |
| image\_version | Version of the docker image | string | `"0.1.0"` | no |
| labels |  | map | `{}` | no |
| namespace | Kubernetes namespace in which to deploy the ecosystem, | string | `"default"` | no |
| namespace\_annotations | Annotations to apply to the namespace. | map | `{}` | no |
| namespace\_labels | Labels to apply to the namespace. | map | `{}` | no |
| secret\_annotations | Additionnal annotations that will be merged for the secret. | map | `{}` | no |
| secret\_labels | Additionnal labels that will be merged for the secret. | map | `{}` | no |
| secret\_name | Name of the secret that will be created. | string | `"azure-resources-exporter"` | no |
| subscription\_id | Subscription ID that will be used by the snapshot-manager. | string | n/a | yes |
| tenant\_id | Tenant ID that will be used by the snapshot-manager. | string | n/a | yes |

<!-- END OF PRE-COMMIT-TERRAFORM DOCS HOOK -->

Thanks
