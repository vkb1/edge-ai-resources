# Edge AI Resources for Open Edge Platform 

Here's a list of resources for working with [Open Edge Platform](https://github.com/open-edge-platform), a modular open source stack on GitHub that taps the power, performance, and security of Intel platforms for edge AI. 

## Table of Contents

- [Open Edge Platform](#open-edge-platform)
- [Edge Microvisor Toolkit](#edge-microvisor-toolkit)
- [Edge Manageability Framework](#edge-manageability-framework)
- [Edge AI Libraries](#edge-ai-libraries)
- [Edge AI Suites](#edge-ai-suites)

## About Open Edge Platform

[Open Edge Platform](https://github.com/open-edge-platform) from Intel delivers a modular, composable stack of open-source software optimized to rapidly deploy, secure, and scale AI solutions at distributed edge sites. 

Open Edge Platform comprises [Edge Microvisor Toolkit](https://github.com/open-edge-platform/edge-microvisor-toolkit), [Edge Manageability Framework](https://github.com/open-edge-platform/edge-manageability-framework), [Edge AI Libraries](https://github.com/open-edge-platform/edge-ai-libraries), and [Edge AI Suites](https://github.com/open-edge-platform/edge-ai-suites). 

Vendors, developers, and technology partners can take part in the GitHub community for these solutions in various ways: contributing code, proposing a design, downloading and trying out releases, opening an issue, benchmarking application performance, and -- perhaps most important of all for building community -- participating in discussions. For more information on Open Edge Platform, check out these resources: 

- [Read and respond to blog posts](https://medium.com/open-edge-platform)
- [Watch demo videos on YouTube](https://www.youtube.com/playlist?list=PLg-UKERBljNxIMUUPWHpA8ZJ_YUU5tPP9)

## Edge Microvisor Toolkit

The versions of Edge Microvisor Toolkit demonstrate the capabilities of Intel platforms for edge AI workloads through yet-to-be-upstreamed Linux kernel [patches](https://github.com/intel/linux-kernel-overlay) from Intel that optimize performance and other capabilities for Intel processors. All the versions of Edge Microvisor Toolkit use [Linux kernel 6.12 from Intel](https://github.com/intel/linux-intel-lts). Here's where to download or build the version you want:

- [Download the current ISO of the Developer Node](https://files-rs.edgeorchestration.intel.com/files-edge-orch/microvisor/iso/EdgeMicrovisorToolkit-3.1.iso) and authenticate it with its [SHA256](https://files-rs.edgeorchestration.intel.com/files-edge-orch/microvisor/iso/EdgeMicrovisorToolkit-3.1.iso.sha256sum). A mutable, ready-made version for development, customization, testing, benchmarking, and VM exploration, the developer node uses GRUB as the bootloader, works with DNF or TDNF for RPM package management, and supports K3s, Docker, and other cloud-native technology. Secure boot and full-disk encryption is enabled only for the real-time version; dm-verity is not enabled for either version.

- [Get the latest weekly release of the RAW image for the real-time or non-RT Developer Node](https://github.com/open-edge-platform/edge-microvisor-toolkit/discussions/categories/announcements?discussions_q=is%3Aopen+category%3AAnnouncements). Its latest weekly release is posted in GitHub Discussions under 📣 [announcements](https://github.com/open-edge-platform/edge-microvisor-toolkit/discussions/categories/announcements?discussions_q=is%3Aopen+category%3AAnnouncements). For predictable performance, the real-time developer node uses the Preempt_RT patch for Linux Kernel 6.12. 🚀 You can convert a RAW image to VHD or VHDX by using a tool like `qemu-img convert`.

- [Build the immutable Standalone Node](https://github.com/open-edge-platform/edge-microvisor-toolkit-standalone-node/blob/main/standalone-node/docs/user-guide/get-started-guide.md). The standalone node is an immutable version integrated with Kubernetes and foundational extensions to help partners quickly evaluate edge AI applications on virtual machines and containers powered by Intel platforms. The use of secure boot and full-disk encryption is optional; dm-verity is turned on by default.

- [Build your own custom mutable or immutable version](https://github.com/open-edge-platform/edge-microvisor-toolkit/blob/3.0/docs/developer-guide/get-started/emt-building-howto.md) by selecting a predefined [JSON image configuration file](https://github.com/open-edge-platform/edge-microvisor-toolkit/tree/3.0/toolkit/imageconfigs) and a [package list file](https://github.com/open-edge-platform/edge-microvisor-toolkit/tree/3.0/toolkit/imageconfigs/packagelists) that determine the image's properties and capabilities. In addition, you can create your own image configuration file and package list to build exactly the version that you want -- a powerful approach to customizing a Linux operating system to validate your edge AI workload on Intel processors.

- [Deploy a version with Edge Manageability Framework](https://github.com/open-edge-platform/edge-microvisor-toolkit/blob/3.0/docs/developer-guide/emt-deployment-edge-orchestrator.md). Versions of the toolkit are coupled with Edge Manageability Framework to help deliver early access to next-generation Intel platform features. Edge Manageability Framework automates the rollout of new OS profiles to compatible hardware platforms so that you can quickly deploy the latest Intel optimizations. See the framework's [GitHub repository](https://github.com/open-edge-platform/edge-manageability-framework).

For more information, see [selecting a version of Edge Microvisor Toolkit](https://github.com/open-edge-platform/edge-microvisor-toolkit/discussions/521). 

For help installing and configuring a version of Edge Microvisor Toolkit, see the [the documentation website](https://docs.openedgeplatform.intel.com/2025.1/edge-microvisor-toolkit/index.html) or [check out the demo videos on YouTube](https://www.youtube.com/playlist?list=PLg-UKERBljNxIMUUPWHpA8ZJ_YUU5tPP9). 🎥


---

Here are other ways to participate in or contribute to Edge Microvisor Toolkit:

- [Participate in discussions](https://github.com/open-edge-platform/edge-microvisor-toolkit/discussions)
- [Open an issue](https://github.com/open-edge-platform/edge-microvisor-toolkit/issues)
- [Submit a pull request](https://github.com/open-edge-platform/edge-microvisor-toolkit/pulls)
- [Read the Contribution Guide](https://github.com/open-edge-platform/edge-microvisor-toolkit/blob/3.0/docs/developer-guide/emt-contribution.md)
- [Submit a design proposal](https://github.com/open-edge-platform/edge-microvisor-toolkit/tree/3.0/design-proposals)
- [Report a security vulnerability](https://github.com/open-edge-platform/edge-microvisor-toolkit/blob/3.0/SECURITY.md)
- [Read and respond to blog posts](https://medium.com/open-edge-platform/subpage/5f0ac5579c60)
- [View the documentation website](https://docs.openedgeplatform.intel.com/2025.1/edge-microvisor-toolkit/index.html)
- [Download the latest weekly release](https://github.com/open-edge-platform/edge-microvisor-toolkit/discussions/categories/announcements?discussions_q=is%3Aopen+category%3AAnnouncements)

## Edge Manageability Framework

- [Participate in discussions](https://github.com/open-edge-platform/edge-manageability-framework/discussions)
- [Open an issue](https://github.com/open-edge-platform/edge-manageability-framework/issues)
- [Submit a pull request](https://github.com/open-edge-platform/edge-manageability-framework/pulls)
- [Submit a design proposal](https://github.com/open-edge-platform/edge-manageability-framework/blob/main/design-proposals/README.md)
- [Report a security vulnerability](https://github.com/open-edge-platform/edge-manageability-framework/blob/main/SECURITY.md)
- [Read the latest release notes](https://docs.openedgeplatform.intel.com/edge-manage-docs/dev/release_notes/index.html)
- [Read and respond to blog posts](https://medium.com/open-edge-platform/subpage/696bdf943dcb)
- [View the documentation website](https://docs.openedgeplatform.intel.com/edge-manage-docs/3.1/index.html)
- [See the latest weekly builds](https://github.com/open-edge-platform/edge-manageability-framework/discussions/categories/weekly-builds)

## Edge AI Libraries

- [Participate in discussions](https://github.com/open-edge-platform/edge-ai-libraries/discussions)
- [Open an issue](https://github.com/open-edge-platform/edge-ai-libraries/issues)
- [Submit a pull request](https://github.com/open-edge-platform/edge-ai-libraries/pulls)
- [Read the Contribution Guide](https://github.com/open-edge-platform/edge-ai-libraries/blob/main/CONTRIBUTING.md)
- [Report a security vulnerability](https://github.com/open-edge-platform/edge-ai-libraries/blob/main/SECURITY.md)
- [Read and respond to blog posts](https://medium.com/open-edge-platform/subpage/923dec88c59c)
- [View the documentation website](https://docs.openedgeplatform.intel.com/2025.1/ai-libraries.html)
- [See the latest weekly build report](https://github.com/open-edge-platform/edge-ai-libraries/discussions/categories/weekly-builds)

## Edge AI Suites

- [Participate in discussions](https://github.com/open-edge-platform/edge-ai-suites/discussions)
- [Open an issue](https://github.com/open-edge-platform/edge-ai-suites/issues)
- [Submit a pull request](https://github.com/open-edge-platform/edge-ai-suites/pulls)
- [Read the Contribution Guide](https://github.com/open-edge-platform/edge-ai-suites/blob/main/CONTRIBUTING.md)
- [Report a security vulnerability](https://github.com/open-edge-platform/edge-ai-suites/blob/main/SECURITY.md)
- [Read and respond to blog posts](https://medium.com/open-edge-platform/subpage/2975ecdb1c86)
- [View the documentation website](https://docs.openedgeplatform.intel.com/2025.1/index.html)
- [See the latest weekly build report](https://github.com/open-edge-platform/edge-ai-suites/discussions/categories/weekly-builds)



