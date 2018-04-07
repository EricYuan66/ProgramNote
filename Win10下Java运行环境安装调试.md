# Win10 下Java运行环境安装，Javac命令无法识别问题解决
### 1 下载对应操作系统版本的JDK，64位操作系统使用64位的JDK
### 2 安装JDK，JDK安装过程中会自动安装JRE
### 3 环境变量配置
- #### 3.1 **在Win10中，因为系统的限制，path 变量只可以使用 JDK 的绝对路径。%JAVA_HOME% 会无法识别，导致配置失败。**
- #### 3.2 Path环境变量：PATH变量用来告诉操作系统到指定目录去查找一个命令。
   - Path变量值1：C:\Program Files\Java\jdk1.7.0_80\bin
   - Path变量值2：C:\Program Files\Java\jdk1.7.0_80\jre\bin
   - **Win10中Path变量设置注意点2：两个环境变量必须分别设置在两行中，不能在一行之中设置两个环境变量，即使用 ；隔离也不行，否则javac命令会报查找不到该命令。**
- #### 3.3 CLASSPATH环境变量
   - CLASSPATH变量环境：CLASSPATH是编译或运行Java程序时用来告诉Java编译器或虚拟机到指定目录查找Java类文件
   - 新建CLASSPATH变量值：.;C:\Program Files\Java\jdk1.7.0_80\lib\dt.jar;C:\Program Files\Java\jdk1.7.0_80\lib\tools.jar
### 4 cmd运行中输入java, java -version, javac 等命令，

