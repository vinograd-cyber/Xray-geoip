# GeoIP

🟢为何制作h1y.dat和geoip.dat

- 很多时候，V2Ray内置的域名不能满足使用，不过 V2Ray 可以使用外部自定义的域名文件，特制了h1y.dat，可以供大家用于 Project V（V2Ray）和Project X（XRay）的自定义域名文件。
这个域名文件每天自动更新，如果你使用了我提供的域名文件也请定期更新。
- 相比于官方原版的geoip.dat：
  - 中国大陆的IPV4地址数据采用了[APNIC](https://www.apnic.net)的最新数据
  - geoip:rej 屏蔽广告和欺诈性网站
- 打开 https://github.com/y823/GeoIP 看到的都是最新版本。

🟢使用

- 下载 [h1y.dat](https://raw.githubusercontent.com/y823/GeoIP/main/geoip.dat) 域名文件放到 v2ray或xray的资源目录中（通常是v2ray/bin/或xray/bin/），域名文件的标签支持cn/gfw/rej三种，在 v2ray或xray 配置文件中（通常是etc/config.json）按标签设定路由规则，所有的域名均以子域名的形式进行匹配。
- [v2ray路由配置示例](https://github.com/y823/GeoIP/blob/main/routing.json)

🟢下载
- [h1y.dat](https://raw.githubusercontent.com/y823/GeoIP/main/h1y.dat)
- [geoip.dat](https://raw.githubusercontent.com/y823/GeoIP/main/geoip.dat)

✔🟢特别说明：

- 📌域名文件h1y.dat支持三种标签cn/gfw/rej
  - 🟨h1y.dat:cn 直连中国（国内）的网站
    
  - 🟦h1y.dat:gfw 代理被GFW屏蔽的网站
      
  - 🟥h1y.dat:rej 屏蔽广告和欺诈性网站

❤🟢致谢
- https://v2ray.com
- https://v2fly.org
- https://xtls.github.io
- https://adaway.org
- https://github.com/gfwlist/gfwlist
