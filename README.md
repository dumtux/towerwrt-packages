# OpenWrt Custom Packages Collection

Add the following line to feeds.conf or feeds.conf.default.

```
src-git-full custom https://github.com/badtux/towerwrt-packages
```

Run

```sh
./scripts/feeds update custom
rm ./package/feeds/packages/swig
rm ./package/feeds/packages/libmraa
rm ./package/feeds/packages/libupm
./scripts/feeds install -a -p custom
make defconfig
```
