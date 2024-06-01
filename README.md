# rig-rocky8

A Docker image with R release and devel installed via [rig](https://github.com/r-lib/rig/), built daily at midnight UTC.

## Usage

```sh
docker run --rm -ti --platform linux/amd64 -v $(pwd):/root/workspace ghcr.io/krlmlr/rig-rocky8:main
```

This mounts the current working directory at `~/workspace`, which is also initial starting directory of the image.

## In a Dockerfile

```dockerfile
FROM ghcr.io/krlmlr/rig-rocky8:main
```
