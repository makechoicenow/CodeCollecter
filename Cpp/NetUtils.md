## 获取指定网卡的ip地址
``` C++
string getEth0Ip(){
    FILE *fp;/*  */
    char buffer[80];
    fp=popen("ifconfig | grep -A1 BROADCAST | grep inet | awk '{print $2}'", "r");
    fgets(buffer,sizeof(buffer),fp);
    std::string str = std::string(buffer);
    str.resize (str.size () - 1);
    return str;
}
```
