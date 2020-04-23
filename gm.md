fabric v1.4.3 国密改造
国密改造参照https://blog.csdn.net/dyj5841619/article/details/90642808
在fabric 1.4.3上修改并完成调试； 并修改此项目vendor第三方库，所以请不要替换vendor目录

1 编译设置
设置export GO111MODULE=off 关闭go modele功能

2 编译peer 
make peer
二进制生层.build/bin/peer

3 编译orderer
make orderer

4 编译其他工具
#   - configtxgen - builds a native configtxgen binary
#   - configtxlator - builds a native configtxlator binary
#   - cryptogen  -  builds a native cryptogen binary

make configtxgen
make configtxlator
make cryptogen

至此，二进制fabric编译完成
