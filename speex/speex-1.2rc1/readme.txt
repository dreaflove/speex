//by changweige
一、编译android下的动态链接库
    ./arm_android_sh 
    make
    make install
    说明：需要配置脚本中ndk的路径
二、编译过程中遇到的问题
     1、soname问题，在使用libspeex.so时，android系统提示需要链接libspeex.so.1,这是因为在生成.so时 soname为libspeex.so.1的原因
     解决方案：
	编辑speex-1.2rc2目录下的libtool文件
       找到“soname_spec="\${libname}\${release}\${shared_ext}\$major“ ”，将\$major删除，即可使soname改为libspeex.so