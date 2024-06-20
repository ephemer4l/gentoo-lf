# gentoo-lf
ebuild repository for [lf](https://github.com/gokcehan/lf).

To generate the vendor tarball yourself for version rXX:

```bash
wget https://github.com/gokcehan/lf/archive/refs/tags/rXX.tar.gz
tar xvf lf-rXX/
GO111MODULE=on go mod vendor
cd ..
tar --create --auto-compress --file lf-XX-vendor.tar.xz lf-rXX/vendor
```
