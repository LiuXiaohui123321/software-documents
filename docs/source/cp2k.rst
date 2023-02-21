cp2k
===============

cp2k软件

CP2K 官网：https://www.cp2k.org/

CP2K 性能分析：https://www.cp2k.org/dev:profiling

CP2K GPU加速相关文章：https://pubs.acs.org/doi/pdf/10.1021/acs.jcim.1c01538

CP2K 介绍（清华-南开，刘锦程）：

- https://mse.nankai.edu.cn/ljc/

量子化学和固体物理计算软件清单（List of quantum chemistry and solid-state physics software
）：

- https://handwiki.org/wiki/List_of_quantum_chemistry_and_solid-state_physics_software

知乎电子结构理论：

- https://www.zhihu.com/column/c_1414556816600256512

赝势方法：

- https://wenku.baidu.com/view/930092b0ef3a87c24028915f804d2b160b4e8612.html?_wkts_=1676967994801
- The Pseudopotential Approximation in Electronic Structure Theory: https://chemistry-europe.onlinelibrary.wiley.com/doi/full/10.1002/cphc.201100387

CP2K 使用方面相关问题
-------------------

- 安装问题
  
  - 官方安装教程：https://github.com/cp2k/cp2k/blob/master/INSTALL.md
  - 知乎CP2K-9.1安装教程（附带软件介绍和测试）：https://zhuanlan.zhihu.com/p/464279124
  - CP2K-9.1, Ubuntu 20.04, GNU: http://bbs.keinsci.com/thread-28171-1-1.html
  - cp2k 9.1, DBCSR相关报错("No DBCSR submodule available")，可以参考这里：http://bbs.keinsci.com/forum.php?mod=viewthread&tid=19009&page=2#pid131928，或者这里：https://github.com/cp2k/cp2k/issues/52
  - MPI相关报错，可以参考这里：http://bbs.keinsci.com/thread-19009-5-1.html
  - gcc版本相关报错（Error in `/usr/libexec/gcc/x86_64-redhat-linux/4.8.5/f951': double free or corruption (fasttop): 0x00000000022d7ea0），可以参考这里：https://groups.google.com/g/cp2k/c/uBzZ0kl2y_E
  - spglib
  
    - Release: https://spglib.github.io/spglib/releases.html
    - Github: https://github.com/atztogo/spglib
  
- 使用问题

  - Quickstep方法：The keyword ''METHOD'' chooses the method for evaluating the forces on atoms to QUICKSTEP, i.e. Density Functional Theory using the Gaussian and Planewaves (GPW) method. 参考这里：https://www.cp2k.org/howto:static_calculation
  - 计算大体系时相关报错（Index to radix array not found），解决办法参考这里：https://blog.csdn.net/zh314js/article/details/76292026，即在脚本的&GLOBAL中加上"EXTENDED_FFT_LENGTHS T"
