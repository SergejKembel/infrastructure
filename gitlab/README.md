# Registering a runner

```bash
docker exec -t -i <name/id of runner container s> gitlab-runner register \
  --non-interactive \
  --executor="docker" \
  --docker-image="docker:latest" \
  --url="https://<Git URL>" \
  --description="Runner 01" \
  --tag-list="docker" \
  --run-untagged="false" \
  --locked="false" \
  --registration-token="<Registration Token>"
```
