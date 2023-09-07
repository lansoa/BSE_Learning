#### Sun.

**git set vim **

```
 git config --global core.editor "vim"
 export GIT_EDITOR=vim
```

```
./scripts/checkpatch.pl HEAD~~~..HEAD
```



##### **git use**

```
git remote add lslab http://foxsen.3322.org:33336/binarytranslation/x86-qemu-mips.git
```

```
git push origin HEAD:refs/for/master
```



```
git config --global credential.helper store
```

```
git am patch
git apply --reject
git status
git add 
git am --continue
```



````
git checkout feature
git rebase master
````

**return the commits point, which is the branchs share.**

```
git stash        //stash  current change
git stash list   //list the current stash 
git stash pop    //use the stash 
```

```python
 export http_proxy=""
```

```
164 ./gzip_base.prefetch input.compressed 2 
175 ./vpr_base.prefetch net.in arch.in place.out dum.out -nodisp -place_only -init_t 5 -exit_t 0.005 -alpha_t 0.9412 -inner_num 2 
175 ./vpr_base.prefetch net.in arch.in place.in route.out -nodisp -route_only -route_chan_width 15 -pres_fac_mult 2 -acc_fac 1 -first_iter_pres_fac 4 -initial_pres_fac 8 
176 ./cc1_base.prefetch cccp.i -o cccp.s    
181 ./mcf_base.prefetch inp.in 
186 ./crafty_base.prefetch < crafty.in 
197 ./parser_base.prefetch 2.1.dict -batch < test.in 
252 ./eon_base.prefetch chair.control.cook chair.camera chair.surfaces chair.cook.ppm ppm pixels_out.cook 
253 ./eon_base.prefetch chair.control.rushmeier chair.camera chair.surfaces chair.rushmeier.ppm ppm pixels_out.rushmeier 
253 ./eon_base.prefetch chair.control.kajiya chair.camera chair.surfaces chair.kajiya.ppm ppm pixels_out.kajiya 
253 ./perlbmk_base.prefetch -I. -I./lib test.pl < test.in 
254 ./gap_base.prefetch -l ./ -q -m 64M < test.in 
255 ./vortex_base.prefetch lendian.raw 
256 ./bzip2_base.prefetch input.random 2 
300 ./twolf_base.prefetch test 
168 ./wupwise_base.prefetch.la 
171 ./swim_base.prefetch.la < swim.in 
172 ./mgrid_base.prefetch.la < mgrid.in 
173 ./applu_base.prefetch.la < applu.in 
177 ./mesa_base.prefetch.la -frames 10 -meshfile mesa.in -ppmfile mesa.ppm
178 ./galgel_base.prefetch.la < galgel.in 
179 ./art_base.prefetch.la -scanfile c756hel.in -trainfile1 a10.img -stride 2 -startx 134 -starty 220 -endx 139 -endy 225 -objects 1 
183 ./equake_base.prefetch.la < inp.in 
187 ./facerec_base.prefetch.la < test.in 
188 ./ammp_base.prefetch.la < ammp.in 
189 ./lucas_base.prefetch.la < lucas2.in 
191 ./fma3d_base.prefetch.la 
200 ./sixtrack_base.prefetch.la < inp.in 
301 ./apsi_base.prefetch.la 

```

### mount 

```
UUID=21d5172f-b250-40b3-8254-db0a912d4b7a /home/lan/mnt ext4 defaults  0  2


第一个数字：0表示开机不检查磁盘，1表示开机检查磁盘； 
第二个数字：0表示交换分区，1代表启动分区（Linux），2表示普通分区 
我挂载的分区是在WIn系统下创建的分区，磁盘格式为ntfs
```

#### AMDGPU

```
sudo apt-get dist-upgrade
sudo apt-get --fix-missing
```

#### LINUX

##### keyboard shortcuts

```
ctrl+c - SIGINT
ctrl+z - SIGTSTP
ctrl+\ - SIGQUIT

ctrl+a: cursor jump to the beginningx
ctrl+b: 光标左移一个字母。
ctrl+c: 杀死当前进程。
ctrl+d: 删除光标后一个字符或exit、logout。
ctrl+e: cursor jump to the ending
ctrl+f：向后移一个字符。
ctrl+h: 删除光标前一个字符，同backspace键相同。
ctrl+k: 剪切光标后至行尾的内容。
ctrl+l: 清屏，相当于clear。
Ctrl+p：重复上一次命令。
ctrl+r: 搜索之前的命令历史。多次ctrl+r 会一直向上搜索。
ctrl+u: 剪切光标前至行首间的所有内容。
ctrl+w: 剪切前面的字符至上一个空格处。
ctrl+t: 交换光标位置前的两个字符。
ctrl+y: 粘贴或者恢复上次的删除。
ctrl+z: 把当前进程转到后台运行，使用fg命令恢复。
Ctrl+x: 跳回之前移动的原位置。
ctrl+m: 等同于回车键
ctrl+o: 等同于回车键
ctrl+s: 暂时冻结当前shell的输入
ctrl+q: 解冻
```



