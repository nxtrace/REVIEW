---
layout: default
title: "GlobalTrace 全球路由追踪工具"
description: "GlobalTrace 是一个基于 Globalping probes 和 NextTrace 数据库的网页路由追踪工具，可从全球观察点发起 trace。"
seo_keywords: "GlobalTrace, NextTrace, Globalping, 路由追踪, traceroute, VPS测评, CDN, Anycast, ASN"
permalink: /globaltrace/
---

# GlobalTrace 全球路由追踪工具

GlobalTrace 是 NextTrace 官方做的网页路由追踪工具，不是 App，也不用安装客户端，浏览器打开就能用。

<div style="display: flex; flex-wrap: wrap; gap: 10px; margin: 16px 0 24px;">
  <a href="https://lg.nxtrace.org/" style="display: inline-flex; align-items: center; padding: 10px 14px; background: #159957; border-radius: 6px; color: #ffffff; text-decoration: none; font-weight: 700;">打开 GlobalTrace</a>
  <a href="https://github.com/nxtrace/GlobalTrace" style="display: inline-flex; align-items: center; padding: 10px 14px; border: 1px solid #d0d7de; border-radius: 6px; color: #1f2937; text-decoration: none; font-weight: 700;">查看源码</a>
</div>

![GlobalTrace 首页]({{ '/assets/images/globaltrace/home.webp' | relative_url }})

平时看 VPS、CDN、Anycast 或跨境访问问题时，本机 nexttrace 只能看到自己当前位置出去的一条路，视角比较窄。GlobalTrace 把 Globalping 和 NextTrace 融合：用 Globalping 的全球 probes 发起 trace，再用 NextTrace 的数据库补 hop 的地理位置、ASN、运营商 / ISP 等信息。

## 能看什么

- 从不同国家、城市、ASN、network 选择 Globalping probe
- 支持 ICMP / TCP / UDP
- 支持 IPv4 / IPv6
- 可以按 tag、eyeball、datacenter 筛 probe
- 结果里能看每跳 IP / hostname、loss、avg / min / max、ASN、地区、owner / ISP
- 有 2D / 3D 地图，方便大概看路径走向
- 结果可以生成分享链接；本站不获取或保存大家的历史记录，通过 Globalping 的能力实现
- 如果有自己的 Globalping Token，也可以填进去获得更多测试额度；Token 本地保存，不上传服务器

![路由结果页]({{ '/assets/images/globaltrace/results.webp' | relative_url }})

## 适合哪些场景

- 看某台 VPS 从不同地区访问路径怎么样
- 看 CDN / Anycast 落点和线路差异
- 看某些 ASN 或城市到目标是不是绕路
- 排查跨境访问时，找多个观察点对比

## 限制

Globalping 本身有 credits / rate limit；部分 hop 没有可定位 GeoIP 也正常。它不是万能回程测试，只是 Globalping probe 到目标的路径视角。

项目 GPL-3.0 开源，前端是 React + MapLibre，后端跑在 Cloudflare Workers。如果有 bug 或者觉得哪里不好用，可以回帖或提 GitHub issue。

## 更多截图

<div align="center">
  <img src="{{ '/assets/images/globaltrace/route-3d.webp' | relative_url }}" alt="GlobalTrace 3D 路径视图" width="48%" />
  <img src="{{ '/assets/images/globaltrace/home-dark.webp' | relative_url }}" alt="GlobalTrace 暗色主题首页" width="48%" />
</div>

<div align="center">
  <img src="{{ '/assets/images/globaltrace/mobile-results.webp' | relative_url }}" alt="GlobalTrace 移动端结果页" width="32%" />
  <img src="{{ '/assets/images/globaltrace/mobile-3d.webp' | relative_url }}" alt="GlobalTrace 移动端 3D 视图" width="32%" />
</div>
