# chez-libghostty

A Chez Scheme library, `(ghostty)`, binding libghostty-vt, the terminal emulator core of Ghostty.

## Building and testing

Needs threaded Chez Scheme 10.4.1 and Zig 0.16.0; Ghostty is a git submodule, so clone with `--recursive`. The build needs no network.

```sh
make SCHEME=/path/to/chez-10.4.1/scheme build
make SCHEME=/path/to/chez-10.4.1/scheme test
make SCHEME=/path/to/chez-10.4.1/scheme bench
make clean
```

## Upstream

`vendor/ghostty` is Ghostty at `b58ef1d678be2747c830bc1b1e6c0a086afecf9a`, unmodified.

`vendor/zig-packages` holds, unmodified, the Zig packages Ghostty's build fetches for libghostty-vt at that commit:

| File | Source | Zig hash |
|---|---|---|
| `arocc-f97cdfc3779aec4b242299e2fc9a1c828c3547c6.tar.gz` | https://github.com/vancluever/arocc/archive/f97cdfc3779aec4b242299e2fc9a1c828c3547c6.tar.gz | `aro-0.0.0-JSD1Qk6lNgDdcDV4Vh7Sfy-34m2TluIVOdPzMmj_0BjX` |
| `ghostty-themes-release-20261012-151317-d3e95e4.tgz` | https://deps.files.ghostty.org/ghostty-themes-release-20261012-151317-d3e95e4.tgz | `N-V-__8AAI2WBQDrsjfyEiqnmYZ4VfGdJaZhN2mKsaTaIVWq` |
| `highway-66486a10623fa0d72fe91260f96c892e41aceb06.tar.gz` | https://deps.files.ghostty.org/highway-66486a10623fa0d72fe91260f96c892e41aceb06.tar.gz | `N-V-__8AAGmZhABbsPJLfbqrh6JTHsXhY6qCaLAQyx25e0XE` |
| `pixels-12207ff340169c7d40c570b4b6a97db614fe47e0d83b5801a932dcd44917424c8806.tar.gz` | https://deps.files.ghostty.org/pixels-12207ff340169c7d40c570b4b6a97db614fe47e0d83b5801a932dcd44917424c8806.tar.gz | `N-V-__8AADYiAAB_80AWnH1AxXC0tql9thT-R-DYO1gBqTLc` |
| `translate-c-4e879eb8aba615de112eabd1231ea6e01920cead.tar.gz` | https://codeberg.org/vancluever/translate-c/archive/4e879eb8aba615de112eabd1231ea6e01920cead.tar.gz | `translate_c-0.0.0-Q_BUWhVNBwDOEcIqub4VFPJPB6D9dgwzUMHTX5KWr8Xr` |
| `uucode-9d55524551411b493cca41ca06363625d90aff1e.tar.gz` | https://github.com/jacobsandlund/uucode/archive/9d55524551411b493cca41ca06363625d90aff1e.tar.gz | `uucode-0.2.0-ZZjBPuuFVgC8YZ8eld4fOKsZANLIhTFMzULQxhkLi1C7` |
| `wuffs-7411f488fe2e2c205c3d3b3d28638b7356522930.tar.gz` | https://deps.files.ghostty.org/wuffs-7411f488fe2e2c205c3d3b3d28638b7356522930.tar.gz | `N-V-__8AAP5JWgCGP_AD0teWpa4krRvE9VPZzvviGdbmN4jI` |
| `zlib-1220fed0c74e1019b3ee29edae2051788b080cd96e90d56836eea857b0b966742efb.tar.gz` | https://deps.files.ghostty.org/zlib-1220fed0c74e1019b3ee29edae2051788b080cd96e90d56836eea857b0b966742efb.tar.gz | `N-V-__8AAB0eQwD-0MdOEBmz7intriBReIsIDNlukNVoNu6o` |
