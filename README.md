# OpenStack-on-KVM
This is a guide for setting up a OpenStack cloud using Ubuntu virtual machines running on a KVM host. The setup covers different sections from spinning up Controller Node, Compute Node, Networking, Object Storage, Block Storage, and ensuring seemless communication within different components.


## What is OpenStack?
OpenStack is an open-source cloud computing platform for public and private clouds, that controls large pools of compute, network and storage resources, and allows on-demand provisioning of virtual resources through a dashboard (Horizon), command-line tools, or RESTsul APIs.

## Nodes in OpenStack

1. **Controller Node**
2. **Compute Node**
3. **Networking Node**
4. **Object Storage Node**: 
5. **Block Storage Node**:
   
Detail information on nodes is found [HERE](../../wiki/)

## Prerequisites
- Basic knowledge of Linux system administration.
- Knowledge of setting up and operating KVM (Kernel-based Virtual Machine).
- A host machine with atleast 16GB RAM and 500GB storage.
- Ubuntu 22.04.4 LTS installed on all nodes.

### Setting Up KVM on Ubuntu 20.04 Desktop
KVM, a virtualization module in the Linux kernel that leverages on modern hardware virtualization extensions such as Intel VT-x and AMD-V. 

To check if processor’s virtualization extensions are enable, execute;

   ```bash
   egrep -c '(vmx|svm)' /proc/cpuinfo
   ```
Please see the detailed process from this [Wiki Page](../../wiki/Setting-Up-KVM-on-Ubuntu-20.04-Desktop)





