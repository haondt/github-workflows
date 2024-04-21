# github-workflows

Some github workflows and actions that I reuse.

See [examples](./examples/) folder for, well, examples.

# Workflows

### docker-hub-build-and-push

<details>
<summary>expand</summary>
Builds an image and pushes to docker hub

Variables:
- `repository`
  - name of repo for image (e.g. `haondt`)
- `image`
  - name of image
- `context`
  - path for build context
- `file`
  - path to dockerfile
secrets:
- `DOCKER_USERNAME`
  - username for docker hub
- `DOCKER_PASSWORD`
  - password for docker hub
</details>

### ghcr-build-and-push

<details>
<summary>expand</summary>
Builds an image and pushes to ghcr

Variables:
- `repository`
  - name of repo for image (e.g. `haondt`)
- `image`
  - name of image
- `context`
  - path for build context
- `file`
  - path to dockerfile
</details>