# cpp项目结构

project —+—bin
　　　　　|
　　　　　|build—+—debug
　　　　　|　　　 |—release
　　　　　|—doc
　　　　　|—inc—+—module1
　　　　　|　　　 |—module2
　　　　　|—lib—+—module1
　　　　　|            |—module2
　　　　　|—log
　　　　　|—res
　　　　　|—sample—+—sample1
　　　　　|　　　　　 |—sample2
　　　　　|—src
　　　　　|—thirdparty—+—package1
　　　　　|　　　　　      |—package2
　　　　　|—CMakeLists.txt
　　　　　|—README.md
　　　　　|— …

- bin/: 二进制文件，可执行程序
- build/: 项目编译目录，各种编译的临时文件和最终的目标文件皆存于此，分为debug/和release/子目录
- doc/: 保存项目各种文档
- inc/: 公共头文件目录，可以按模块划分组织目录来保存模块相关头文件
- lib/: 生成库文件，linux下为.so和.a，windows下为.dll和.lib
- log/: 日志文件
- res/: 资源目录
- sample/: 样例程序目录
- src: 源代码
- thirdparty: 第三方库
- CMakeLists.txt: 项目构建配置文件，当然也有可能是其他类型的构建配置文件,比如bjam
- README.md: 项目的总体说明文件
