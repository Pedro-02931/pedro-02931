# Docker in WSL

Docker inside WSL acts as a **translation layer between Windows and Linux applications**. It doesn't inherently **boost performance** but allows running **Linux-based applications (including GUI) inside Windows** without dual-booting.

## **At the Kernel Level**:

* **Docker starts a lightweight VM** in WSL that runs a **Linux kernel**.
* This VM **translates container syscalls into Windows-compatible operations**.
* It operates like a **networked microserver**, intercepting requests and managing them inside **containerized environments**.

## **At the Hardware Level**:

* The performance hit comes from **Hyper-V**, which introduces some **virtualization overhead**.
* If running GPU-intensive workloads (like AI models), **WSL supports GPU passthrough**, meaning Docker containers can access CUDA cores.

## **At the Shell Level**:

* Running **Linux GUI apps** (like VSCode, GIMP, or Blender) inside WSL via Docker involves:
  * Forwarding **X11** (or using **Wayland** for modern apps).
  * Using **WSLg**, which renders graphics via **RDP (Remote Desktop Protocol)**.
