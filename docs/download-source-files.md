# Download source files

To download the Proton source code, clone the proton repo and its submodules.

```bash
mkdir -p ~/proton && cd ~/proton
git clone --recursive https://github.com/ProtonProtocol/proton
```

If you previously cloned the repository without the --recursive flag, the submodules must be updated before starting the build process:

```bash
cd ~/proton/proton
git submodule update --init --recursive
```