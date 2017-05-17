# superpixels
SLIC超像素分割的算法介绍和源码分析
源码分析：作者上传的并不是纯粹的matlab代码，而是采用c写的生成的mex文件。
使用前提：我的电脑安装Matlab 2016ra和Vs2015
首先在下载源码的文件夹下面打开matlab，要写实现c和matlab混编，需要先配置，在命令行敲：mex -setup

备注：matlab比较擅长矩阵运算，而运算for的速度较慢，如果将matlab与C或C++进行混合编程，则可以提升程序运行速度。
matlab与C/C++的混合编程是通过mexFunction进行的，即在C或C++的源文件中添加一个mexFunction函数，然后通过MX矩阵库和MEX函数库进行编程
