#  Python环境配置记录

https://mobaxterm.mobatek.net/download.html
以前使用的是 xshell,xftp,xmanage.本质上与新的软件的效果是一样的，但是 xmanage 是


watch -n 1 nvidia-smi









4.20晚上：
ssh -X -p 2241 lxin@202.38.68.70

scp -P 2241 -r D:\Desktop\局部路径规划\DQN_pytorch-master\DQN_pytorch-master\ lxin@202.38.68.70:~/DQN/
/data/dataset/lxin/cd-metadl-main/baselines/baseline4_dino


ssh -p  2253  lxin@202.38.68.70
total/test3


ssh -L 16006:127.0.0.1:5011  -p 2253 lxin@202.38.68.70

D:\Desktop\new\temp\mid_moreobs\mid\test.py

/ssd/lxin/anaconda3/lib/python3.9/site-packages
nohup python -u ~/nexp/total/train.py > train.log 2>&1 &
nohup python -u ~/nexp/total/train2.py > train2.log 2>&1 &




nohup python -u test5.6.py > t5.log 2>&1 &

nohup python -u test36.py > test36.log 2>&1 &

obstacles: 13

\# obstable_positions: []

\# obstable_positions:  [[40,0,5],[-40,0,5],[0,40,5],[0,-40,5]]

obstable_positions: [ [68,68,1],[25,107,1],[-103,157,1],[-102,-7,1]

,[13,-58,1],[66,-8,1],[-16,5,1],[-16,21,1],[-16,37,1],[-16,53,1],[0,0,1],[16,0,1],[32,0,1]]

torchlayers.py

~/anaconda3/envs/gymlab/lib/python3.8/site-packages/stable_baselines3/dqn/dqn.py

ssh -p  22237 lxin@202.85.220.177

ssh -L 16006:127.0.0.1:5000 -p 22237 lxin@202.85.220.177

CUDA_VISIBLE_DEVICES=1 python train.py

tensorboard --logdir=/home/.../...

http://127.0.0.1:16006

ssh -L 16006:127.0.0.1:5000 -p 39218 lx@202.38.69.241
ssh -p 39218 lx@202.38.69.241

ssh -p 22 lxin@103.59.149.110

ssh -L 16006:127.0.0.1:5000 -p 22 lxin@103.59.149.110

wget https://repo.anaconda.com/archive/Anaconda3-2021.11-Linux-x86_64.sh

 bsah Anaconda3-2021.11-Linux-x86_64.sh

vim .bashrc：编辑，在文件末尾添加export PATH=$PATH:/data/lxin/anaconda3/bin

source .bashrc

conda info --envs
conda env list

##  pytorch 安装记录



首先添加源

清华源

conda config --add channels https://mirrors.tuna.tsinghua.edu.cn/anaconda/pkgs/free/
conda config --add channels https://mirrors.tuna.tsinghua.edu.cn/anaconda/pkgs/main/
conda config --set show_channel_urls yes



保险起见，同时添加第三方源

conda config --add channels https://mirrors.tuna.tsinghua.edu.cn/anaconda/cloud/conda-forge/
conda config -y-add channels https://mirrors.tuna.tsinghua.edu.cn/anaconda/cloud/msys2/
conda config --add channels https://mirrors.tuna.tsinghua.edu.cn/anaconda/cloud/bioconda/
conda config --add channels https://mirrors.tuna.tsinghua.edu.cn/anaconda/cloud/menpo/
conda config --add channels https://mirrors.tuna.tsinghua.edu.cn/anaconda/cloud/pytorch/



在pytorch官网https://pytorch.org/查找安装命令；

注意：要去掉-c pytorch 才能是从镜像源下载，加快速度。

#  gym

从本地向服务器传输文件：

scp -P 39218 -r D:\Desktop\局部路径规划\DQN_pytorch-master\DQN_pytorch-master\ lx@202.38.69.241:~/DQN/

从服务器下载：

```
scp -r username@servername:/var/www/remote_dir/（远程目录） /var/www/local_dir（本地目录）
```



https://github.com/liux-n/arena-rosnav/blob/local_planner_subgoalmode/docs/eval_28032021.md

nohup python -u test2.py > test.log 2>&1 &
nohup 不挂起的意思

python test.py python 运行test.py文件

-u 代表程序不启用缓存，也就是把输出直接放到log中，没这个参数的话，log文件的生成会有延迟

test.log 将输出日志保存到这个log中

2>1 2与>结合代表错误重定向，而1则代表错误重定向到一个文件1，而不代表标准输出；

2>&1 &与1结合就代表标准输出了，就变成错误重定向到标准输出.

& 最后一个& ，代表该命令在后台执行


python main.py train --task-id 0 --gpu 0

# Win下python安装Atari游戏报错OSError: [WinError 126]

具体解决办法就是：

> 先 pip uninstall atari_py
> 再 pip install --no-index -f https://github.com/Kojoley/atari-py/releases atari_py

原因是原来安装的是旧版，需要卸载重新安装新版本。



3.7晚上：HW4，在8e4可以达到收敛；但是此时的训练环境依旧比较简单，动态障碍物初始时在一条直线上，而且小车的出发点和目标点都是固定的。

qpalzm159qpalzm159

 

```
conda install pytorch==1.10.2 torchvision torchaudio cudatoolkit=11.3 -c pytorch
```

