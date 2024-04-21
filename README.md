# github-workflows

Some github workflows and actions that I reuse.

# Workflows

### docker-build-and-push
<details>
<summary>expand</summary>
Builds an image and pushes to docker hub or ghcr.

Variables:
- `REGISTRY`
    - one of 
      - `ghcr`
      - `docker-hub`
- `REPOSITORY`
  - name of repo for image (e.g. `haondt`)
- `IMAGE_NAME`
  - name of image
- `BUILD_CONTEXT`
  - path for build context
- `DOCKERFILE`
  - path to dockerfile
Secrets:
- `DOCKER_USERNAME`
  - (optional) username for docker hub
- `DOCKER_PASSWORD`
  - (optional) password for docker hub
</details>

# Actions

### docker-setup

sets up qemu, buildx and metadata for docker image