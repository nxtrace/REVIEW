---
layout: default
title: "🇳🇱 咸鱼云 Saltyfish Amsterdam Premium 荷兰阿姆斯特丹 CN2 GIA VPS 测评"
seo_keywords: "阿姆斯特丹VPS, AMS, 咸鱼云, Saltyfish, CN2 GIA, CTG GIA, CMIN2, 9929, snapstack, 荷兰VPS"
redirect_from:
  - /reviews/saltyfish-ams-pro.md
  - /REVIEW/reviews/saltyfish-ams-pro.md
---

# 🇳🇱 咸鱼云 Saltyfish Amsterdam Premium 荷兰阿姆斯特丹 CN2 GIA VPS 测评

<div class="back-home" style="margin: 12px 0 24px;">
  <a href="{{ '/' | relative_url }}" style="display: inline-flex; align-items: center; gap: 8px; padding: 8px 12px; background: linear-gradient(135deg, #f8fafc 0%, #eef2f7 100%); border: 1px solid #e5e7eb; border-radius: 999px; color: #1f2937; text-decoration: none; font-size: 14px; font-weight: 600;">
    <span style="font-size: 16px;">←</span>
    <span>返回主页</span>
  </a>
</div>

<div class="toc-container" markdown="1">

## 目录
{: .no_toc }

* TOC
{:toc}

</div>

## 买

### 购买链接

