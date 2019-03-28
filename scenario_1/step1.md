Multilib in WRLinux 10.18

## Multilib is enabled by default in WrLinux

Multilib is enabled by default in WRLinux 10.18 for 64-bit bsps, including qemux86-64, qemuarm64, qemumips64 and other real bsps such as intel-x86-64 and intel-socfpga-64.

It includes "multilib.conf" to support multilib but reset variable "MULTILIBS" to disable multilib for all bsps in a common configure file wrlinux/wrlinux-distro/conf/distro/wrlinux-common.inc.

   # Multilib configuration
   MULTILIBS ?= ""
   require conf/multilib.conf

##############
`git clone https://github.com/katacoda/scenario-examples.git katacoda-scenario-examples`{{execute}}

Within the repository, you will see a set of examples of implementing various Katacoda functionality.

The scenario you are currently reading is in the directory `ls -lha katacoda-scenario-examples/create-scenario-101`{{execute}}. The directory name is what defines the URL.

An example of the current step is `katacoda-scenario-examples/create-scenario-101/step1.md`{{open}}

All the steps are collected via a JSON file, for example, `katacoda-scenario-examples/create-scenario-101/index.json`{{open}}.

The JSON file defines the scenario title, the description, steps order, the UI layout and environment. You can find more about the layouts within our scenarios at [katacoda.com/scenario-examples/ui-layouts](https://katacoda.com/scenario-examples/ui-layouts) and environments at [katacoda.com/scenario-examples/environments](https://katacoda.com/scenario-examples/environments).
