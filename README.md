## asuswrt-merlin New Gen for K3(version 382.xx and higher)

This project forks form Asuswrt-Merlin, the goal is to fit for PHICOMM-K3.


## features

1.Based entirely on asuswrt-merlin.ng.

2.Fixed kernel boot & gpio for K3, no error in TTL.

3.Transplant CFE code from src-rt-7.x.main to K3, router will not crash.

4.Adding K3 screen control util, screen is full function now.

5.Some extra CN & TW translation.


## how to build

Firsr of all you should modify cfe MAC address to your own in rt-k3_nvram.txt

where to modify:

et0macaddr=00:11:22:33:44:55 -> et0macaddr=XX:XX:XX:XX:XX:XX

XX:XX:XX:XX:XX:XX means your own MAC address.

---------------

Added model RT-K3, use "make rt-k3" to compile and gen trx image.

Use "make" in /release/src-rt-7.14.114.x/src/cfe/build/broadcom/bcm947xx/ to compile cfe separately.

---------------

Output folder:

TRX image: in release/src-rt-7.14.114.x/src/image/

CFE image: in release/src-rt-7.14.114.x/src/cfe/

(CFE has copied to /rom/etc/ in TRX)


## Additional pack(put into release/src/router/)

K3screenctrl - https://github.com/ghostnup/k3screenctrl


## Credits

ASUS

[RMerl](https://github.com/RMerl/) for makeing up asuswrt-merlin.ng

Lostlonger for research transplant from merlin to K3

[MerlinRdev](https://github.com/MerlinRdev/) for sharing K3-merlin.ng source code

[Updateing](https://github.com/Updateing/) for making screen usable

## 打赏我(buy me a beer)

![alipay](https://s1.ax1x.com/2020/05/24/YxgA9f.jpg)
![wechat](https://s1.ax1x.com/2020/05/24/YxgVgS.jpg)
