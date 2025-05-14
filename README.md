# Excercises for 《Linux 内核完全注释》
## chapter 4, Section 4.9: 一个简单的多任务内核实例 
### Host Environment

OS:
```
                        Ubuntu 22.04.5 LTS x86_64
                        Kernel: 6.8.0-57-generic
                        Shell: zsh 5.8.1
```
assembler:
```$ apt show bin86                                                                
Package: bin86                                                                  
Version: 0.16.17-3.3                                                            
Priority: optional                                                              
Section: universe/devel                                                         
Source: linux86                                                                 
Origin: Ubuntu                                                                  
Maintainer: Ubuntu Developers <ubuntu-devel-discuss@lists.ubuntu.com>           
Original-Maintainer: Juan Cespedes <cespedes@debian.org>                        
Bugs: https://bugs.launchpad.net/ubuntu/+filebug                                
Installed-Size: 249 kB                                                          
Depends: libc6 (>= 2.14)                                                        
Conflicts: linux86                                                              
Download-Size: 81.2 kB                                                          
APT-Manual-Installed: yes                                                       
APT-Sources: https://mirrors.tuna.tsinghua.edu.cn/ubuntu jammy/universe amd64 Pa
ckages                                                                          
Description: 16-bit x86 assembler and loader                                    
 This is the as86 and ld86 distribution written by Bruce Evans.                 
 It's a complete 8086 assembler and loader which can make 32-bit                
 code for the 386+ processors.                                               
```
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
