# Software

## bspwm

```sh
sudo apt install libxcb-xinerama0-dev libxcb-keysyms1-dev
git clone https://github.com/baskerville/bspwm.git
cp bspwm
make && sudo make install
```

## sxhkd

```sh
git clone https://github.com/baskerville/sxhkd.git
cd sxhkd/
make && sudo make install
```

## Neovim

```sh
sudo ln -sf /bin/bash /bin/sh
make CMAKE_BUILD_TYPE=RelWithDebInfo
sudo make install
```

## RipGrep

```sh
clone https://github.com/BurntSushi/ripgrep
cd ripgrep
cargo build --release
./target/release/rg --version
```

## youtube-dl / streamlink

```sh
sudo curl -L https://yt-dl.org/downloads/latest/youtube-dl -o /usr/local/bin/youtube-dl
sudo chmod a+rx /usr/local/bin/youtube-dl

pip3 install streamlink
~/.local/bin/streamlink https://www.twitch.tv/<name> best --player vlc --file-caching 1OOO --network-caching 1OOOO
```
