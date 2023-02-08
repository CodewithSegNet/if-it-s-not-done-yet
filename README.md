# WHAT IS VAGRANT

In a nutshell, Vagrant is a tool for working with virtual environments, and in most circumstances, this means working with virtual machines. Vagrant provides a simple and easy to use command-line client for managing these environments, and an interpreter for the text-based definitions of what each environment looks like, called Vagrantfiles. Vagrant is [open source](https://opensource.com/resources/what-open-source), which means that anyone can download it, modify it, and share it freely.

While many virtual machine hypervisors provide their own command-line interface, and technically the provisioning of virtual machines through these programs can be done directly or through shell scripts, the advantage Vagrant provides by adding an additional layer is simplicity, interoperability across multiple systems, and a more consistent approach which could theoretically be used with any virtual environment running on top of any other system.

By providing a common text-based format to work with virtual machines, your environment can be defined in code, making it easy to back up, modify, share, and manage with revision control. It also means that rather than sharing a whole virtual machine image, which could be many gigabytes, every time a change is made to the configuration, a simple text file weighing at just a few kilobytes can be shared instead.

Why would I use Vagrant?
While at its core, Vagrant provides a rather simple function, it may be useful to a wide range of people working on different kinds of tasks.

For developers, Vagrant makes it easy to create a local environment which mimics the environment upon which your code will eventually be deployed. You can make sure you have the same libraries and dependencies installed, same processes installed, same operating system and version, and many other details without having to sacrifice the way your local machine is set up, and without the lag or cost of creating an external development environment and connecting to it.

Where can I get Vagrant?
These same advantages for developers also make it an interesting option for UX and UI designers, who can see exactly what their work will look like on a different system, or even get to work with their own isolated copy of the system a developer is programing without having to jump through a lot of hoops.

It’s also a great tool if you’re trying to learn a new tool, operating system, or environment without fear of making a mistake that might compromise your current system. Whether you’re studying for a certification exam, testing out a new deployment script, or just trying something new, you can do so with the confidence that you won’t hurt anything on your local machine or in a production environment. As an added bonus, once you get it right you can use the same process and script to deploy to a real life situation or live environment.

There are a few different ways to get Vagrant. Vagrant is available for download as a binary package for Linux, Mac, and Windows from the [official download page](https://www.vagrantup.com/downloads.html).

For many Linux distributions, you can find Vagrant in your default repositories, and install it just as you would any other piece of software. For example, in Fedora, you can simply run.
<br>
<br> 
**$ sudo dnf install vagrant**
<br>
<br> 
However, the makers of Vagrant caution that the versions available in some repositories are not kept up to date, and you may have fewer issues if you use the official installers.

And if you’re particularly interested in how Vagrant works, as an open source project, Vagrant’s source code is available on [GitHub](https://github.com/mitchellh/vagrant) for you to inspect, clone, and even contribute to.

How do I get started with Vagrant?
The best way to get started with Vagrant is to install it and try it out yourself. Aside from that, the official [documentation](https://www.vagrantup.com/docs/) are invaluable, and provide great directions for taking your first steps. It also helps to know some of the basic terminology used by Vagrant.

- ***Box***: A box is a packaged Vagrant environment, typically a virtual machine. 

- ***Provider***: A provider is the location in which the virtual environment runs. It can be local (the default is to use VirtualBox), remote, or even a special case like a [Docker](https://opensource.com/resources/what-docker) container.

- ***Provisioner***: A provisioner is a tool to set up the virtual environment, and can be as simple as a shell script, but alternatively a more advanced tool like Chef, Puppet, or Ansible can be used.



## WHAT IS VIRTUAL MACHINE
- a virtual machine (VM) is the virtualization/emulation of a computer system. 

Virtual machines are based on computer architectures and provide functionality of a physical computer. Their implementations may involve specialized hardware, software, or a combination. Virtual machines differ and are organized by their function, shown here:

- System virtual machines (also termed full virtualization VMs) provide a substitute for a real machine. They provide functionality needed to execute entire operating systems. A hypervisor uses native execution to share and manage hardware, allowing for multiple environments which are isolated from one another, yet exist on the same physical machine. Modern hypervisors use hardware-assisted virtualization, virtualization-specific hardware, primarily from the host CPUs. 

- Process virtual machines are designed to execute computer programs in a platform-independent environment.
