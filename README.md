# OpenStack-on-KVM
This is a guide for setting up a OpenStack cloud using Ubuntu virtual machines running on a KVM host. The setup covers different sections from spinning up Controller Node, Compute Node, Networking, Object Storage, Block Storage, and ensuring seemless communication within different components.

## What is OpenStack?
OpenStack is an open-source cloud computing platform for public and private clouds, that controls large pools of compute, network and storage resources, and allows on-demand provisioning of virtual resources through a dashboard (Horizon), command-line tools, or RESTsul APIs.

## Nodes in OpenStack

1. **Controller Node**: 
   - Manages the OpenStack services.
   - Runs the Identity service (Keystone), Image service (Glance), management portions of Compute (Nova), Networking (Neutron), and other shared services.
   - Provides the web-based interface (Horizon).

2. **Compute Node**: 
   - Hosts the virtual machine instances.
   - Runs the hypervisor component of Compute (Nova).

3. **Networking Node**:
   - Handles networking services such as routing, NAT, DHCP, and VPN as part of the Networking service (Neutron).

4. **Object Storage Node**: 
   - Stores and retrieves unstructured data objects via a RESTful, HTTP-based API.
   - Uses the Object Storage service (Swift).

5. **Block Storage Node**: 
   - Provides persistent block storage to running instances.
   - Manages the creation, attaching, and detaching of block devices via the Block Storage service (Cinder).

## Prerequisites
- Basic knowledge of Linux system administration.
- Knowledge of setting up and operating KVM (Kernel-based Virtual Machine).
- A host machine with atleast 16GB RAM and 500GB storage.
- Ubuntu 22.04.4 LTS installed on all nodes.

### Setting Up KVM on Ubuntu 20.04 Desktop


