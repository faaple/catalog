# NATS 2.10

To build and run this image, [install Unikraft's companion command-line toolchain `kraft`](https://unikraft.org/docs/cli) and then you can run:

```console
kraft build --no-cache --no-update --log-type basic --log-level debug --plat qemu --arch x86_64 .
kraft run --log-type basic --log-level debug -M 256M -p 4222:4222 .
```

Connect to the server using `netcat`:

```console
$ nc -zv localhost 4222
Connection to localhost 4222 port [tcp/*] succeeded! 
```