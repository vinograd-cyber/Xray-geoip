V2Ray-SiteDAT
用于 Project V（v2ray）和Project X（xray）的自定义域名文件。

使用
下载 geofiles 文件夹中的 h1y.dat 域名文件放到 v2ray或xray的资源目录中（通常是v2ray/bin/或xray/bin/），域名文件的标签支持cn/gfw/rej三种，在 v2ray或xray 配置文件中（通常是etc/config.json）按标签设定路由规则，所有的域名均以子域名的形式进行匹配。

✔特别说明：

✳域名文件h1y.dat支持三种标签cn/gfw/rej
  - h1y.dat:cn 常见中国站点的域名（用以直连）
    - 举例：
      - {
          "type": "field",
          "outboundTag": "direct",
          <b>"domain": [
            "ext:h1y.dat:cn"
          ]</b>
        }
  - h1y.dat:gfw 被GFW屏蔽的站点域名（用以代理）
    - 举例：
      - {
          "type": "field",
          "outboundTag": "proxy",
          <b>"domain": [
            "ext:h1y.dat:gfw"
          ]</b>
        },
      
  - h1y.dat:rej 广告和钓鱼网站的域名（用以屏蔽）
    - 举例：
      - {
          <b>"domain": [
            "ext:h1y.dat:rej",
          ]</b>,
          "type": "field",
          "outboundTag": "block"
        }, 

❤致谢
- https://github.com/v2ray/domain-list-community
- https://oisd.nl
