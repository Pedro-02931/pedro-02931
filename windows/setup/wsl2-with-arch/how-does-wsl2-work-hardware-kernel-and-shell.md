# How Does WSL2 Work? (Hardware, Kernel & Shell)

WSL2 **is essentially a lightweight virtual machine running a full Linux kernel on top of Windows**. Think of it like **Venom and Eddie**—where **Eddie (a shit of piece) is the host** and **Venom (fucking cosmic entity) is the parasite that actually runs the show**.

Through this layer, it can:

* **Perform syscalls**,
* **Read and write files**,
* **Compile packages**,
* **Manage processes**,
* **Access system resources**—all while Windows remains the primary OS.

Since WSL2 operates within a **virtual hard disk (VHD)**, it automatically handles partitioning. No need to manually fiddle with disk tables.

Here's a **Mermaid diagram** to visualize the architecture:

```mermaid
classDiagram
    direction LR
    class Windows {
        <<System>>
        + Kernel32.dll()
        + ntdll.dll()
        + Sysmon()
        + EventViewer()
    }

    class WSL {
        <<VirtualizationLayer>>
        + init(kernel: string, distro: string)
        + executeSyscall(call: string): string
        + mountDrive(driveLetter: string, path: string): boolean
        + listProcesses(): string[]
        + fetchEventLogs(): string[]
    }

    class Arch {
        <<DistroInstance>>
        + init(username: string, hostname: string, packages: list)
        + installPackage(package: string): boolean
        + executeCommand(command: string): string
        + configureService(service: string, state: string): boolean
        + buildFromAUR(pkgbuild: string): string
    }

    class SyscallLayer {
        <<InteractionLayer>>
        + mapSyscalls(winCall: string): string
        + handleFileAccess(path: string, mode: string): string
        + logSyscallEvents(): string
    }

    class VirtualDisk {
        <<StorageLayer>>
        + allocateSpace(size: string): boolean
        + writeData(offset: int, data: string): boolean
        + readData(offset: int, length: int): string
        + encryptVolume(key: string): boolean
        + decryptVolume(key: string): boolean
    }

    Windows --|> WSL : "Manages virtualization"
    WSL --> SyscallLayer : "Syscall proxying"
    WSL --> VirtualDisk : "Manages VHD"
    Arch --|> WSL : "Runs inside"
    SyscallLayer --> Windows : "Maps syscalls"
    SyscallLayer --> Arch : "Translates to Linux"
    VirtualDisk --> Windows : "Exposes via Hyper-V"

    class Monitoring {
        <<EventTracing>>
        + monitorFileAccess()
        + logEventSource()
        + trackSyscallActivity()
        + reportTelemetry()
    }

    Windows --> Monitoring : "Feeds data"
    Monitoring --> WSL : "Tracks actions"
    Monitoring --> VirtualDisk : "Logs access"

```

