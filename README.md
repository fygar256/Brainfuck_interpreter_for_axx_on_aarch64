# barinfuck interpreter for aarch64

assembly on freeBSD

```
caxx aarch64.axx bf_aarch64.s -o bf_aarch64.o -m 183
clang --target=aarch64-linux-gnu -fuse-ld=lld -nostdlib -static -o bf_aarch64 bf_aarch64.o
```

execution
`./bf_aarch64 mandelbrot.bf`
