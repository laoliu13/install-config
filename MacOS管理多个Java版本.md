  1. 执行命令 /usr/libexec/java_home -V 检查本地是否安装了Java环境
  2. https://www.oracle.com/java/technologies/downloads Oracle官网下载JDK安装包
  3. 安装好后，打开 ~/.bash_profile 文件，添加以下内容
     
    ```
    # java版本  export
    export JDK8_HOME=/Library/Java/JavaVirtualMachines/jdk1.8.0_181.jdk/Contents/Home
    export JDK17_HOME=/Library/Java/JavaVirtualMachines/jdk-17.jdk/Contents/Home
    # alias 命令链接到 export 命令
    alias jdk8="export JAVA_HOME=$JDK8_HOME"
    alias jdk17="export JAVA_HOME=$JDK17_HOME"
    ```
  4. 执行命令 source ~/.bash_profile使配置生效
  5. 输入jdk8或者jdk17切换Java版本
