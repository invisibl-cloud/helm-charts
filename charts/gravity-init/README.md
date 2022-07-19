# gravity-init

![version: v1.0.0-rc12](https://img.shields.io/badge/version-v1.0.0--rc12-informational?style=flat-square) ![type: application](https://img.shields.io/badge/type-application-informational?style=flat-square) ![app version: v1.0-rc12-2dc74af](https://img.shields.io/badge/app%20version-v1.0--rc12--2dc74af-informational?style=flat-square)

A Helm chart for gravity-init

## TL;DR;

```bash
helm repo add invisibl https://charts.invisibl.io
helm install --generate-name --wait invisibl/gravity-init
```

## Values

| Key | Type | Default | Description |
|-----|------|---------|-------------|
| profile | string | `"management"` |  |
| tls.enabled | bool | `true` |  |
| tls.genBy | string | `"helm"` |  |
| env | object | `{}` |  |
| replicaCount | int | `1` |  |
| priorityClassName | string | `"system-cluster-critical"` |  |
| image.repository | string | `"invisibl/grtyinit"` |  |
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
| resources.limits.memory | string | `"256Mi"` |  |
| resources.requests.cpu | string | `"100m"` |  |
| resources.requests.memory | string | `"256Mi"` |  |
| nodeSelector | object | `{}` |  |
| tolerations | list | `[]` |  |
| affinity | object | `{}` |  |
| stack.apply | bool | `false` |  |
| stack.tags.gravityManager | string | `"v1.0-rc12-d22bc0f"` |  |
| stack.tags.gravityUI | string | `"v1.0-rc12-580b7b6"` |  |
| stack.tags.kroda | string | `"v1.0-rc12-0497c63"` |  |
| stack.tags.identityManager | string | `"1.0.0"` |  |
