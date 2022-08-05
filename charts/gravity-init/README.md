# gravity-init

![version: v1.0.9](https://img.shields.io/badge/version-v1.0.9-informational?style=flat-square) ![type: application](https://img.shields.io/badge/type-application-informational?style=flat-square) ![app version: v1.0.9](https://img.shields.io/badge/app%20version-v1.0.9-informational?style=flat-square)

A Helm chart for gravity-init

## TL;DR;

```bash
helm repo add invisibl https://charts.invisibl.io
helm install --generate-name --wait invisibl/gravity-init
```

## Values

| Key | Type | Default | Description |
|-----|------|---------|-------------|
| tls.enabled | bool | `true` |  |
| tls.genBy | string | `"helm"` |  |
| env | object | `{}` |  |
| replicaCount | int | `1` |  |
| priorityClassName | string | `"system-cluster-critical"` |  |
| image.repository | string | `"invisibl/gravity-init"` |  |
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
| resources.limits.memory | string | `"128Mi"` |  |
| resources.requests.cpu | string | `"50m"` |  |
| resources.requests.memory | string | `"128Mi"` |  |
| nodeSelector | object | `{}` |  |
| tolerations | list | `[]` |  |
| affinity | object | `{}` |  |
| stack.apply | bool | `false` |  |
| stack.tags.gravityManager | string | `"v1.0.9"` |  |
| stack.tags.gravityUI | string | `"v1.0.9"` |  |
| stack.tags.kroda | string | `"v1.0.8"` |  |
