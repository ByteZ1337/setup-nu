# setup-nu

Installs a (optionally hash pinned) [nushell](https://www.nushell.sh) release

```yaml
- uses: ByteZ1337/setup-nu@v1
  with:
    version: 0.116.1
    sha256: d6d8ace4be491ed8abba4026e73b60c0470b4671d7039307e7d772282ef863da
```

Hash is the `nu-<version>-x86_64-unknown-linux-gnu.tar.gz` line of the release's `SHA256SUMS`:

```sh
gh release download <version> -R nushell/nushell -p SHA256SUMS -O - | grep x86_64-unknown-linux-gnu.tar.gz
```

Linux x86_64 runners only.
