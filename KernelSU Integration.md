# KernelSU Integration

> '''
>
> #### The official KSU has not supported `non-gki` devices for a long time.
>
> #### So we chose the more reliable KSU fork.
>
> '''

### backslashxx's KernelSU
---------------------------------

* [Repository](https://github.com/backslashxx/KernelSU)
* [Releases](https://github.com/backslashxx/KernelSU/releases)

### how to setup
---------------------------------

```shell
# 1. into workdir
cd android_kernel_xiaomi_sdm710

# 2. setup with backslashxx's KernelSU
curl -LSs https://raw.githubusercontent.com/backslashxx/KernelSU/master/kernel/setup.sh  | bash -s master

# 3. enable 'CONFIG_KSU'
sed -i 's/CONFIG_KSU=n/CONFIG_KSU=y/g' ./arch/arm64/configs/grus_defconfig
```

### help
---------------------------------
* [scope-minimized manual hooks](https://github.com/backslashxx/KernelSU/issues/5)
