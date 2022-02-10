```
# 提权root
sudo -i

# 安装基础软件
apt update && apt install -y curl firefox vim openssh-server ifstat

# 安装优化工具
apt install -y gnome-tweak-tool
```

## 键鼠操作方式Mac化

所有程序找到优化

- 键盘和鼠标
  - 键盘 > 其他布局选项 > Ctrl键位置 > 左Alt和左Ctrl对换
  - 鼠标 > 模拟鼠标点击 > 两指点击模拟右键

## 开发套件
```
curl -O http://saas.rayrotate.com/clash-linux-amd64-v1.9.0.gz \
  && gunzip clash-linux-amd64-v1.9.0.gz \
  && mv clash-linux-amd64-v1.9.0 /usr/local/bin/clash \
  && cd /usr/local/bin/ && chmod +x clash \
  && wget -O config.yaml "https://n2.urltosub.com/link/DhF7gejPaogRvwvi?clash=1&log-level=info"
```
```
# 安装mysql-workbench
curl -O \
  https://cdn.mysql.com//Downloads/MySQLGUITools/mysql-workbench-community_8.0.26-1ubuntu20.04_amd64.deb \
  && dpkg -i mysql-workbench-community_8.0.26-1ubuntu20.04_amd64.deb; apt install -f -y
```
```
# 安装sublime-text
curl -O \
  https://download.sublimetext.com/Sublime%20Text%202.0.2%20x64.tar.bz2 \
  && mkdir -p /etc/devoops && tar -xjf Sublime*.tar.bz2 && mv 'Sublime Text 2' /etc/devoops \
  && ln -s /etc/devoops/Sublime\ Text\ 2/sublime_text   /usr/bin/subl
```
```
----- BEGIN LICENSE -----
Andrew Weber
Single User License
EA7E-855605
813A03DD 5E4AD9E6 6C0EEB94 BC99798F
942194A6 02396E98 E62C9979 4BB979FE
91424C9D A45400BF F6747D88 2FB88078
90F5CC94 1CDC92DC 8457107A F151657B
1D22E383 A997F016 42397640 33F41CFC
E1D0AE85 A0BBD039 0E9C8D55 E1B89D5D
5CDB7036 E56DE1C0 EFCC0840 650CD3A6
B98FC99C 8FAC73EE D2B95564 DF450523
------ END LICENSE ------
```
```
# 安装postman
snap install postman
```
```
# 安装Another Redis Desktop Manager
snap install another-redis-desktop-manager
```
