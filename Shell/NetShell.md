## tcpdump 抓包 ip
>  sudo tcpdump -i eth1 host 9.223.245.208 -w ./target6.cap

## tcpdump 抓包 prot, 回环端口
> sudo tcpdump -i lo port 10086 -w ./target6.cap

## tcpdump 抓包端口 udp包
> tcpdump -i lo udp port  端口号 -X


