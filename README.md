# GeoIP

🟢为何制作h1y.dat

- 很多时候，V2Ray内置的域名不能满足使用，不过 V2Ray 可以使用外部自定义的域名文件，刚好我也制作了一个，可以供大家用于 Project V（V2Ray）和Project X（XRay）的自定义域名文件。
这个域名文件每天自动更新，如果你使用了我提供的域名文件也请定期更新。
- 打开 https://github.com/y823/V2Ray-SiteDAT/tree/main/geofiles 看到的都是最新版本。

🟢使用

- 下载 geofiles 文件夹中的 h1y.dat 域名文件放到 v2ray或xray的资源目录中（通常是v2ray/bin/或xray/bin/），域名文件的标签支持cn/gfw/rej三种，在 v2ray或xray 配置文件中（通常是etc/config.json）按标签设定路由规则，所有的域名均以子域名的形式进行匹配。
- [v2ray路由配置示例](https://github.com/y823/V2Ray-SiteDAT/blob/main/routing.json)

🟢下载
- [h1y.dat](https://raw.githubusercontent.com/y823/V2Ray-SiteDAT/main/geofiles/h1y.dat)

✔🟢特别说明：

- 📌域名文件h1y.dat支持三种标签cn/gfw/rej
  - 🟨h1y.dat:cn 直连中国（国内）的网站
    - 路由配置实例：
      - {
          "type": "field",
          "outboundTag": "direct",
          <b>"domain": [
            "ext:h1y.dat:cn"
          ]</b>
        }
  - 🟩h1y.dat:gfw 代理被GFW屏蔽的网站
    - 路由配置示例：
      - {
          "type": "field",
          "outboundTag": "proxy",
          <b>"domain": [
            "ext:h1y.dat:gfw"
          ]</b>
        }
      
  - 🟥h1y.dat:rej 屏蔽广告和欺诈性网站
    - 路由配置示例：
      - {
          <b>"domain": [
            "ext:h1y.dat:rej",
          ]</b>,
          "type": "field",
          "outboundTag": "block"
        }

❤🟢致谢
- https://v2ray.com
- https://v2fly.org
- https://xtls.github.io
- https://adaway.org
- https://github.com/gfwlist/gfwlist
