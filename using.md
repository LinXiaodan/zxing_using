## 软件
VMware Workstation，cmake

## 系统
Ubuntu16.0

## 详细说明
因为使用电脑系统为windows10，要使用linux的cmake，所以采取在VMware Workstation上安装Ubuntu16.0的方法，cmake为之前已经安装好的（未安装的自行百度安装方法），使用“cmake --version”查询（好吧，原本装在虚拟机上的ubuntu要进行拍照，但是点击拍照就闪退，所以就又装了一个新的ubuntu在虚拟机上，补上cmake的安装方法以及安装包在cmake文件夹中）

## 使用步骤
1. 将zxing-cpp-master.zip在windows中解压到zxing-cpp-master后（也可以在Ubuntu中解压，具体方法自己查），将文件夹复制到Ubuntu中
2. ctrl+alt+t打开命令行，cd进入zxing-cpp-master中，依次执行以下指令
```
mkdir build
cd build
cmake ..
make 
```
3. 发现在zxing-cpp-master目录下出现build文件，且在里面具有可执行文件zxing
4. 在命令行输入“./zxing”回车，出现zxing执行文件的使用方式提示
5. 将一张条码图a.png复制到build文件中，在命令行输入"./zxing a.png"并回车，得到条码的解码内容
