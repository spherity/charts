# indy-ledger-browser

![Version: 0.1.1](https://img.shields.io/badge/Version-0.1.1-informational?style=flat-square) ![Type: application](https://img.shields.io/badge/Type-application-informational?style=flat-square) ![AppVersion: sha-37fa4367](https://img.shields.io/badge/AppVersion-sha--37fa4367-informational?style=flat-square)

A Helm chart for Kubernetes

## Values

| Key | Type | Default | Description |
|-----|------|---------|-------------|
| affinity | object | `{}` |  |
| autoscaling.enabled | bool | `false` |  |
| autoscaling.maxReplicas | int | `100` |  |
| autoscaling.minReplicas | int | `1` |  |
| autoscaling.targetCPUUtilizationPercentage | int | `80` |  |
| config.genesis_url | string | `"https://raw.githubusercontent.com/IDunion/IDunion_TestNet_Genesis/master/pool_transactions_genesis"` |  |
| config.indy_wallet_seed | string | `""` |  |
| config.info_site_text | string | `"Verifiable Organizations Network"` |  |
| config.info_site_url | string | `"https://idunion.org/"` |  |
| config.ip | string | `"0.0.0.0"` |  |
| config.ledger_cache_path | string | `"/home/indy/.indy_client/ledger-cache/ledger-cache-db"` |  |
| config.ledger_instance_name | string | `"Idunion Test Net"` |  |
| config.register_new_dids | bool | `false` |  |
| fullnameOverride | string | `""` |  |
| image.pullPolicy | string | `"IfNotPresent"` |  |
| image.repository | string | `"ghcr.io/bcgov/von-network-base"` |  |
| image.tag | string | `""` |  |
| imagePullSecrets | list | `[]` |  |
| ingress.annotations | object | `{}` |  |
| ingress.className | string | `""` |  |
| ingress.enabled | bool | `true` |  |
| ingress.hosts[0].host | string | `"browser.idunion.spherity.io"` |  |
| ingress.hosts[0].paths[0].path | string | `"/"` |  |
| ingress.hosts[0].paths[0].pathType | string | `"ImplementationSpecific"` |  |
| ingress.tls | list | `[]` |  |
| initChownData.enabled | bool | `true` |  |
| initChownData.image.pullPolicy | string | `"IfNotPresent"` |  |
| initChownData.image.repository | string | `"busybox"` |  |
| initChownData.image.sha | string | `""` |  |
| initChownData.image.tag | string | `"1.31.1"` |  |
| nameOverride | string | `""` |  |
| nodeSelector | object | `{}` |  |
| persistence.accessModes[0] | string | `"ReadWriteOnce"` |  |
| persistence.enabled | bool | `true` |  |
| persistence.finalizers[0] | string | `"kubernetes.io/pvc-protection"` |  |
| persistence.inMemory.enabled | bool | `false` |  |
| persistence.size | string | `"1Gi"` |  |
| persistence.type | string | `"pvc"` |  |
| podAnnotations | object | `{}` |  |
| podSecurityContext.fsGroup | int | `1001` |  |
| podSecurityContext.runAsGroup | int | `1001` |  |
| podSecurityContext.runAsUser | int | `1001` |  |
| replicaCount | int | `1` |  |
| resources | object | `{}` |  |
| securityContext.runAsGroup | int | `1001` |  |
| securityContext.runAsUser | int | `1001` |  |
| service.port | int | `8080` |  |
| service.type | string | `"ClusterIP"` |  |
| serviceAccount.annotations | object | `{}` |  |
| serviceAccount.create | bool | `true` |  |
| serviceAccount.name | string | `""` |  |
| tolerations | list | `[]` |  |

----------------------------------------------
Autogenerated from chart metadata using [helm-docs v1.5.0](https://github.com/norwoodj/helm-docs/releases/v1.5.0)
