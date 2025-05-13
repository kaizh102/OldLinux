# Excercises for 《Linux 内核完全注释》
## chapter 4, Section 4.9: 一个简单的多任务内核实例 
### Host Environment

OS:

                        Ubuntu 22.04.5 LTS x86_64
                        Kernel: 6.8.0-57-generic
                        Shell: zsh 5.8.1


Simulation Software:

                        Bochs x86 Emulator 2.7
              Built from SVN snapshot on August  1, 2021
                Timestamp: Sun Aug  1 10:07:00 CEST 2021

Bochs BIOS Image:

  `linux-0.00-050613/linux-0.00-rh9/BIOS-bochs-latest`

Bochs VGA Image:

  `linux-0.00-050613/linux-0.00-rh9/VGABIOS-lgpl-latest`

Bochs config file:

  `linux-0.00-050613/linux-0.00-rh9/bochsrc-0.00.bxrc`

Command for watching output of the custom OS kernel:

  `cat /dev/pts/X`
