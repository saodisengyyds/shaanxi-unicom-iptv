# 联通 IPTV 单播直播源

本项目为纯净、独立的**联通宽带专属单播直播源**，共包含 **85 个频道**（央视全套、各大卫视、地方频道、少儿动画、高清专区等）。

免光猫单线复用，免路由器 IGMP 组播转换设置，连接联通宽带 Wi-Fi 即可直接播放。

---

## 📺 播放与订阅直连地址

可以直接复制以下链接添加到播放器（TiviMate、影视仓、DIYP 影音、MX Player、APTV 等）中：

| 源类型 | 格式 | CDN 加速直连地址（推荐） | 国内加速镜像直连 | GitHub 原生直连 |
| :--- | :---: | :--- | :--- | :--- |
| **主直播源**<br>(含台标/EPG/回看) | M3U | `https://cdn.jsdelivr.net/gh/saodisengyyds/unicom-iptv@main/unicom.m3u` | `https://gh-proxy.com/https://raw.githubusercontent.com/saodisengyyds/unicom-iptv/main/unicom.m3u` | `https://raw.githubusercontent.com/saodisengyyds/unicom-iptv/main/unicom.m3u` |
| **时移回看专线**<br>(43个频道) | M3U | `https://cdn.jsdelivr.net/gh/saodisengyyds/unicom-iptv@main/unicom_playback.m3u` | `https://gh-proxy.com/https://raw.githubusercontent.com/saodisengyyds/unicom-iptv/main/unicom_playback.m3u` | `https://raw.githubusercontent.com/saodisengyyds/unicom-iptv/main/unicom_playback.m3u` |
| **机顶盒纯文本源** | TXT | `https://cdn.jsdelivr.net/gh/saodisengyyds/unicom-iptv@main/unicom.txt` | `https://gh-proxy.com/https://raw.githubusercontent.com/saodisengyyds/unicom-iptv/main/unicom.txt` | `https://raw.githubusercontent.com/saodisengyyds/unicom-iptv/main/unicom.txt` |

---

## 💡 使用说明

1. **网络要求**：必须在**联通宽带**（连接家里联通 Wi-Fi）环境下播放，不可跨运营商或使用手机移动数据；
2. **零硬件配置**：属于标准 HTTP 单播流，无需开启路由器的 IGMP Snooping 或 udpxy 组播代理；
3. **EPG 电子节目单**：已内嵌自动节目单配置，主流播放器导入后可直接显示当前节目与节目预告；
4. **推荐播放器**：
   - **电视端 / 电视盒子**：TiviMate、影视仓、DIYP 影音、百川影音、Kodi
   - **手机 / 平板端**：MX Player（Android）、APTV（iOS/tvOS）

---

## 🔗 原始数据源

- **接口地址**：`http://shanxiunicom.livehot.wasu.tv/weekhot_cs2/interfaces/liveChannel.do`
  *(仅限联通宽带内网设备访问，用于后续提取最新频道数据备份)*
