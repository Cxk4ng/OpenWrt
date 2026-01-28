## 固件下载

```ini
OpenWrt
  ├── LEDE (2016年分裂)
  │       └── 2018年合并回 OpenWrt
  │
  ├── ImmortalWrt（基于 OpenWrt/LEDE，国内社区分支）
  │
  └── iStoreOS（基于 OpenWrt/ImmortalWrt/LeanWrt 等，主打易用性和插件）
```



### 官方原版

* OpenWrt
    * https://github.com/openwrt/openwrt

* ImmortalWrt
    * https://github.com/immortalwrt/immortalwrt  📌




### 二次开发

* Lean版 (偶尔会打包闭源组件)
    * https://github.com/coolsnowwolf/lede 

* Lienol版 
    * https://github.com/Lienol/openwrt

* hanwckf版
    * https://github.com/hanwckf/immortalwrt-mt798x


*   iStoreOS
    * https://github.com/istoreos/istoreos 📌



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

* https://github.com/tindy2013/subconverter
* https://github.com/MetaCubeX/subconverter (支持vless reality协议)



**Docker服务搭建**

* https://hub.docker.com/r/tindy2013/subconverter



**IOS设备搭建**

* https://github.com/sub-store-org/Sub-Store





## 配置模板 📌

> 推荐精简版(local.yaml | remote-mini.ini) `大陆白名单模式` + `url-test`



### 远程配置

* https://raw.githubusercontent.com/cxk4ng/OpenWrt/main/remote-mini.ini
* https://raw.githubusercontent.com/cxk4ng/OpenWrt/main/remote-full.ini



### 本地配置

* https://raw.githubusercontent.com/cxk4ng/OpenWrt/main/local.yaml





## 分流规则

### 节点分类

```ini
# 自动选择 (间隔:300ms 容差:5ms 并发:100)
custom_proxy_group=🇭🇰 香港节点`url-test`(香港|HK|Hong Kong|Hongkong)`http://www.gstatic.com/generate_204`300,5,100
custom_proxy_group=🇨🇳 台湾节点`url-test`(台湾|TW|Taiwan)`http://www.gstatic.com/generate_204`300,5,100
custom_proxy_group=🇰🇷 韩国节点`url-test`(韩国|KR|Korea|KOR)`http://www.gstatic.com/generate_204`300,5,100
custom_proxy_group=🇯🇵 日本节点`url-test`(日本|JP|Japan|Tokyo)`http://www.gstatic.com/generate_204`300,5,100
custom_proxy_group=🇸🇬 狮城节点`url-test`(狮城|新加坡|SG|Singapore)`http://www.gstatic.com/generate_204`300,5,100
custom_proxy_group=🇺🇲 美国节点`url-test`(美国|US|United States|Seattle)`http://www.gstatic.com/generate_204`300,5,100
custom_proxy_group=🇨🇦 加国节点`url-test`(加拿大|CA|Canada)`http://www.gstatic.com/generate_204`300,5,100

# 手动选择
custom_proxy_group=🎏 亚洲国家`select`(澳门|朝鲜|印度|印度尼西亚|印尼|土耳其|伊朗|泰国|巴基斯坦|菲律宾|马来西亚|越南|缅甸|柬埔寨|迪拜|以色列|阿联酋|India)
custom_proxy_group=🏰 欧洲国家`select`(俄罗斯|德国|土耳其|法国|英国|意大利|西班牙|乌克兰|波兰|荷兰|葡萄牙|比利时|爱尔兰|匈牙利|摩尔多瓦|German|French|United Kingdom|London|Russia|Moscow)
custom_proxy_group=🗺︎ 美洲国家`select`(巴西|墨西哥|哥伦比亚|阿根廷|秘鲁|委内瑞拉|智利|厄瓜多尔|玻利维亚)
custom_proxy_group=🦘 澳洲国家`select`(澳大利亚|巴布亚新几内亚|新西兰|新喀里多尼亚|斐济|悉尼|Australia)
custom_proxy_group=🌍 非洲国家`select`(南非|埃及|尼日利亚|South Africa|Egypt)
```



### 参考资料

> 非常感谢ACL4SSR&blackmatrix7&Tindy2013 等大佬的无私奉献

* https://wiki.metacubex.one/config/
* https://github.com/ACL4SSR/ACL4SSR/tree/master/Clash/Ruleset
* https://github.com/blackmatrix7/ios_rule_script/tree/master/rule/Clash
