//by changweige
һ������android�µĶ�̬���ӿ�
    ./arm_android_sh 
    make
    make install
    ˵������Ҫ���ýű���ndk��·��
�����������������������
     1��soname���⣬��ʹ��libspeex.soʱ��androidϵͳ��ʾ��Ҫ����libspeex.so.1,������Ϊ������.soʱ sonameΪlibspeex.so.1��ԭ��
     ���������
	�༭speex-1.2rc2Ŀ¼�µ�libtool�ļ�
       �ҵ���soname_spec="\${libname}\${release}\${shared_ext}\$major�� ������\$majorɾ��������ʹsoname��Ϊlibspeex.so