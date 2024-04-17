# wiser

 A very minimal vmm built using Linux Kernel Virtual Machine for Linux.
 
 Following project is under-development expect unfinished components.
 
 ![Image](../main/assets/wiser.png?raw=true) 

## Usage

User needs to download and build kernel images from https://www.kernel.org/.


```bash 
Usage: wiser [OPTION...] --image path-to-kernel-image
wiser - Extremely tiny type-2 hypervisor for linux. Will boot your
unikernel/linux someday.

  -c, --vcpu                 Number of cpu for your vm
  -i, --image=IMAGE          linux kernel bzImage
  -r, --memory               Ram size for your vm
  -v, --verbose              Produce verbose output
  -?, --help                 Give this help list
      --usage                Give a short usage message
  -V, --version              Print program version

Mandatory or optional arguments to long options are also mandatory or optional
for any corresponding short options.

Report bugs to https://github.com/flouthoc/wiser/issues.
```

* #### image
Path to linux kernel bzImage. The bzImage file is in a specific format. It contains concatenated ```bootsect.o + setup.o + misc.o + piggy.o```.

## Roadmap
* ~~Allow users to load initramfs. Closed in https://github.com/flouthoc/wiser/pull/4~~
* Add basic support for Apple hypervisor

## Use cases

Here are 20 novel use cases for the wiser minimal VMM (Virtual Machine Manager) built using Linux Kernel Virtual Machine:

*    Lightweight sandboxing: Use wiser to run untrusted applications or code in an isolated environment.
*    Unikernel development: Leverage wiser to develop and test unikernels, which are specialized, single-address-space machine images constructed using library operating systems.
*    Operating system experimentation: Utilize wiser to experiment with different operating system configurations, kernels, or custom operating systems without affecting the host system.
*    Minimal virtualization for IoT devices: Deploy wiser on resource-constrained IoT devices to enable lightweight virtualization and isolation of different software components.
*    Rapid prototyping of embedded systems: Use wiser to quickly prototype and test embedded system designs by running minimal operating system images.
*    Containerization alternative: Employ wiser as a lightweight alternative to containerization for running isolated workloads with minimal overhead.
*    Secure execution environment: Create a secure execution environment using wiser to run sensitive applications or process confidential data.
*    Kernel development and testing: Utilize wiser to develop, debug, and test Linux kernel modifications or custom kernel modules in an isolated environment.
*    Minimal virtualization for edge computing: Deploy wiser on edge computing devices to enable efficient virtualization and resource management.
*    Virtualized network functions: Use wiser to create lightweight virtualized network functions (VNFs) for software-defined networking (SDN) and network function virtualization (NFV) deployments.
*    Bare-metal cloud provisioning: Leverage wiser to quickly provision and manage bare-metal cloud instances with minimal overhead.
*    Lightweight virtualization for serverless computing: Employ wiser to enable lightweight virtualization for serverless computing platforms, reducing the overhead of spinning up and tearing down instances.
*    Security research and exploit testing: Use wiser to create isolated environments for security research, vulnerability analysis, and exploit testing without compromising the host system.
*    Minimal virtualization for high-performance computing (HPC): Utilize wiser to enable lightweight virtualization in HPC environments, maximizing performance and resource utilization.
*    Educational tool for operating system courses: Incorporate wiser into operating system courses to provide students with hands-on experience in kernel development, virtualization, and system programming.
*    Virtualized honeypots: Deploy wiser to create lightweight virtualized honeypots for attracting and analyzing malicious activities.
*    Fault-tolerant systems: Use wiser to build fault-tolerant systems by running critical components in isolated virtual machines, minimizing the impact of failures.
*    Virtualized build environments: Employ wiser to create lightweight virtualized build environments for software development, ensuring consistent and reproducible builds across different systems.
*    Minimal virtualization for mobile devices: Integrate wiser into mobile devices to enable lightweight virtualization and isolation of different mobile applications or services.
*    Virtualized network simulators: Utilize wiser to create lightweight virtualized network simulators for testing and evaluating network protocols and topologies.

## See also

https://news.ycombinator.com/item?id=10782897

## References
* https://github.com/kvmtool/kvmtool
* https://gitlab.prognosticlab.org/debashis/palacios
* https://wiki.osdev.org/Main_Page
* https://c9x.me/x86/
