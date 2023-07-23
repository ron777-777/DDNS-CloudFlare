# DDNS-CloudFlare
这是DDNS的脚本基于CloudFLare平台，在@zanjie1999的脚本上做了可以更改代理的选项，更为自由。
```
sudo wget https://raw.githubusercontent.com/ron777-777/DDNS-CloudFlare/main/cf-v4-ddns.sh
sudo chmod +x cf-v4-ddns.sh
sudo vim cf-v4-ddns.sh
```
修改  
`CFKEY`  
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
`*/2 * * * * /usr/local/bin/cf-ddns.sh >/dev/null 2>&1` 

