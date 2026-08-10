# Self-hosted runner

## Environment and prerequisites
- Rocky Linux 10.2
- Python 3.12.13
- Pip 26.2.1
- Podman 5.8.2
- jupyter-repo2docker 2026.4.0 (installed with pip)
- repo2podman in the version of this commit: 0ddb88e0bb01c3b9f900a7f5de24c0bfd25f13ed (installed with pip)

## Installation
- install and register the GitHub runner following GitHub's instructions
- install issue2docker in the prototype-demo-v2 version (https://gitlab.git.nrw/rpdm/projects-and-services/caesar/issue2docker/-/tree/prototype-demo-v2?ref_type=heads) in the work folder of the runner by cloning it and installing its dependencies

## Repository variables

- `CONTAINER_TOOL`, set to `podman`
- `DOCKER_COMMAND`, set to `sudo podman`
- `PYTHON_COMMAND`, set to `sudo python3.12`
- `REPO2DOCKER_ARGS`, set to `--engine=podman --user-id=<your user id> --user-name=<your user name>`
