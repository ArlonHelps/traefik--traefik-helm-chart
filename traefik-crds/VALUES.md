# traefik-crds

![Version: 1.4.0](https://img.shields.io/badge/Version-1.4.0-informational?style=flat-square) ![Type: application](https://img.shields.io/badge/Type-application-informational?style=flat-square)

A Traefik based Kubernetes ingress controller

**Homepage:** <https://traefik.io/>

## Maintainers

| Name | Email | Url |
| ---- | ------ | --- |
| mloiseleur | <michel.loiseleur@traefik.io> |  |
| charlie-haley | <charlie.haley@traefik.io> |  |
| darkweaver87 | <remi.buisson@traefik.io> |  |
| jnoordsij |  |  |

## Source Code

* <https://github.com/traefik/traefik>
* <https://github.com/traefik/traefik-helm-chart>

## Requirements

Kubernetes: `>=1.22.0-0`

## Values

| Key | Type | Default | Description |
|-----|------|---------|-------------|
| deleteOnUninstall | bool | `false` | Set it to true if you want to uninstall CRDs when uninstalling this chart. By default, CRDs will be kept so your custom resources will not be deleted accidentally. |
| gatewayAPI | bool | `false` | Set it to true to install GatewayAPI CRDs. Needed if you set providers.kubernetesGateway.enabled to true in main chart |
| hub | bool | `false` | Set it to true to install Traefik Hub CRDs. Needed if you set hub.enabled to true in main chart |
| traefik | bool | `true` | Install Traefik CRDs by default |

----------------------------------------------
Autogenerated from chart metadata using [helm-docs v1.14.2](https://github.com/norwoodj/helm-docs/releases/v1.14.2)
