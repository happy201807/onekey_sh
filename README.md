# ddns-obfs

使用腳本讓VPS自動更新DDNS  

ddns.sh

编译安装shadowsocks-libev

shadowsocks.sh

wget https://raw.githubusercontent.com/happy201807/ddns-obfs/main/shadowsocks.sh && bash shadowsocks.sh

编辑配置文件

nano /etc/ss.json

安装BBR加速

wget --no-check-certificate 

chmod +x bbr.sh

./bbr.sh

重启

lsmod | grep bbr    查看是否加载

编译安装obfs

obfs.sh

添加启动服务  

进入/usr/lib/systemd/system增加shadowsocks.service文件

开机启动服务

systemctl daemon-reload

systemctl start shadowsocks.service

开机自启

systemctl enable shadowsocks.service


