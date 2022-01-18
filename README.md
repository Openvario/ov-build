# ov-build
Build system for Openvario Images

Before a Openvario build can be started, the needed source layers have to be checked out. 
To automate this step [kas](https://kas.readthedocs.io/en/latest/intro.html) tool is used.

## Quickstart

1. Clone repository
```
git clone https://github.com/Openvario/ov-build.git
```

2. Start the build
```
docker run -it --rm -v $(pwd):/workdir ghcr.io/openvario/ovbuild-container:main --workdir=/workdir kas build openvario.yml
```
