git clone https://git.lede-project.org/source.git

./scripts/feeds update -a

# se openvpn openssl anche luci openssl, altrimenti mbedtls
./scripts/feeds install olsrd luci-app-olsr openvpn netdiscover etherwake tcpdump-mini iperf iptraf-ng arp-scan luci-app-commands luci luci-ssl-openssl luci-ssl

# routing dinamico
./scripts/feeds install bird4 luci-app-bird4 

# printer server
./scripts/feeds install p910nd luci-app-p910nd

make menuconfig
make defconfig

scripts/diffconfig.sh > mydiffconfig2

