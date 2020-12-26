## 筛选某一行的上一行，并且对目标行其中的数字求均值
> cat spp_sengine_proxy.INFO | grep -B 1 "return trpc rsp len" | grep "Malloc Size" | grep -Eo '[0-9]+$' |  awk '{ total += $1; count++ } END { print total/count }'

## sed 修改文件内容
> sed  -i 's/properties/property/g'  build.xml
