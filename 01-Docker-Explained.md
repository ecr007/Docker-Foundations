# Docker Explained

Docker uses images and containers to allow apps to runs anywhere consistently.

* The configuration file describe everthing your app need to run. 

## Containers vs. Virtual Machines 

Containers aren't smaller vitual machines. 

**Virtual Machines**

- Use the hypervisor to emulate real hardware.
- Can take a lot of space.
- Require you to install/configure operating system. 
- Can run multiples apps at the same time. 
- Cannot interact with their hosts. 

**Containers**

- Do not emulate any hardware and do not need to "boot up ".
- Do not requiere operating system installation.
- Take up much less space. 
- Can run only one app at a time (by design). 
- Can interact with their host.

## Anatomy of a container

**Groups of containers**
- Linux namespaces
- Linux Control Group

**Namespaces**

- USERNS: User Lists
- MOUNT: Access to filesystems
- NET: Network comunications
- IPC: Interprocess comunications
- TIME: The ability to change time
- CGROUP: Create control groups 
- UTC: Create host/domain names

**What is the main problem that Docker aims to solve?**
Apps working on one michine but not other.

**Tool that allow you to create non-root containers by defaults?**
Podman

**Adavntages of Docker**
Docker Hub makes easily distribute images to anyone, anywhere. 

**Control Groups**
- Controling how much of any resources a process can get. 
- CPU time, memory quota, and memory access are some of things you can limit through me 
- Control groups cannot limit how much disk space or disk IO a process can use.

**Differences between containers and virtual machines**
- Containers are just smaller vistual machine. 

## Testing
After install docker you would write in your terminal:

```docker run hello-world```
