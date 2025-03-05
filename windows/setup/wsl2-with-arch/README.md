# WSL2 With Arch

Given that I'm **too lazy for college but not for work**, I decided to use [**ArchWSL**](https://wsldl-pg.github.io/ArchW-docs/How-to-Setup/).

~~Man, screw configuring time zone keys every time you switch OSes, not to mention the pain of partition allocation when you're stuck with a shitty computer. But hey, when I want something, I get it done—even from scratch. That’s what you call natural talent.~~

```powershell
wsl --install
```

Once WSL2 is installed, extract the **ArchWSL** files (which include an executable that sets up the **Arch kernel, boot, and a virtual disk**) and run the command list from the [ArchWSL documentation](https://wsldl-pg.github.io/ArchW-docs/How-to-Setup/).

Boom, **Arch is up and running inside Windows**—the equivalent of a "Hello World!" moment.

***

This setup allows for **maximum control over package management, performance, and system optimization**, combining:

* **Arch’s bleeding-edge flexibility**,
* **Windows’ compatibility**,
* **WSL’s lightweight virtualization**,
* **Docker’s modular environment management**.

With **syscall mapping**, **parallel downloads**, **disk optimizations**, and **virtualization layers**, the system achieves **near-native performance inside Windows** while maintaining the **Arch workflow**.

~~Basically, it's a cybernetic parasite feeding off Windows while running Arch in a controlled environment~~.
