# hello-rust
```
 ____________________
< Hello programmers! >
 --------------------
        \
         \
            _~^~^~_
        \) /  o o  \ (/
          '_   -   _'
          / '-----' \
```

# statically link an executable
docker pull rust # this is a aarch64 image!

```
root@228cd5f7a4b2:~/hello-rust/src# rustc -C target-feature=+crt-static  hello.rs
root@228cd5f7a4b2:~/hello-rust/src# ls
hello  hello.rs  main.rs
root@228cd5f7a4b2:~/hello-rust/src# file hello
hello: ELF 64-bit LSB executable, ARM aarch64, version 1 (GNU/Linux), statically linked, BuildID[sha1]
```