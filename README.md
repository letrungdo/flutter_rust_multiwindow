### Pre

Install rustc 1.75 or newer

```bash
curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh
```

```bash
git clone https://github.com/microsoft/vcpkg
./vcpkg/bootstrap-vcpkg.sh

export VCPKG_ROOT=$HOME/vcpkg
vcpkg/vcpkg install libvpx libyuv opus aom
```

### Run build

```bash
VCPKG_ROOT=$HOME/vcpkg cargo run
```

Download this file:

- macOS: https://raw.githubusercontent.com/c-smile/sciter-sdk/master/bin.osx/libsciter.dylib
- Window: https://raw.githubusercontent.com/c-smile/sciter-sdk/master/bin.win/x64/sciter.dll

And move this file to target/debug


```bash
cd flutter
sh run.sh
```
