## 固件下载

### 官方原版

* https://github.com/openwrt/openwrt



### 二次开发

* Lean版 https://github.com/coolsnowwolf/lede

* Lienol版 https://github.com/Lienol/openwrt



### 三次开发

> 基于Lean版编译 整合了常用插件

* sirpdboy https://github.com/sirpdboy/openwrt  📌
* firker https://www.right.com.cn/forum/thread-1811791-1-1.html
* lusty https://www.right.com.cn/forum/thread-7667094-1-1.html
* Myan's https://www.right.com.cn/forum/thread-4062018-1-1.html
* jinjin https://www.right.com.cn/forum/thread-4051663-1-1.html
* xuanwumen https://www.right.com.cn/forum/thread-4091453-1-1.html
* zgxwc https://www.right.com.cn/forum/thread-3705778-1-1.html





## 订阅转换

### 在线转换

> 一定程度存在订阅泄露 或者访问不稳定情况

| 作者          | 介绍                             | 地址                           |
| ------------- | -------------------------------- | ------------------------------ |
| Tindy X 📌     | Sub 作者维护 Dler Cloud 机场赞助 | https://sub.dler.io/           |
| 友善的肥羊    | Subconverter 订阅转换前端增强版  | https://suburl.v1.mk/          |
| 品云订阅转换  | 品云官方订阅转换工具             | https://id9.cc/                |
| つつの · 鲸歌 | TAG 机场官方合作工具             | https://sub.tsutsu.one/        |
| immconvert    | ImmTelecom 机场官网订阅转换工具  | https://immconvert.com/        |
| Next Convert  | Nexitally 奶昔机场官方订阅转换   | https://nexconvert.com/        |
| ACL4SSR       | 知名的规则转换网站               | https://acl4ssr-sub.github.io/ |



### 本地转换

> 在线订阅存在泄露和访问不稳定问题 建议自己搭建本地订阅转换

**本地电脑搭建**

https://github.com/tindy2013/subconverter



**Docker服务搭建**

https://hub.docker.com/r/tindy2013/subconverter



**IOS设备搭建**

https://github.com/sub-store-org/Sub-Store





## 分流规则

### 我的模板

* https://raw.githubusercontent.com/cxk4ng/OpenWrt/main/ProxyGroups/rule.ini



### 节点分类

```ini
# 自动选择
custom_proxy_group=🇭🇰 香港节点`url-test`(香港|HK|Hong Kong|Hongkong)`http://www.gstatic.com/generate_204`300,,100
custom_proxy_group=🇨🇳 台湾节点`url-test`(台湾|TW|Taiwan)`http://www.gstatic.com/generate_204`300,,100
custom_proxy_group=🇰🇷 韩国节点`url-test`(韩国|KR|Korea|KOR)`http://www.gstatic.com/generate_204`300,,100
custom_proxy_group=🇯🇵 日本节点`url-test`(日本|JP|Japan)`http://www.gstatic.com/generate_204`300,,100
custom_proxy_group=🇺🇲 美国节点`url-test`(美国|US|United States)`http://www.gstatic.com/generate_204`300,,100
custom_proxy_group=🇸🇬 狮城节点`url-test`(狮城|新加坡|SG|Singapore)`http://www.gstatic.com/generate_204`300,,100

