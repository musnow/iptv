# iptv
提取自湖南邵阳电信组播地址。

组播内容来自http://10.255.9.200/IPTV_EPG/Channel/GetChannelsList?&version=YYS.5.9.7.266.6.HNDXIPTV.0.0_Release_ZTE_4K

使用itv端口拨号获取内网 `10.139.x.x` 后使用rtp2httpd进行转单播地址，其中 `http://192.168.10.1:5140` 替换成你的rtp2httpd地址，fcc地址如果是邵阳电信应该是正确的。

需要使用tvg-logo及访问iptv内网请设置静态路由表。

| 接口 | 目标 | 	类型 |
| ----- | ----- |----- |
| iptv | 124.232.131.0/24 | unicast |
| iptv | 124.232.135.225/32 | unicast |
| iptv | 124.232.149.44/32 | unicast |
| iptv | 124.232.231.172/32 | unicast |
| iptv | 222.246.132.231/32 | unicast |
| iptv | 220.168.138.0/24 | unicast |
| iptv | 220.168.139.0/24 | unicast |
| iptv | 175.10.54.0/24 | unicast |
| iptv | 61.150.160.0/24 | unicast |
| iptv | 239.76.0.0/16 | unicast |
| iptv | 10.0.0.0/8 | unicast |
