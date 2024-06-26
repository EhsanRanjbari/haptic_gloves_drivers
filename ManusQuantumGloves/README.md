# Instruction on how to install and use the Manus Glove Device

# Dependencies
### Manus Glove SDK  
- Download the SDK from https://www.manus-meta.com/resources/downloads/quantum-metagloves
    - Credentials can be found [here](https://github.com/ami-iit/lab-organisation/wiki/Shared-accounts).
- Extract the files into a folder and rename it "ManusGlove-API".

- Add following environment variable:

```bash
set ManusGlove_DIR=C:\ManusGlove-API\SDKClient
set PATH=%PATH%:%ManusGlove_DIR%\ManusSDK
```
### Manus Core
- Download and install the Manus Core from [here](https://www.manus-meta.com/resources/downloads/quantum-metagloves).

### Build
- clone the repo
- cd `ManusQuantumGloves`
- `mkdir && cd build`
- `cmake -G"Visual Studio 17 2022" ..`
- `cmake --build . --target INSTALL --config Release`
