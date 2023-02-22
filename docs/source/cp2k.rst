cp2k
===============

cp2k软件
-------

CP2K 官网：https://www.cp2k.org/

CP2K 性能分析：https://www.cp2k.org/dev:profiling

CP2K GPU加速相关文章：https://pubs.acs.org/doi/pdf/10.1021/acs.jcim.1c01538

CP2K 介绍（清华-南开，刘锦程）：https://mse.nankai.edu.cn/ljc/


CP2K 方法和算法介绍
-------------------

- CP2K Open Source Molecular Dynamics: CP2K/For Users/For Developers
- Basis Sets: https://www.cp2k.org/basis_sets
- 基组和赝势：https://www.cp2k.org/_media/events:2015_cecam_tutorial:ling_basis_pseudo.pdf
- Diagonalisation &Orbital Transformation: https://www.cp2k.org/_media/events:2016_summer_school:20160824_scf.pdf

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

  - CP2K input reference: https://manual.cp2k.org/cp2k-9_1-branch/index.html
  - Input reference of CP2K version 9.1: https://manual.cp2k.org/cp2k-9_1-branch/CP2K_INPUT/FORCE_EVAL/SUBSYS/KIND.html#BASIS_SET
  - Quickstep方法：The keyword ''METHOD'' chooses the method for evaluating the forces on atoms to QUICKSTEP, i.e. Density Functional Theory using the Gaussian and Planewaves (GPW) method. 参考这里：https://www.cp2k.org/howto:static_calculation
  - 计算大体系时相关报错（Index to radix array not found），解决办法参考这里：https://blog.csdn.net/zh314js/article/details/76292026，即在脚本的&GLOBAL中加上"EXTENDED_FFT_LENGTHS T"
  - B站CP2K 相关视频
  
    - Running CP2K calculations (prof. Jürg Hutter): https://www.bilibili.com/video/BV1oZ4y1c78K/?spm_id_from=333.337.search-card.all.click
    - CP2K介绍——Nature, Science文章神器【CP2K课程01】: https://www.bilibili.com/video/BV1vJ41137Cn/?spm_id_from=333.337.search-card.all.click
    - cp2k.inp输入文件初探【CP2K课程02】: https://www.bilibili.com/video/BV1nJ411M76M/?spm_id_from=333.788.recommend_more_video.0
    - CP2K学习笔记（1）（涉及QUICKSTEP测试算例）：https://www.bilibili.com/read/cv12519490
    
  - 知乎CP2K 相关文章
  
    - CP2K学习记录(1)：Si晶胞的静态计算：https://zhuanlan.zhihu.com/p/495399694
    - Second generation CPMD: 
    - QuickStep & OT method: https://zhuanlan.zhihu.com/p/29841461
