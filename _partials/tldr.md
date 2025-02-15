## TLDR

Add TLDR - a modern addition to MAN pages, which will help you find nice documentation and examples on most Linux commands:

```bash
echo "alias tldr='docker run --rm -it -v ~/.tldr/:/root/.tldr/ nutellinoit/tldr'" >> ~/.aliases
source ~/.aliases
```

You can try `tldr` with:

```bash
tldr gh
```

ℹ️ It's normal that it takes ~1 minute the first time, as the cache needs to be built. Subsequent calls will be fast.

Finally you should get:

<img alt="tldr" src="images/tldr.png" width=500>

## gRPCurl

gRPCurl is `curl` for [gRPC servers](https://grpc.io/docs/what-is-grpc/introduction/).

- Install `grpcurl`
    ```bash
    curl -s https://grpc.io/get_grpcurl | bash
    ```
- Add `grpcurl` to your `PATH`
    ```bash
    echo '# Add grpcurl to PATH' >> ~/.zshrc
    echo 'PATH=$PATH:$HOME/.grpcurl/bin/' >> ~/.zshrc
    ```
