# GetPageSpeed Docker Images

This repository contains Docker images for various versions of CentOS/RHEL with GetPageSpeed LTS support. 
These images are configured to provide extended support and updates for CentOS/RHEL systems even after their official end-of-life.

## Available Images

- `getpagespeed/lts:el7`
- `getpagespeed/lts:el8`
- `getpagespeed/lts:el9`

## Usage

### Pull the Image

```bash
docker pull getpagespeed/lts:el7
```

### Run a Container

```bash
docker run -it getpagespeed/lts:el7 /bin/bash
```

## Building Locally

### Build CentOS 7 Image

```bash
docker build -t getpagespeed/lts:el7 -f Dockerfile.el7 .
```

### Build Rocky Linux 8 Image

```bash
docker build -t getpagespeed/lts:el8 -f Dockerfile.el8 .
```

### Build Rocky Linux 9 Image

```bash
docker build -t getpagespeed/lts:el9 -f Dockerfile.el9 .
```

## Contributing

Contributions are welcome! Please open an issue or submit a pull request with your improvements.

## License

This repository is provided under the same terms as the CentOS project.


### Summary

By using the repository name `GetPageSpeed/docker-images`, you clearly communicate the purpose of the repository. 
The structure and documentation ensure that it is easy to navigate, use, and contribute to, making it a robust solution for maintaining Docker images with GetPageSpeed LTS support.

### TODO

Rebuild upon release of `getpagespeed-extras-release` to bring the latest changes in the GetPageSpeed configuration.