- [**官方购买入口**](https://portal.saltyfish.io/aff.php?aff=610&gid=22)

### 规格对照

> China Mainland Optimized by China Telecom CN2 GIA.

<details markdown="1">
<summary>Amsterdam VPS - Premium Network</summary>

| 套餐 | vCPU | 内存 | SSD | 流量 | 端口 | 价格 |
|---|---:|---:|---:|---:|---:|---:|
| ams.p1.mini | 1 | 1 GB | 10 GB | 1000 GB | 2.5 Gbps | ¥121.80 / 季 |
| ams.p1.micro | 1 | 2 GB | 15 GB | 2000 GB | 2.5 Gbps | ¥82.60 / 月 |
| ams.p1.medium | 2 | 4 GB | 30 GB | 4000 GB | 2.5 Gbps | ¥165.20 / 月 |

</details>

## 评

咸鱼云荷兰阿姆斯特丹 CN2 GIA+CMIN2 小鸡，线路优秀。  
中国优化路由是从他家法兰克福拉过来的，所以延迟表现会稍差于他家FRA.Pro机型（延迟大约高10ms），国际方向是本地直接出的，  
速度和FRA.Pro一致，三网晚高峰都可以跑到600Mbps以上。  
考虑到他家AMS.Pro价格相对于的便宜一些，不太在意极致延迟的话可以选择。  

电信 CTG GIA (aka: CN2 GIA）回程 / CTG GIA 去程  
联通 CTG GIA 回程 / CUG VIP (aka: 9929) 去程  
移动 CMIN2 回程 / CMIN2 去程  

## 测

### 路由表现

<details markdown="1">
<summary>线路概览</summary>

**IPv4 路由图**
![ipv4-radar]({{ '/assets/images/saltyfish-ams-pro/radar.png' | relative_url }})

</details>

<details markdown="1">
<summary>IPv4 去程</summary>

<div align="center">
  <img src="{{ '/assets/images/saltyfish-ams-pro/IPv4去程/2025-12-25 21.03.21.png' | relative_url }}" alt="IPv4 去程路由 1" width="32%" />
  <img src="{{ '/assets/images/saltyfish-ams-pro/IPv4去程/2025-12-25 21.03.23.png' | relative_url }}" alt="IPv4 去程路由 2" width="32%" />
  <img src="{{ '/assets/images/saltyfish-ams-pro/IPv4去程/2025-12-25 21.03.24.png' | relative_url }}" alt="IPv4 去程路由 3" width="32%" />
</div>

</details>

<details markdown="1">
<summary>IPv4 回程 · ICMP</summary>

<div align="center">
  <img src="{{ '/assets/images/saltyfish-ams-pro/IPv4 回程 · ICMP/2025-12-25 20.58.18.png' | relative_url }}" alt="IPv4 回程 ICMP 1" width="32%" />
  <img src="{{ '/assets/images/saltyfish-ams-pro/IPv4 回程 · ICMP/2025-12-25 20.58.19.png' | relative_url }}" alt="IPv4 回程 ICMP 2" width="32%" />
  <img src="{{ '/assets/images/saltyfish-ams-pro/IPv4 回程 · ICMP/2025-12-25 20.58.21.png' | relative_url }}" alt="IPv4 回程 ICMP 3" width="32%" />
</div>

</details>

<details markdown="1">
<summary>IPv4 回程 · TCP</summary>

<div align="center">
  <img src="{{ '/assets/images/saltyfish-ams-pro/IPv4 回程 · TCP/2025-12-25 21.00.27.png' | relative_url }}" alt="IPv4 回程 TCP 1" width="32%" />
  <img src="{{ '/assets/images/saltyfish-ams-pro/IPv4 回程 · TCP/2025-12-25 21.00.29.png' | relative_url }}" alt="IPv4 回程 TCP 2" width="32%" />
  <img src="{{ '/assets/images/saltyfish-ams-pro/IPv4 回程 · TCP/2025-12-25 21.00.30.png' | relative_url }}" alt="IPv4 回程 TCP 3" width="32%" />
</div>

</details>

### 实时监控
- **实时三网 ICMP**：<https://ping.nxtrace.org/goto/ZMX6at7DR>
- **实时三网 TCP**：<https://ping.nxtrace.org/goto/ZSTRBt7DR>
- **官方 Looking Glass**：<https://lg.saltyfish.io/?router=ams-premium>
- **北京三网延迟监控截图**：
  <details markdown="1">
  <summary>展开查看</summary>
  
  ![北京三网延迟监控截图]({{ '/assets/images/saltyfish-ams-pro/北京三网延迟监控截图.png' | relative_url }})
  
  </details>

### ITDOG 多地延迟测试

<details markdown="1">
<summary>展开查看</summary>

**白天**
![ITDOG 多地延迟测试 · 白天]({{ '/assets/images/saltyfish-ams-pro/多地Ping值测试/Saltyfish.AMS.Pro_多地Ping值测试_白天.png' | relative_url }})

**晚高峰**
![ITDOG 多地延迟测试 · 晚高峰]({{ '/assets/images/saltyfish-ams-pro/多地Ping值测试/Saltyfish.AMS.Pro 多地Ping值测试_晚高峰.png' | relative_url }})

</details>

### 北京四网代理单线程测速

<details markdown="1">
<summary>北京移动晚高峰</summary>

![北京移动晚高峰]({{ '/assets/images/saltyfish-ams-pro/北京四网代理单线程测速/北京移动晚高峰.jpg' | relative_url }})

</details>

<details markdown="1">
<summary>北京移动白天</summary>

![北京移动白天]({{ '/assets/images/saltyfish-ams-pro/北京四网代理单线程测速/北京移动白天.jpg' | relative_url }})

</details>

<details markdown="1">
<summary>北京联通晚高峰</summary>

![北京联通晚高峰]({{ '/assets/images/saltyfish-ams-pro/北京四网代理单线程测速/北京联通晚高峰.jpg' | relative_url }})

</details>

<details markdown="1">
<summary>北京联通白天</summary>

![北京联通白天]({{ '/assets/images/saltyfish-ams-pro/北京四网代理单线程测速/北京联通白天.jpg' | relative_url }})

</details>

<details markdown="1">
<summary>北京网通晚高峰</summary>

![北京网通晚高峰]({{ '/assets/images/saltyfish-ams-pro/北京四网代理单线程测速/北京网通晚高峰.jpg' | relative_url }})

</details>

<details markdown="1">
<summary>北京网通白天</summary>

![北京网通白天]({{ '/assets/images/saltyfish-ams-pro/北京四网代理单线程测速/北京网通白天.jpg' | relative_url }})

</details>

<details markdown="1">
<summary>北京电信晚高峰</summary>

![北京电信晚高峰]({{ '/assets/images/saltyfish-ams-pro/北京四网代理单线程测速/北京电信晚高峰.jpg' | relative_url }})

</details>

<details markdown="1">
<summary>北京电信白天</summary>

![北京电信白天]({{ '/assets/images/saltyfish-ams-pro/北京四网代理单线程测速/北京电信白天.jpg' | relative_url }})

</details>

### CDN 测速

<details markdown="1">
<summary>Apple CDN</summary>

![Apple CDN 测速]({{ '/assets/images/saltyfish-ams-pro/CDN测速/截屏2026-05-08 下午2.53.46.png' | relative_url }})

</details>

<details markdown="1">
<summary>Cloudflare CDN</summary>

![Cloudflare CDN 测速]({{ '/assets/images/saltyfish-ams-pro/CDN测速/截屏2026-05-08 下午2.53.58.png' | relative_url }})

</details>

### 机器性能跑分

<details markdown="1">
<summary>综合性能跑分（YABS·GB4）</summary>

![综合性能跑分]({{ '/assets/images/saltyfish-ams-pro/综合性能跑分.png' | relative_url }})

</details>

### IP 解锁

<details markdown="1">
<summary>流媒体 / 平台解锁记录</summary>

![解锁情况]({{ '/assets/images/saltyfish-ams-pro/解锁情况/2025-12-25 20.52.00.png' | relative_url }})

</details>