```
getconf PAGESIZE
```



```
bash-completion
```

#### Ubuntu

```
换源
/etc/apt/sources.list

sudo pam_tally2 -r -u ubuntu
```

#### Password

```
中国科训：
Ls13947024532--
```

#### SSH

```
sudo apt-get install openssh-server

安装ssh服务
sudo apt-get install openssh-server
启动ssh服务
sudo /etc/init.d/ssh start
设置开机自启动	
sudo systemctl enable ssh
关闭ssh开机自动启动命令
sudo systemctl disable ssh
单次开启ssh
sudo systemctl start ssh
单次关闭ssh
sudo systemctl stop ssh
设置好后重启
reboot

remember password 
ssh-copy-id id@server
```

#### vim

```
set mouse=a

ctrl+w paste string from y
```

#### Fonts

```
sudo mkdir -p /usr/share/fonts/winFonts
sudo cp ~/Desktop/font/*.ttf /usr/share/fonts/winFonts/
sudo chmod 644 /usr/share/fonts/winFonts/*.ttf
cd /usr/share/fonts/winFonts/
sudo mkfontscale #（创建雅黑字体的fonts.scale文件，它用来控制字体旋转缩放）
sudo mkfontdir #（创建雅黑字体的fonts.dir文件，它用来控制字体粗斜体产生）
sudo fc-cache -fv #（建立字体缓存信息，也就是让系统认识雅黑）
```

#### bashrc

```
/etc/profile：系统配置文件，用户登录时读取一次
/etc/bash.bashrc：系统配置文件 ，用户登录时读取一次，每次打开一个新终端会话时读取一次
~/.profile（~/.bash_profile、~/.bash_login）：用户配置文件，用户登录时读取一次
~/.bashrc：用户配置文件，用户登录时读取一次，每次打开一个新终端会话时读取一次
```

#### grep

| Character | Matches                                                      |
| --------- | ------------------------------------------------------------ |
| ^         | The beginning of a text line                                 |
| $         | The end of a text line                                       |
| .         | Any single character                                         |
| [...]     | Any single character in the bracketed list or range          |
| [^...]    | Any character not in the list or range                       |
| *         | Zero or more occurrences of the preceding character or regular expression |
| .*        | Zero or more occurrences of any single character             |
| \         | The escape of special meaning of next character              |

#### passwd

```
passwd username 
vi /etc/pam.d/common-password
password	requisite 			pam_cracklib.so retry=3 minlen=8 minclass=3 enforce_for_root

password    sufficient    pam_unix.so sha512
password    required      pam_deny.so
```

pam_tally2 --user=loongson --reset 



#### DD

```
lsblk
umount 
lsblk 
sudo dd if=Loongnix-20.2.livecd.mate.loongarch64.en.iso of=/dev/sdb bs=1M
```





#### UZ

```
unzip -O CP936


```



#### Docker

```
    docker save imageID > filename
    docker load < filename
```



##### UNIPUS 

```
passwd Lanshuo1997
```



#### Keyboard remap

```bash
vi ~/.Xmodmap

keycode 105 = Caps_Lock NoSymbol Caps_Lock
keycode 66 = Control_R NoSymbol Control_R

clear lock
clear control


add lock = Caps_Lock
add control = Control_L Control_R
	

```



### sudoers

```
sudo vim /etc/sudoers

# User privilege specification
root ALL=(ALL:ALL) ALL
jerry ALL=(ALL:ALL) ALLz
```





### dhclient

get ip addr from network machine





### tmux

```
copy mode 

space is start to copy
enter is copy to clipboard

```



### ip/mac

```
arp -a 10.20.4.24

-a # 主机 ：显示 arp 缓冲区的所有条目；
-H # 地址类型 ：指定 arp 指令使用的地址类型；
-d # 主机 ：从 arp 缓冲区中删除指定主机的 arp 条目；
-D # 使用指定接口的硬件地址；
-e # 以 Linux 的显示风格显示 arp 缓冲区中的条目；
-i # 接口 ：指定要操作 arp 缓冲区的网络接口；
-s # 主机 MAC 地址 ：设置指定的主机的 IP 地址与 MAC 地址的静态映射；
-n # 以数字方式显示 arp 缓冲区中的条目；
-v # 显示详细的 arp 缓冲区条目，包括缓冲区条目的统计信息；
-f # 文件 ：设置主机的 IP 地址与 MAC 地址的静态映射。
```



### useradd

```
sudo useradd -m lyz 
passwd lyz

chsh
```



