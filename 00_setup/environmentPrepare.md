# **基础环境搭建**

### step1 Linux环境

1. 安装WLS Ubuntu

==2.3两步的安装需要在普通用户下进行==

2. 更新配置

```
sudo apt update && sudo apt upgrade -y
sudo apt install -y build-essential software-properties-common curl wget ca-certificates apt-transport-https gnupg lsb-release
```
3. 核心开发工具

编译工具
```
sudo apt install -y gcc g++ gfortran make cmake
```

并行计算环境MPI
```
sudo apt install -y mpich libmpich-dev
```

数学库(HPC Benchmark依赖)
```
sudo apt install -y libblas-dev libatlas-base-dev liblapack-dev
```

Python与虚拟环境管理
```
sudo apt install -y python3 python3-pip python3-venv
```

安装Miniconda
```
cd ~
wget https://repo.anaconda.com/miniconda/Miniconda3-latest-Linux-x86_64.sh
bash Miniconda3-latest-Linux-x86_64.sh
```

激活
```
source ~/.bashrc
conda create -n asc python=3.10 -y
conda activate asc
```
========================================== 到此==

git与版本管理工具
```
sudo apt install -y git git-lfs
//配置如下
git config --global user.name "你的GitHub用户名"
git config --global user.email "你的GitHub邮箱"
```

远程/会话管理
```
sudo apt install -y tmux htop tree zip unzip
```

文本编辑器与markdown协作环境
```
sudo apt install -y nano vim
```

### step2 基础命令行回顾

[done] 

