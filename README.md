rockchip-vaapi-driver
=================

Rockchip VA-API Driver

How to Install
===============
1.Install Rockchip Mpp
```bash
git clone https://github.com/rockchip-linux/mpp.git -b develop
mkdir -p mpp/build && cd mpp/build
cmake .. -D{Your Mpp Flags}
make -j$(nproc --all)
sudo make install
```
2.Build libva
```bash
git clone https://github.com/qqdasb/libva-rkmpp.git
mkdir -p libva-rkmpp/build && cd libva-rkmpp/build
./autogen.sh --{Your libva flags}
make -j$(nproc --all)
sudo make install
```
