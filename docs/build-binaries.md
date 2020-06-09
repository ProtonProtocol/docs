# Build binaries

The build script first installs all dependencies and then builds Proton. 

To run it, first change to the ~/proton/proton folder, then launch the script:

```bash
cd ~/proton/proton
./scripts/eosio_build.sh
```

The build process writes temporary content to the `proton/build` folder. After building, the program binaries can be found at `proton/build/programs`.