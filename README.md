<div align="center">

<h1 align="center">BPatch</h1>

[![GitHub License](https://img.shields.io/github/license/bmax121/APatch?logo=gnu)](/LICENSE)

</div>

BPatch is a fork of [APatch](https://github.com/bmax121/APatch), an Android kernel and system patching solution.

## Features

- A kernel-based root solution for Android devices.
- APM: Support for modules similar to Magisk.
- KPM: Support for modules that allow injection of code into the kernel, providing kernel inline-hook and syscall-table-hook.
- Relies on [KernelPatch](https://github.com/bmax121/KernelPatch/).
- The UI and module source code are derived and modified from [KernelSU](https://github.com/tiann/KernelSU).

## Supported Versions

- Architecture: ARM64 only.
- Android kernel versions: 3.18 - 6.12.

## Requirements

Kernel configuration options:
- `CONFIG_KALLSYMS=y` and `CONFIG_KALLSYMS_ALL=y`
- `CONFIG_KALLSYMS=y` and `CONFIG_KALLSYMS_ALL=n` (initial support)

## Security Alert

The **SuperKey** grants higher privileges than standard root access. Weak or compromised keys can result in unauthorized control of the device. Use robust keys and safeguard them from exposure.

## Credits

- [KernelPatch](https://github.com/bmax121/KernelPatch/): The core interface.
- [Magisk](https://github.com/topjohnwu/Magisk): magiskpolicy components.
- [KernelSU](https://github.com/tiann/KernelSU): App UI and Magisk-style module system.

## License

BPatch is licensed under the GNU General Public License v3 (GPL-3).
