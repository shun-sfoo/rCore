# rCore

## env

### archlinux

```bash
pacman -S qemu-arch-extra
```

### rust

```bash
# 安装rustc的nightly版本，并把该版本设置为rustc的缺省版本
rustup install nightly
# 在某项目下设置为nightly
rustup override set nightly
# `rustup override unset`  to remove
# rustup default nightly
```

crates.io 中国的镜像服务器

```bash
# vim ~/.cargo/config
[source.crates-io]
replace-with = 'tuna'

[source.tuna]
registry = "https://mirrors.tuna.tsinghua.edu.cn/git/crates.io-index.git"
```

Rust 相关的软件包

```bash
rustup target add riscv64gc-unknown-none-elf
cargo install cargo-binutils
rustup component add llvm-tools-preview
rustup component add rust-src
```
