# Prerequisites

## Platform

This tutorial is being developed on a Lenovo P72 mobile worstation with 2Tb of NVME and 128Gb of RAM.  The Kubernetes components will be LXC-containerized.  The host platform for the LXD containers initially will be Ubuntu 20.04 and then once that is working ported over to the four Orabuntu-LXC-supported RedHat-family Linuxes (CentOS, Fedora, RedHat and Oracle Linux).

[Estimated cost] This is an LXD-containerized Kubernetes so it can be theoretically run on any infrastructure from at-home to cloud.

## Running Commands in Parallel with tmux

[tmux](https://github.com/tmux/tmux/wiki) can be used to run commands on multiple compute instances at the same time. Labs in this tutorial may require running the same commands across multiple compute instances, in those cases consider using tmux and splitting a window into multiple panes with synchronize-panes enabled to speed up the provisioning process.

> The use of tmux is optional and not required to complete this tutorial.

![tmux screenshot](images/tmux-screenshot.png)

> Enable synchronize-panes by pressing `ctrl+b` followed by `shift+:`. Next type `set synchronize-panes on` at the prompt. To disable synchronization: `set synchronize-panes off`.

Next: [Installing the Client Tools](02-client-tools.md)
