# identity-manager

![version: 1.0.0](https://img.shields.io/badge/version-1.0.0-informational?style=flat-square) ![type: application](https://img.shields.io/badge/type-application-informational?style=flat-square) ![app version: 1.0.0](https://img.shields.io/badge/app%20version-1.0.0-informational?style=flat-square)

A Helm chart for Kubernetes

## TL;DR;

```bash
helm repo add invisibl https://charts.invisibl.io
helm install --generate-name --wait invisibl/identity-manager
```

## Values

| Key | Type | Default | Description |
|-----|------|---------|-------------|
| replicaCount | int | `1` |  |
| image.repository | string | `"invisibl/identity-manager"` |  |
| image.pullPolicy | string | `"IfNotPresent"` |  |
| image.tag | string | `""` |  |
| imagePullSecrets | list | `[]` |  |
| nameOverride | string | `""` |  |
| fullnameOverride | string | `""` |  |
| serviceAccount.create | bool | `true` |  |
| serviceAccount.annotations | object | `{}` |  |
| serviceAccount.name | string | `""` |  |
| rbac.enabled | bool | `true` |  |
| rbac.namespaced | bool | `false` |  |
| podAnnotations | object | `{}` |  |
| podSecurityContext | object | `{}` |  |
| securityContext | object | `{}` |  |
| service.type | string | `"ClusterIP"` |  |
| service.port | int | `80` |  |
| ingress.enabled | bool | `false` |  |
| ingress.annotations | object | `{}` |  |
| ingress.hosts[0].host | string | `"chart-example.local"` |  |
| ingress.hosts[0].paths[0].path | string | `"/"` |  |
| ingress.hosts[0].paths[0].backend.serviceName | string | `"chart-example.local"` |  |
| ingress.hosts[0].paths[0].backend.servicePort | int | `80` |  |
| ingress.tls | list | `[]` |  |
| resources | object | `{}` |  |
| autoscaling.enabled | bool | `false` |  |
| autoscaling.minReplicas | int | `1` |  |
| autoscaling.maxReplicas | int | `100` |  |
| autoscaling.targetCPUUtilizationPercentage | int | `80` |  |
| nodeSelector | object | `{}` |  |
| tolerations | list | `[]` |  |
| affinity | object | `{}` |  |
| provider.azure.enabled | bool | `false` |  |
| provider.azure.type | int | `0` |  |
| provider.azure.resourceID | string | `""` |  |
| provider.azure.clientID | string | `""` |  |
| provider.azure.selector | string | `""` |  |
| provider.aws.enabled | bool | `false` |  |
| provider.aws.arn | string | `""` |  |
