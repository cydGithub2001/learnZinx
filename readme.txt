1.远程tollchain需要识别一阵子。可以手动输入；/usr/bin/make;/usr/bin/cc;/usr/bin/c++
2.然后设置deployment,及其mapping；
3.iostream等找不到,可以tools->Resync with RemoteHost
4.设置自动upload:tools -> deployment -> automatic upload
5.引入动态库看下cmakelists.txt
6.服务器和本地cmake/c++版本不一致, 需要变更默认的cmakelists.txt
7.g++ main.cpp -o main -I/usr/include/ -L/usr/bin/ -lzinx 等同于 g++ main.cpp -o main -lzinx
