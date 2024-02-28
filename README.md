# ROS 2 Nano Bot - Project

## Coding Guidelines

Guidelines are documented [here](./CONTRIBUTING.md).

## Native Setup

You need to install a few prerequisites so that you can run the real setup:
```bash
./scripts/install_prerequisites.sh
```
You can then run the ansible playbook through the command:
```bash
ansible-playbook setup/setup.yaml --ask-become
```

> **_NOTE:_**  If this is your first install of ROS2, you will need to source the framework manually after install (or open a new terminal, or reboot your machine) before being able to use ros commands. Use `source /opt/ros/humble/setup.bash` to load the ROS2 framework to your environment.

## Docker Setup

You can develop directly in the project's pre-built docker environment.
Build it locally with the provided script:
```bash
./scripts/build_dev_docker_image.sh full
```
Or pull it from the project's registry with the command:
```bash
docker pull TBD
```
## Compilation/Run instructions

From your development environment run the command:
```bash
colcon build
```
