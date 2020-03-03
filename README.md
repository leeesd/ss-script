#
1、安装BBR魔改版
wget -N --no-check-certificate https://raw.githubusercontent.com/FunctionClub/YankeeBBR/master/bbr.sh && bash ./bbr.sh install
蓝底窗⼝按tab键，选NO回车
输入Y重启
bash bbr.sh start
2、安装SS
wget --no-check-certificate -O shadowsocks-libev-debian.sh https://raw.githubusercontent.com/teddysun/shadowsocks_install/master/shadowsocks-libev-debian.sh
chmod +x shadowsocks-libev-debian.sh
./shadowsocks-libev-debian.sh 2>&1 | tee shadowsocks-libev-debian.log
3、安装KCPTUN
wget --no-check-certificate https://github.com/kuoruan/shell-scripts/raw/master/kcptun/kcptun.sh
chmod +x ./kcptun.sh
./kcptun.sh
4、安装客户端（支持win、os、安卓、ios）
配置kcptun插件：
key=4431080;crypt=aes;mode=fast2;mtu=1350;sndwnd=1024;rcvwnd=1024;datashard=10;parityshard=3;dscp=0
