# Swift Toolchain Manager

Switch Swift toolchain easily.

## Installation

### zplug

```zsh
zplug "giginet/swift-toolchain-manager", lazy:true, use:'stm', as:command
```

## Usage

It works well with peco.

```console
$ export TOOLCHAINS=`stm list | peco | xargs stm show`
$ swift --version
```

### list

List all available Swift toolchains

```console
$ stm list
swift-4.0-RELEASE.xctoolchain
swift-4.0.3-RELEASE.xctoolchain
swift-4.1-DEVELOPMENT-SNAPSHOT-2018-03-01-a.xctoolchain
swift-4.2-CONVERGENCE.xctoolchain
swift-4.2-DEVELOPMENT-SNAPSHOT-2018-05-29-a.xctoolchain
swift-4.2-DEVELOPMENT-SNAPSHOT-2018-07-01-a.xctoolchain
swift-4.2-DEVELOPMENT-SNAPSHOT-2018-09-08-a.xctoolchain
swift-5.0-DEVELOPMENT-SNAPSHOT-2019-03-10-a.xctoolchain
swift-DEVELOPMENT-SNAPSHOT-2018-03-02-a.xctoolchain
swift-DEVELOPMENT-SNAPSHOT-2018-09-08-a.xctoolchain
swift-DEVELOPMENT-SNAPSHOT-2018-10-24-a.xctoolchain
swift-latest.xctoolchain
```

### show

Show identifier of specific Swift toolchain

```console
$ stm show swift-latest
org.swift.5020190310a
```
