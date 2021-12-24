
🔷使用
- 打开 https://github.com/vinograd-cyber/GeoIP 看到的都是最新版本。
- 下载 [h1y.dat](https://raw.githubusercontent.com/vinograd-cyber/GeoIP/main/geoip.dat) 域名文件放到 v2ray或xray的资源目录中，域名文件的标签支持cn/gfw/rej三种，在 v2ray或xray 配置文件中按标签设定路由规则，所有的域名均以子域名的形式进行匹配。
- [v2ray路由配置示例](https://github.com/vinograd-cyber/GeoIP/blob/main/routing.json)

🔷下载
- [h1y.dat](https://raw.githubusercontent.com/vinograd-cyber/GeoIP/main/h1y.dat)
- [geoip.dat](https://raw.githubusercontent.com/vinograd-cyber/GeoIP/main/geoip.dat)

🔷特别说明：
- 📌域名文件h1y.dat：
  - ext:h1y.dat:cn 直连中国（国内）的网站
  - ext:h1y.dat:gfw 代理被GFW屏蔽的网站
  - ext:h1y.dat:rej 屏蔽广告和欺诈性网站
- 📌IP文件geoip.dat：
  - geoip:cn 直连中国（国内）的网站
  - geoip:rej 屏蔽广告和欺诈性网站
