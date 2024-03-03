# plugin_template
## Dependencies
- [CommonLibSSE](https://github.com/Ryan-rsm-McKenzie/CommonLibSSE)
## Build prerequisites
- Visual Studio 2022
  - Desktop development with C++
- [vcpkg](https://github.com/microsoft/vcpkg)
## Build instructions
Open x64 Native Tools Command Prompt for VS 2022.
```
git clone https://github.com/andrelo1/plugin_template
cd plugin_template
cmake -B build -S . -DCMAKE_TOOLCHAIN_FILE=[path to vcpkg]/scripts/buildsystems/vcpkg.cmake -DVCPKG_TARGET_TRIPLET=x64-windows-static-md -DVCPKG_OVERLAY_PORTS=vcpkg/ports
cmake --build build --config Release
```
