# TizenBrew

Welcome to TizenBrew! TizenBrew is a way to experience modded websites (like [TizenTube](https://github.com/reisxd/TizenTube)) and you can install newer apps without having to deal with Tizen Studio multiple times.

TizenBrew is a modular system, meaning you can install new modded websites and apps without having to mess with Tizen Studio.

## Installation

To install TizenBrew, you need to have a Samsung TV (Tizen) device that has at least Tizen 3.0 (2017 or newer). You can install TizenBrew by following the instructions below:

1. Install Tizen Studio by following the instructions [here](https://developer.samsung.com/smarttv/develop/getting-started/setting-up-sdk/installing-tv-sdk.html).

2. Connect to your TV using this [guide](https://developer.samsung.com/smarttv/develop/getting-started/using-sdk/tv-device.html).

3. Download the latest TizenBrew Widget from the [releases page](https://github.com/reisxd/TizenBrew/releases).

4. Check if the TV is connected by running:
```bash
sdb devices
```

Note that sdb is in `C:\tizen-studio\tools` on Windows and in `~/tizen-studio/tools` on Linux.

5. Install the TizenBrew Widget by running:
```bash
sdb push path/to/TizenBrew.wgt /tmp/TizenBrew.wgt
sdb shell 0 vd_appinstall TizenBrewStandalone /tmp/TizenBrew.wgt 
```

or:
```bash
sdb install path/to/TizenBrew.wgt
```

6. Set the Host PC IP address to `127.0.0.1` by following [this](https://developer.samsung.com/smarttv/develop/getting-started/using-sdk/tv-device.html#Connecting-the-TV-and-SDK)

7. You can now launch the TizenBrew app on your TV.