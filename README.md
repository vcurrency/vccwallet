VccWallet Fullnode is a z-Addr first, Sapling compatible wallet and full node for vcoind that runs on Linux, Windows and macOS.

![Screenshot](resources/screenshot1.png?raw=true)
![Screenshots](resources/screenshot2.png?raw=true)

# Installation
**Note**: Vccwallet Fullnode will download the entire blockchain (about 26GB), and requires some familiarity with the command line. If you don't want to download the blockchain but prefer a Lite wallet, please check out [Vccwallet Lite](https://www.vccwallet.co).

**Note**: Vccwallet Fullnode will download the entire blockchain (about 26GB), and requires some familiarity with the command line. If you don't want to download the blockchain but prefer a Lite wallet, please check out [Vccwallet Lite](https://www.vccwallet.co).

Head over to the releases page and grab the latest installers or binary. https://github.com/VcoinFoundation/vccwallet/releases

### Linux

If you are on Debian/Ubuntu, please download the '.AppImage' package and just run it.

```
./Vccwallet.Fullnode-0.9.10.AppImage
```

If you prefer to install a `.deb` package, that is also available.

```
sudo dpkg -i vccwallet_0.9.10_amd64.deb
sudo apt install -f
```

### Windows

Download and run the `.msi` installer and follow the prompts. Alternately, you can download the release binary, unzip it and double click on `vccwallet.exe` to start.

### macOS

Double-click on the `.dmg` file to open it, and drag `Vccwallet Fullnode` on to the Applications link to install.

## vcoind

VccWallet needs a Vcoin node running vcoind. If you already have a vcoind node running, VccWallet will connect to it.

If you don't have one, VccWallet will start its embedded vcoind node.

Additionally, if this is the first time you're running VccWallet or a vcoind daemon, VccWallet will download the Vcoin params (~777 MB) and configure `vcoin.conf` for you.

## Compiling from source

VccWallet is written in Electron/Javascript and can be build from source. Note that if you are compiling from source, you won't get the embedded vcoind by default. You can either run an external vcoind, or compile vcoind as well.

#### Pre-Requisits

You need to have the following software installed before you can build Vccwallet Fullnode

- Nodejs v12.16.1 or higher - https://nodejs.org
- Yarn - https://yarnpkg.com

```
git clone https://github.com/VcoinFoundation/vccwallet.git
cd vccwallet

yarn install
yarn build
```

To start in development mode, run

```
yarn dev
```

To start in production mode, run

```
yarn start
```

### [Troubleshooting Guide & FAQ](https://github.com/VcoinFoundation/vccwallet/wiki/Troubleshooting-&-FAQ)

Please read the [troubleshooting guide](https://docs.vccwallet.co/troubleshooting/) for common problems and solutions.
For support or other questions, tweet at [@vccwallet](https://twitter.com/vccwallet) or [file an issue](https://github.com/VcoinFoundation/vccwallet/issues).

_PS: VccWallet is NOT an official wallet, and is not affiliated with the Electric Coin Company in any way._
