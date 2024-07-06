# GetPageSpeed Docker Images

This repository contains Docker images for various versions of CentOS/RHEL with GetPageSpeed LTS support. These images are configured to provide extended support and updates for CentOS/RHEL systems even after their official end-of-life.

## Available Images

- `getpagespeed/rhel:centos7-lts`
- `getpagespeed/rhel:el7-lts`
- `getpagespeed/rhel:centos8-lts`
- `getpagespeed/rhel:el8-lts`
- `getpagespeed/rhel:centos9-lts`
- `getpagespeed/rhel:el9-lts`

## Usage

### Pull the Image

```bash
docker pull getpagespeed/rhel:centos7-lts
```

Run a Container

docker run -it getpagespeed/rhel:centos7-lts /bin/bash

For the GitHub repository name, you want it to be clear, descriptive, and scalable for future versions. Considering this, a suitable repository name could be:

**`getpagespeed-docker-images`**

### Naming Convention
This name indicates that the repository contains Docker images maintained by GetPageSpeed, and it's flexible enough to accommodate images for various versions of CentOS/RHEL and potentially other distributions in the future.

### Repository Structure
Here’s a suggested structure for your repository to organize Dockerfiles and related configurations:

```
getpagespeed-docker-images/
├── .github/
│   └── workflows/
│       └── docker-build.yml
├── Dockerfile.centos7
├── Dockerfile.centos8
├── Dockerfile.centos9
├── README.md
└── other-files/
```

### README.md
Make sure to include a detailed README file that explains the purpose of the repository, how to use the Docker images, and instructions for contributing or building the images locally.

```markdown
# GetPageSpeed Docker Images

This repository contains Docker images for various versions of CentOS/RHEL with GetPageSpeed LTS support. These images are configured to provide extended support and updates for CentOS/RHEL systems even after their official end-of-life.

## Available Images

- `getpagespeed/rhel:centos7-lts`
- `getpagespeed/rhel:el7-lts`
- `getpagespeed/rhel:centos8-lts`
- `getpagespeed/rhel:el8-lts`
- `getpagespeed/rhel:centos9-lts`
- `getpagespeed/rhel:el9-lts`

## Usage

### Pull the Image

```bash
docker pull getpagespeed/rhel:centos7-lts
```

### Run a Container

```bash
docker run -it getpagespeed/rhel:centos7-lts /bin/bash
```

## Building Locally

### Build CentOS 7 Image

```bash
docker build -t getpagespeed/rhel:centos7-lts -f Dockerfile.centos7 .
```

### Build CentOS 8 Image

```bash
docker build -t getpagespeed/rhel:centos8-lts -f Dockerfile.centos8 .
```

### Build CentOS 9 Image

```bash
docker build -t getpagespeed/rhel:centos9-lts -f Dockerfile.centos9 .
```

## Contributing

Contributions are welcome! Please open an issue or submit a pull request with your improvements.

## License

This repository is provided under the same terms as the CentOS project.
```

### Summary
By using the repository name `getpagespeed-docker-images`, you clearly communicate the purpose of the repository. The structure and documentation ensure that it is easy to navigate, use, and contribute to, making it a robust solution for maintaining Docker images with GetPageSpeed LTS support.