# 手动选择
custom_proxy_group=🇪🇺 欧洲国家`select`(俄罗斯|德国|土耳其|法国|英国|意大利|西班牙|乌克兰|波兰|荷兰|葡萄牙|比利时)
custom_proxy_group=🎏 亚洲国家`select`(印度|印度尼西亚|土耳其|伊朗|泰国|巴基斯坦|菲律宾|马来西亚|越南|缅甸|柬埔寨)
custom_proxy_group=🗺︎ 美洲国家`select`(巴西|墨西哥|哥伦比亚|阿根廷|加拿大|秘鲁|委内瑞拉|智利|厄瓜多尔|玻利维亚)
custom_proxy_group=🇦🇺 澳洲国家`select`(澳大利亚|巴布亚新几内亚|新西兰|新喀里多尼亚|斐济)
```



### 规则整理

```ini
# 国外媒体
ruleset=📹 YouTube,https://raw.githubusercontent.com/blackmatrix7/ios_rule_script/refs/heads/master/rule/Clash/YouTube/YouTube.list
ruleset=🎥 Netflix,https://raw.githubusercontent.com/blackmatrix7/ios_rule_script/refs/heads/master/rule/Clash/Netflix/Netflix.list
ruleset=🎵 Spotify,https://raw.githubusercontent.com/blackmatrix7/ios_rule_script/refs/heads/master/rule/Clash/Spotify/Spotify.list
ruleset=🏰 Disney,https://raw.githubusercontent.com/blackmatrix7/ios_rule_script/refs/heads/master/rule/Clash/Disney/Disney.list
ruleset=📺 Bahamut,https://raw.githubusercontent.com/blackmatrix7/ios_rule_script/refs/heads/master/rule/Clash/Bahamut/Bahamut.list

# 社交应用
ruleset=🕊 Twitter,https://raw.githubusercontent.com/blackmatrix7/ios_rule_script/refs/heads/master/rule/Clash/Twitter/Twitter.list
ruleset=☎ Telegram,https://raw.githubusercontent.com/blackmatrix7/ios_rule_script/refs/heads/master/rule/Clash/Telegram/Telegram.list
ruleset=📷 Instagram,https://raw.githubusercontent.com/blackmatrix7/ios_rule_script/refs/heads/master/rule/Clash/Instagram/Instagram.list
ruleset=⚙️ TikTok,https://raw.githubusercontent.com/blackmatrix7/ios_rule_script/refs/heads/master/rule/Clash/TikTok/TikTok.list

# 人工智能
ruleset=🧠 OpenAI,https://raw.githubusercontent.com/blackmatrix7/ios_rule_script/refs/heads/master/rule/Clash/OpenAI/OpenAI.list
ruleset=🌟 Gemini,https://raw.githubusercontent.com/blackmatrix7/ios_rule_script/refs/heads/master/rule/Clash/Gemini/Gemini.list
ruleset=👀 Copilot,https://raw.githubusercontent.com/blackmatrix7/ios_rule_script/refs/heads/master/rule/Clash/Copilot/Copilot.list

# 游戏平台
ruleset=🎮 Game,https://raw.githubusercontent.com/blackmatrix7/ios_rule_script/refs/heads/master/rule/Clash/Epic/Epic.list
ruleset=🎮 Game,https://raw.githubusercontent.com/blackmatrix7/ios_rule_script/refs/heads/master/rule/Clash/Steam/Steam.list
ruleset=🎮 Game,https://raw.githubusercontent.com/blackmatrix7/ios_rule_script/refs/heads/master/rule/Clash/Xbox/Xbox.list
ruleset=🎮 Game,https://raw.githubusercontent.com/blackmatrix7/ios_rule_script/refs/heads/master/rule/Clash/Sony/Sony.list
ruleset=🎮 Game,https://raw.githubusercontent.com/blackmatrix7/ios_rule_script/refs/heads/master/rule/Clash/Nintendo/Nintendo.list
ruleset=🎮 Game,https://raw.githubusercontent.com/blackmatrix7/ios_rule_script/refs/heads/master/rule/Clash/PlayStation/PlayStation.list
ruleset=🎮 Game,https://raw.githubusercontent.com/blackmatrix7/ios_rule_script/refs/heads/master/rule/Clash/Rockstar/Rockstar.list
ruleset=🎮 Game,https://raw.githubusercontent.com/blackmatrix7/ios_rule_script/refs/heads/master/rule/Clash/Battle/Battle.list
ruleset=🎮 Game,https://raw.githubusercontent.com/blackmatrix7/ios_rule_script/refs/heads/master/rule/Clash/Origin/Origin.list

