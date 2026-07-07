# KernelSU Integration

> '''
>
> * #### The official KSU has not supported `non-gki` devices for a long time.
>
> * #### So we chose the more reliable KSU fork.
>
> '''

### Backslashxx's KernelSU
---------------------------------

> '''
> 
> * [Repository](https://github.com/backslashxx/KernelSU)
> * [Releases](https://github.com/backslashxx/KernelSU/releases)
> 
> '''

### How To Setup
---------------------------------

```shell
# 1. into workdir
cd android_kernel_xiaomi_sdm710

# 2. setup with backslashxx's KernelSU
curl -LSs https://raw.githubusercontent.com/backslashxx/KernelSU/master/kernel/setup.sh  | bash -s master
```

### Quick Build (Github Actions)
---------------------------------

> '''
> 
> 1. fork this repository
> 
> 2. enable github actions
>
> 3. create a repository's secret of actions (optional)
>
>    name: `SIGNING_KEY`
>
>    content: like `certs/signing_key.pem`
>
>             -----BEGIN PRIVATE KEY-----
>             MIIJQw...more content...0zxuI=
>             -----END PRIVATE KEY-----
>             -----BEGIN CERTIFICATE-----
>             MIIFKD...more content...R8gw==
>             -----END CERTIFICATE-----
> 
> 4. manual run workflow (build kernel)
>
> '''

### Related
---------------------------------

> '''
>
> * [scope-minimized manual hooks](https://github.com/backslashxx/KernelSU/issues/5)
> 
> '''
