# identity-manager-demo

![version: 1.0.0](https://img.shields.io/badge/version-1.0.0-informational?style=flat-square) ![type: application](https://img.shields.io/badge/type-application-informational?style=flat-square) ![app version: 1.0.0](https://img.shields.io/badge/app%20version-1.0.0-informational?style=flat-square)

A Helm chart for Kubernetes

## TL;DR;

```bash
helm repo add invisibl https://charts.invisibl.io
helm install --generate-name --wait invisibl/identity-manager-demo
```

## Values

| Key | Type | Default | Description |
|-----|------|---------|-------------|
| replicaCount | int | `1` |  |
| image.repository | string | `"invisibl/identity-manager-demo"` |  |
| image.pullPolicy | string | `"IfNotPresent"` |  |
| image.tag | string | `""` |  |
| workloadIdentity.aws.oidcProvider | string | `""` |  |
| workloadIdentity.aws.accountId | string | `""` |  |
| nameOverride | string | `""` |  |
| fullnameOverride | string | `""` |  |
| serviceAccount.create | bool | `true` |  |
| serviceAccount.annotations | object | `{}` |  |
| serviceAccount.name | string | `""` |  |