# 苹果
ruleset=🍎 Apple,https://raw.githubusercontent.com/blackmatrix7/ios_rule_script/refs/heads/master/rule/Clash/Apple/Apple.list
ruleset=🍎 Apple,https://raw.githubusercontent.com/blackmatrix7/ios_rule_script/refs/heads/master/rule/Clash/AppleTV/AppleTV.list
ruleset=🍎 Apple,https://raw.githubusercontent.com/blackmatrix7/ios_rule_script/refs/heads/master/rule/Clash/AppStore/AppStore.list
ruleset=🍎 Apple,https://raw.githubusercontent.com/blackmatrix7/ios_rule_script/refs/heads/master/rule/Clash/AppleNews/AppleNews.list
ruleset=🍎 Apple,https://raw.githubusercontent.com/blackmatrix7/ios_rule_script/refs/heads/master/rule/Clash/AppleMusic/AppleMusic.list

# 谷歌
ruleset=📢 Google,https://raw.githubusercontent.com/blackmatrix7/ios_rule_script/refs/heads/master/rule/Clash/Google/Google.list
ruleset=📢 Google,https://raw.githubusercontent.com/blackmatrix7/ios_rule_script/refs/heads/master/rule/Clash/YouTubeMusic/YouTubeMusic.list
ruleset=📢 Google,https://raw.githubusercontent.com/blackmatrix7/ios_rule_script/refs/heads/master/rule/Clash/GoogleSearch/GoogleSearch.list
ruleset=📢 Google,https://raw.githubusercontent.com/blackmatrix7/ios_rule_script/refs/heads/master/rule/Clash/GoogleDrive/GoogleDrive.list

# 微软
ruleset=Ⓜ️ Microsoft,https://raw.githubusercontent.com/blackmatrix7/ios_rule_script/refs/heads/master/rule/Clash/GitHub/GitHub.list
ruleset=Ⓜ️ Microsoft,https://raw.githubusercontent.com/blackmatrix7/ios_rule_script/refs/heads/master/rule/Clash/OneDrive/OneDrive.list
ruleset=Ⓜ️ Microsoft,https://raw.githubusercontent.com/blackmatrix7/ios_rule_script/refs/heads/master/rule/Clash/Microsoft/Microsoft.list

# 国内直连
ruleset=🚩 国内直连,https://raw.githubusercontent.com/blackmatrix7/ios_rule_script/refs/heads/master/rule/Clash/Lan/Lan.list
ruleset=🚩 国内直连,https://raw.githubusercontent.com/blackmatrix7/ios_rule_script/refs/heads/master/rule/Clash/China/China.list
ruleset=🚩 国内直连,https://raw.githubusercontent.com/blackmatrix7/ios_rule_script/refs/heads/master/rule/Clash/Direct/Direct.list
ruleset=🚩 国内直连,https://raw.githubusercontent.com/blackmatrix7/ios_rule_script/refs/heads/master/rule/Clash/ChinaMax/ChinaMax.list
ruleset=🚩 国内直连,https://raw.githubusercontent.com/blackmatrix7/ios_rule_script/refs/heads/master/rule/Clash/ChinaIPs/ChinaIPs.list
ruleset=🚩 国内直连,https://raw.githubusercontent.com/blackmatrix7/ios_rule_script/refs/heads/master/rule/Clash/ChinaMedia/ChinaMedia.list

# 广告拦截
ruleset=🛑 广告拦截,https://raw.githubusercontent.com/blackmatrix7/ios_rule_script/refs/heads/master/rule/Clash/Privacy/Privacy.list
ruleset=🛑 广告拦截,https://raw.githubusercontent.com/blackmatrix7/ios_rule_script/refs/heads/master/rule/Clash/Hijacking/Hijacking.list
ruleset=🛑 广告拦截,https://raw.githubusercontent.com/blackmatrix7/ios_rule_script/refs/heads/master/rule/Clash/Advertising/Advertising.list
ruleset=🛑 广告拦截,https://raw.githubusercontent.com/blackmatrix7/ios_rule_script/refs/heads/master/rule/Clash/EasyPrivacy/EasyPrivacy.list

# 漏网之鱼
ruleset=🐟 漏网之鱼,[]FINAL
```



### 参考资料

> 非常感谢ACL4SSR&blackmatrix7&Tindy2013 等大佬的无私奉献

* https://github.com/ACL4SSR/ACL4SSR/tree/master/Clash/Ruleset
* https://github.com/blackmatrix7/ios_rule_script/tree/master/rule/Clash
