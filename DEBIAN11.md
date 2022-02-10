# debian 11

- sudo -i
```
echo 'deb https://mirrors.tencent.com/debian/ bullseye main' \
  > /etc/apt/sources.list &&\
echo 'deb https://mirrors.tencent.com/debian-security/ bullseye-security main' \
  >> /etc/apt/sources.list &&\
echo 'deb https://mirrors.tencent.com/debian/ bullseye-updates main' \
  >> /etc/apt/sources.list &&\
apt update && apt install -y vim ifstat openssh-server
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
# 安装postman 安装redis-cli
apt install snapd && service snapd start \
  && snap install postman \
  && snap install another-redis-desktop-manager
```

```
# https://docs.docker.com/engine/install/debian/
# 安装docker
apt install -y ca-certificates curl gnupg lsb-release \
  && curl -fsSL \
  https://download.docker.com/linux/debian/gpg | gpg --dearmor -o /usr/share/keyrings/docker-archive-keyring.gpg \
  && echo \
  "deb [arch=$(dpkg --print-architecture) signed-by=/usr/share/keyrings/docker-archive-keyring.gpg] https://download.docker.com/linux/debian \
  $(lsb_release -cs) stable" | sudo tee /etc/apt/sources.list.d/docker.list > /dev/null \
  && apt update && apt install -y docker-ce \
  && service start docker && docker version
```
