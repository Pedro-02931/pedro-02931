# Mounting a Physical Disk to WSL (if you ckacked windows Pro)

When running:

```powershell
wmic diskdrive list brief
```

You get a list of **device IDs** for physical drives. To mount a disk inside WSL:

```powershell
wsl --mount \\.\{disk}
```

## **Why Does This Improve File Transfers?**

Mounting a **physical disk** inside WSL is more efficient than using Windows' **File Explorer**, because:

1. **Lower Overhead**: File Explorer treats it like a **network drive**, meaning every operation involves **network stack overhead**.
2. **Direct Syscalls**: WSL uses **syscalls directly to the Linux kernel**, bypassing unnecessary Windows file handling.
3. **Optimized I/O**: Instead of dealing with SMB or NTFS translation layers, WSL can work with **raw partitions**.
