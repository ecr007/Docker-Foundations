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