# Verilog-to-Bitstream2.0
在构建VTB的时候遇到的问题及解决办法

## 运行系统及依赖项版本
>* VTB基于`linux32位系统`运行，我们使用的虚拟机VMware运行linux系统，采用的版本为`Ubuntu16`，32位linux系统。<br>
>* 安装依赖项<br>
>>* 安装Subversion<br>
```Bash
    sudo apt-get install subversion #版本默认为1.9.3
```
>>* 安装clang<br>
```Bash
    sudo apt-get install clang #版本为默认为3.8.0
```
>>* 安装VTR依赖 <br>
```Bash
    sudo apt-get install \
      build-essential \
      flex \
      bison \
      cmake \
      fontconfig \
      libcairo2-dev \
      libfontconfig1-dev \
      libx11-dev \
      libxft-dev \
      libgtk-3-dev \
      perl \
      liblist-moreutils-perl \
      python 
```
>>* 附加软件包 <br>
```Bash
    sudo apt-get install \
      doxygen \
      python-sphinx \
      python-sphinx-rtd-theme \
      python-recommonmark
```
>>* 开发依赖包<br>
```Bash
    sudo apt-get install \
      git \
      valgrind \
      gdb \
      ctags
```
## VTR-7.0编译
> 打开终端，进入`VTR-7.0`根目录,执行make
>> 可能会出现的错误：
>>>* 在执行odin编译时出现
