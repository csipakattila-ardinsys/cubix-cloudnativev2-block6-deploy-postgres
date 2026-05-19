# Cubix Cloud-Native Application Development Training: cloud-native requirements (PostgreSQL deployment)
Fork this repository for the practice session.

## How to start the Chart

Replace password setting.

```shell
helm upgrade postgresql bitnami/postgresql --version 14.2.3 --namespace cubix --install --values values.yaml --set auth.password=password --set image.repository=bitnamilegacy/postgresql --set volumePermissions.image.repository=bitnamilegacy/os-shell --set metrics.image.repository=bitnamilegacy/postgres-exporter --set global.security.allowInsecureImages=true
```
