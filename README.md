# openwrt-n2n-latest

official latest code will be clone when compiling

# usage

```bash
wget https://downloads.openwrt.org/releases/19.07.4/targets/ipq40xx/generic/openwrt-sdk-19.07.4-ipq40xx-generic_gcc-7.5.0_musl_eabi.Linux-x86_64.tar.xz
tar xvf openwrt-sdk-19.07.4-ipq40xx-generic_gcc-7.5.0_musl_eabi.Linux-x86_64.tar.xz
cd openwrt-sdk-19.07.4-ipq40xx-generic_gcc-7.5.0_musl_eabi.Linux-x86_64/package
git clone https://github.com/hiplon/openwrt-n2n-latest n2n
cd ..
make menuconfig # (selected Network -> VPN -> n2n-edge and n2n-supernode)
make package/n2n/compile V=s

```