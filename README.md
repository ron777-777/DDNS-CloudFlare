# DDNS-CloudFlare
这是DDNS的脚本基于CloudFLare平台，在现有脚本上做了可以更改代理的选项，更为自由。
```
sudo wget https://raw.githubusercontent.com/ron777-777/DDNS-CloudFlare/main/cf-v4-ddns.sh
sudo chmod +x cf-v4-ddns.sh
sudo vim cf-v4-ddns.sh
```
修改  
`CFKEY`  
在此获取https://www.cloudflare.com/a/account/my-account  
`CFUSER`  
`CFZONE_NAME`  
`CFRECORD_NAME`  
`CFRECORD_TYPE`  
`PROXY`  
`CFTTL`  
`FORCE`  
定时更新使用
`crontab -e`
在最后加上
`*/2 * * * * /root/cf-v4-ddns.sh >/dev/null 2>&1`  

更详细的教程参考https://cloud.tencent.com/developer/article/1947620

