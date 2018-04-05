# diaspora helm

Helm chart to deploy a diaspora pod. Based on the [this diaspora docker container](https://gitlab.koehn.com/docker/diaspora).

```
$ helm install diaspora --set postgresql.postgresPassword $(< /dev/urandom tr -dc _A-Z-a-z-0-9 | head -c32) --set redis.redisPassword $(< /dev/urandom tr -dc _A-Z-a-z-0-9 | head -c32)
```
