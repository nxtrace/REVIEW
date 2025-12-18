---
layout: default
title: "🇯🇵 V.PS Performance Tokyo Gen2 日本东京 CN2/9929 VPS 测评"
seo_keywords: "V.PS Tokyo Performance KVM VPS Gen 2, V.PS Tokyo EPYC Gen 2 Explorer, xtom, sa.net, Riven Cloud, GreenCloud, 绿云, CN2, 9929, 东京VPS, 日本VPS, EPYC, JP"
redirect_from:
  - /reviews/xtom-tokyo-epyc-gen2.md
  - /REVIEW/reviews/xtom-tokyo-epyc-gen2.md
---

# 🇯🇵 V.PS Performance Tokyo Gen2 日本东京 CN2/9929 VPS 测评

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

### 购买信息

- [**官方购买入口**](https://vps.hosting/?affid=2152&oid=36)

### 规格对照

<details markdown="1">
<summary>xTom Tokyo Gen 2 (Performance KVM VPS)</summary>

| 套餐 | vCPU | 内存 | NVMe | 流量（单向 In+Out） | 端口 | 月付 |
|---|---:|---:|---:|---:|---:|---:|
| Tokyo EPYC Flash Gen 2 | 2 Cores | 4 GB | 30 GB | 1 TB | 1 Gbps | €47.95 |
| Tokyo EPYC Flow Gen 2 | 2 Cores | 8 GB | 60 GB | 2 TB | 1.25 Gbps | €95.95 |
| Tokyo EPYC Fleet Gen 2 | 4 Cores | 16 GB | 120 GB | 4 TB | 2 Gbps | €191.95 |
| Tokyo EPYC Formula Gen 2 | 8 Cores | 32 GB | 240 GB | 8 TB | 2.5 Gbps | €383.95 |

</details>

## 评

算是靠谱的商家里少数卖同时带9929和CN2线路的日本小鸡了，东西确实贵，但也确实值这个价，商家也没有什么线路掺水的黑历史，富哥可以考虑一下  
**电信联通用户速度还是比较稳定**的跑到 700Mbps 以上  
**移动用户慎重选择**  

电信 / 移动 CTG GIA(aka CN2 GIA) 回程  
联通 CUG VIP(aka 9929) 回程  
电信 CTG GIA 去程  
联通 CUG VIP 去程  
移动 CMI 去程  
另 IPv6 有三网优化但是就电信方向能用（163）  

## 测

### 路由表现

<details markdown="1">
<summary>线路概览</summary>

**IPv4 路由图**
![ipv4-radar]({{ '/assets/images/xtom-tokyo-epyc-gen2/4-radar.png' | relative_url }})

**IPv6 路由图**
![ipv6-radar]({{ '/assets/images/xtom-tokyo-epyc-gen2/6-radar.png' | relative_url }})

</details>

<details markdown="1">
<summary>IPv4 去程</summary>

<div align="center">
  <img src="{{ '/assets/images/xtom-tokyo-epyc-gen2/IPv4去程/IMAGE 2025-12-14 16:03:14.jpg' | relative_url }}" alt="IPv4 去程路由 1" width="32%" />
  <img src="{{ '/assets/images/xtom-tokyo-epyc-gen2/IPv4去程/IMAGE 2025-12-14 16:03:18.jpg' | relative_url }}" alt="IPv4 去程路由 2" width="32%" />
  <img src="{{ '/assets/images/xtom-tokyo-epyc-gen2/IPv4去程/IMAGE 2025-12-14 16:03:20.jpg' | relative_url }}" alt="IPv4 去程路由 3" width="32%" />
</div>

</details>

<details markdown="1">
<summary>IPv4 回程 · ICMP</summary>

<div align="center">
  <img src="{{ '/assets/images/xtom-tokyo-epyc-gen2/IPv4 回程 · ICMP/IMAGE 2025-12-14 16:03:46.jpg' | relative_url }}" alt="IPv4 回程 ICMP 1" width="32%" />
  <img src="{{ '/assets/images/xtom-tokyo-epyc-gen2/IPv4 回程 · ICMP/IMAGE 2025-12-14 16:03:48.jpg' | relative_url }}" alt="IPv4 回程 ICMP 2" width="32%" />
  <img src="{{ '/assets/images/xtom-tokyo-epyc-gen2/IPv4 回程 · ICMP/IMAGE 2025-12-14 16:03:49.jpg' | relative_url }}" alt="IPv4 回程 ICMP 3" width="32%" />
</div>

</details>

<details markdown="1">
<summary>IPv4 回程 · TCP</summary>

<div align="center">
  <img src="{{ '/assets/images/xtom-tokyo-epyc-gen2/IPv4 回程 · TCP/IMAGE 2025-12-14 16:03:38.jpg' | relative_url }}" alt="IPv4 回程 TCP 1" width="32%" />
  <img src="{{ '/assets/images/xtom-tokyo-epyc-gen2/IPv4 回程 · TCP/IMAGE 2025-12-14 16:03:39.jpg' | relative_url }}" alt="IPv4 回程 TCP 2" width="32%" />
  <img src="{{ '/assets/images/xtom-tokyo-epyc-gen2/IPv4 回程 · TCP/IMAGE 2025-12-14 16:03:40.jpg' | relative_url }}" alt="IPv4 回程 TCP 3" width="32%" />
</div>

</details>

<details markdown="1">
<summary>IPv6 去程</summary>

<div align="center">
  <img src="{{ '/assets/images/xtom-tokyo-epyc-gen2/IPv6去程/IMAGE 2025-12-14 16:15:39.jpg' | relative_url }}" alt="IPv6 去程路由 1" width="32%" />
  <img src="{{ '/assets/images/xtom-tokyo-epyc-gen2/IPv6去程/IMAGE 2025-12-14 16:15:40.jpg' | relative_url }}" alt="IPv6 去程路由 2" width="32%" />
  <img src="{{ '/assets/images/xtom-tokyo-epyc-gen2/IPv6去程/IMAGE 2025-12-14 16:15:41.jpg' | relative_url }}" alt="IPv6 去程路由 3" width="32%" />
</div>

</details>

<details markdown="1">
<summary>IPv6 回程 · ICMP</summary>

<div align="center">
  <img src="{{ '/assets/images/xtom-tokyo-epyc-gen2/IPv6 回程 · ICMP/IMAGE 2025-12-14 16:16:11.jpg' | relative_url }}" alt="IPv6 回程 ICMP 1" width="32%" />
  <img src="{{ '/assets/images/xtom-tokyo-epyc-gen2/IPv6 回程 · ICMP/IMAGE 2025-12-14 16:16:12.jpg' | relative_url }}" alt="IPv6 回程 ICMP 2" width="32%" />
  <img src="{{ '/assets/images/xtom-tokyo-epyc-gen2/IPv6 回程 · ICMP/IMAGE 2025-12-14 16:16:14.jpg' | relative_url }}" alt="IPv6 回程 ICMP 3" width="32%" />
</div>

</details>

<details markdown="1">
<summary>IPv6 回程 · TCP</summary>

<div align="center">
  <img src="{{ '/assets/images/xtom-tokyo-epyc-gen2/IPv6 回程 · TCP/IMAGE 2025-12-14 16:15:56.jpg' | relative_url }}" alt="IPv6 回程 TCP 1" width="32%" />
  <img src="{{ '/assets/images/xtom-tokyo-epyc-gen2/IPv6 回程 · TCP/IMAGE 2025-12-14 16:15:58.jpg' | relative_url }}" alt="IPv6 回程 TCP 2" width="32%" />
  <img src="{{ '/assets/images/xtom-tokyo-epyc-gen2/IPv6 回程 · TCP/IMAGE 2025-12-14 16:15:59.jpg' | relative_url }}" alt="IPv6 回程 TCP 3" width="32%" />
</div>

</details>

### 实时监控
- **实时三网 ICMP**：<https://ping.nxtrace.org/goto/WJYlkcMvR>
- **实时三网 TCP**：<https://ping.nxtrace.org/goto/tX7uk5MDg>
- **北京三网延迟监控截图**：
  <details markdown="1">
  <summary>展开查看</summary>
  
  ![北京三网延迟监控截图]({{ '/assets/images/xtom-tokyo-epyc-gen2/北京三网延迟监控截图.png' | relative_url }})
  
  </details>

### 北京四网代理单线程测速

<details markdown="1">
<summary>北京移动晚高峰</summary>

![北京移动晚高峰]({{ '/assets/images/xtom-tokyo-epyc-gen2/北京四网代理单线程测速/北京移动晚高峰.jpg' | relative_url }})

</details>

<details markdown="1">
<summary>北京移动白天</summary>

![北京移动白天]({{ '/assets/images/xtom-tokyo-epyc-gen2/北京四网代理单线程测速/北京移动白天.jpg' | relative_url }})

</details>

<details markdown="1">
<summary>北京联通晚高峰</summary>

![北京联通晚高峰]({{ '/assets/images/xtom-tokyo-epyc-gen2/北京四网代理单线程测速/北京联通晚高峰.jpg' | relative_url }})

</details>

<details markdown="1">
<summary>北京联通白天</summary>

![北京联通白天]({{ '/assets/images/xtom-tokyo-epyc-gen2/北京四网代理单线程测速/北京联通白天.jpg' | relative_url }})

</details>

<details markdown="1">
<summary>北京网通晚高峰</summary>

![北京网通晚高峰]({{ '/assets/images/xtom-tokyo-epyc-gen2/北京四网代理单线程测速/北京网通晚高峰.jpg' | relative_url }})

</details>

<details markdown="1">
<summary>北京网通白天</summary>

![北京网通白天]({{ '/assets/images/xtom-tokyo-epyc-gen2/北京四网代理单线程测速/北京网通白天.jpg' | relative_url }})

</details>

<details markdown="1">
<summary>北京电信晚高峰</summary>

![北京电信晚高峰]({{ '/assets/images/xtom-tokyo-epyc-gen2/北京四网代理单线程测速/北京电信晚高峰.jpg' | relative_url }})

</details>

<details markdown="1">
<summary>北京电信白天</summary>

![北京电信白天]({{ '/assets/images/xtom-tokyo-epyc-gen2/北京四网代理单线程测速/北京电信白天.jpg' | relative_url }})

</details>

### 机器性能跑分

<details markdown="1">
<summary>综合性能跑分</summary>

![综合性能跑分]({{ '/assets/images/xtom-tokyo-epyc-gen2/综合性能跑分.jpg' | relative_url }})

</details>

### IP 解锁

<details markdown="1">
<summary>流媒体 / 平台解锁记录</summary>

![解锁情况 1]({{ '/assets/images/xtom-tokyo-epyc-gen2/解锁情况/IMAGE 2025-12-14 16:05:42.jpg' | relative_url }})
![解锁情况 2]({{ '/assets/images/xtom-tokyo-epyc-gen2/解锁情况/IMAGE 2025-12-14 16:05:44.jpg' | relative_url }})

</details>

## 提示

由于 V.PS 短期内不会补货，可考虑其下游（RivenCloud / GreenCloud）：
- GreenCloud 500G@500Mbps=25USD/mo：<https://greencloudvps.com/billing/store/cn-premium-optimized>
- RivenCloud 1T@1Gbps=49USD/mo：<https://portal.sa.net/store/cloud-server>
