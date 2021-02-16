# Script-Runner
It will run script from any public url.

### Environment Variables:
- `SCRIPT_URL`: Is used to specify script url.

### How to use?
- Create `docker-compose.yaml`
```yaml
version: "3"
services:
  script:
    container_name: script-runner
    image: quay.io/onet/script-runner:1.0.0
    environment:
      - SCRIPT_URL=script-location.sh
```
- Run compose file `docker-compose up`


