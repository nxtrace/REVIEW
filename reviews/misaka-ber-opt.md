---
layout: default
title: Misaka.BER.Opt
seo_keywords: "Misaka 柏林,Misaka 德国, 德国VPS, CN2, BER, EPYC"
redirect_from:
  - /reviews/misaka-ber-opt.md
  - /REVIEW/reviews/misaka-ber-opt.md
---

# Misaka.BER.Opt

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

- [**官方购买入口**](https://app.misaka.io/iaas/vm/create/ber03/s3c-1c512m)

### 规格对照

<details markdown="1">
<summary>Standard NVMe (Gen3, AMD EPYC)</summary>

| 套餐 | vCPU | 内存 | 本地 NVMe SSD | 流量（单向 In+Out） | 月付 |
|---|---:|---:|---:|---:|---:|
| S3N-1C1G | 1 | 1 GiB | 16 GiB | 1 TiB | $6 |
| S3N-1C2G | 1 | 2 GiB | 32 GiB | 2 TiB | $10 |
| S3N-2C3G | 2 | 3 GiB | 48 GiB | 3 TiB | $15 |
| S3N-2C4G | 2 | 4 GiB | 64 GiB | 4 TiB | $20 |
| S3N-4C6G | 4 | 6 GiB | 96 GiB | 6 TiB | $30 |
| S3N-4C8G | 4 | 8 GiB | 112 GiB | 8 TiB | $40 |
| S3N-6C12G | 6 | 12 GiB | 128 GiB | 12 TiB | $60 |
| S3N-8C16G | 8 | 16 GiB | 144 GiB | 16 TiB | $80 |
| S3N-8C24G | 8 | 24 GiB | 160 GiB | 24 TiB | $120 |
| S3N-16C32G | 16 | 32 GiB | 240 GiB | 32 TiB | $160 |

</details>

<details markdown="1">
<summary>Standard NVMe w/ CN2 (Gen3, AMD EPYC)</summary>

| 套餐 | vCPU | 内存 | 本地 NVMe SSD | 流量（单向 In+Out） | 月付 |
|---|---:|---:|---:|---:|---:|
| S3C-1C512M | 1 | 512 MiB | 10 GiB | 512 GiB | $10.5 |
| S3C-1C1G | 1 | 1 GiB | 16 GiB | 1 TiB | $15 |
| S3C-1C2G | 1 | 2 GiB | 32 GiB | 2 TiB | $30 |
| S3C-2C3G | 2 | 3 GiB | 48 GiB | 3 TiB | $45 |
| S3C-2C4G | 2 | 4 GiB | 64 GiB | 4 TiB | $60 |
| S3C-4C6G | 4 | 6 GiB | 96 GiB | 6 TiB | $90 |
| S3C-4C8G | 4 | 8 GiB | 112 GiB | 8 TiB | $120 |
| S3C-6C12G | 6 | 12 GiB | 128 GiB | 12 TiB | $180 |
| S3C-8C16G | 8 | 16 GiB | 144 GiB | 16 TiB | $240 |
| S3C-8C24G | 8 | 24 GiB | 160 GiB | 24 TiB | $360 |
| S3C-16C32G | 16 | 32 GiB | 240 GiB | 32 TiB | $480 |

</details>

> 说明：规格表仅供对照，库存状态以 Misaka 控制台为准。

## 评

三网回程莫斯科 CN2 GIA（商家的L2从莫斯科拉到柏林），对于电信用户延迟最低的西欧机器了，相比友商法兰克福/伦敦的CN2小鸡无论是延迟还是稳定性都好很多，因此本站强烈推荐预算较为充裕的需要欧洲方向线路的电信用户考虑这款产品。但是联通/移动宽带用户就需要关注所在地区跨网拥堵情况了。商家信誉及机器性能/稳定性也都很好，国际方向接了RETN、1299、Lumen、DTAG，该有的都有了。  
**电信用户速度可比较稳定**的跑到 700Mbps 以上  
**移动联通用户慎重选择 ** 

三网 CN2 GIA 回程  
电信 CN2 GIA 去程  
联通 Lumen 去程  
移动 RETN 去程

## 测

### 路由表现

<details markdown="1">
<summary>线路概览</summary>

**IPv4 路由图**
![ipv4-radar]({{ '/assets/images/misaka-ber-opt/4-radar.png' | relative_url }})

**IPv6 路由图**
![ipv6-radar]({{ '/assets/images/misaka-ber-opt/6-radar.png' | relative_url }})

</details>

<details markdown="1">
<summary>IPv4 去程</summary>

<div align="center">
  <img src="{{ '/assets/images/misaka-ber-opt/IPv4去程/2025-12-17 11.02.19.png' | relative_url }}" alt="IPv4 去程路由 1" width="32%" />
  <img src="{{ '/assets/images/misaka-ber-opt/IPv4去程/2025-12-17 11.02.34.png' | relative_url }}" alt="IPv4 去程路由 2" width="32%" />
  <img src="{{ '/assets/images/misaka-ber-opt/IPv4去程/2025-12-17 11.02.58.png' | relative_url }}" alt="IPv4 去程路由 3" width="32%" />
</div>

</details>

<details markdown="1">
<summary>IPv4 回程 · ICMP</summary>

<div align="center">
  <img src="{{ '/assets/images/misaka-ber-opt/IPv4 回程 · ICMP/截屏2025-12-17 上午10.43.33.png' | relative_url }}" alt="IPv4 回程 ICMP 1" width="32%" />
  <img src="{{ '/assets/images/misaka-ber-opt/IPv4 回程 · ICMP/截屏2025-12-17 上午10.46.53.png' | relative_url }}" alt="IPv4 回程 ICMP 2" width="32%" />
  <img src="{{ '/assets/images/misaka-ber-opt/IPv4 回程 · ICMP/截屏2025-12-17 上午10.47.01.png' | relative_url }}" alt="IPv4 回程 ICMP 3" width="32%" />
</div>

</details>

<details markdown="1">
<summary>IPv4 回程 · TCP</summary>

<div align="center">
  <img src="{{ '/assets/images/misaka-ber-opt/IPv4 回程 · TCP/截屏2025-12-17 上午10.47.43.png' | relative_url }}" alt="IPv4 回程 TCP 1" width="32%" />
  <img src="{{ '/assets/images/misaka-ber-opt/IPv4 回程 · TCP/截屏2025-12-17 上午10.47.52.png' | relative_url }}" alt="IPv4 回程 TCP 2" width="32%" />
  <img src="{{ '/assets/images/misaka-ber-opt/IPv4 回程 · TCP/截屏2025-12-17 上午10.49.20.png' | relative_url }}" alt="IPv4 回程 TCP 3" width="32%" />
</div>

</details>

### 实时监控
- **实时三网 ICMP**：<https://ping.nxtrace.org/goto/HEhVjEINg>
- **实时三网 TCP**：<https://ping.nxtrace.org/goto/CGCVjPSHg>
- **官方 Looking Glass**：<https://ping.sx/mtr?p=230>
- **北京三网延迟监控截图**：
  <details markdown="1">
  <summary>展开查看</summary>
  
  ![北京三网延迟监控截图]({{ '/assets/images/misaka-ber-opt/北京三网延迟监控截图（近七天）.png' | relative_url }})
  
  </details>

### 北京四网代理单线程测速

<details markdown="1">
<summary>北京移动晚高峰</summary>

![北京移动晚高峰]({{ '/assets/images/misaka-ber-opt/北京四网代理单线程测速/北京移动晚高峰.jpg' | relative_url }})

</details>

<details markdown="1">
<summary>北京移动白天</summary>

![北京移动白天]({{ '/assets/images/misaka-ber-opt/北京四网代理单线程测速/北京移动白天.jpg' | relative_url }})

</details>

<details markdown="1">
<summary>北京联通晚高峰</summary>

![北京联通晚高峰]({{ '/assets/images/misaka-ber-opt/北京四网代理单线程测速/北京联通晚高峰.jpg' | relative_url }})

</details>

<details markdown="1">
<summary>北京联通白天</summary>

![北京联通白天]({{ '/assets/images/misaka-ber-opt/北京四网代理单线程测速/北京联通白天.jpg' | relative_url }})

</details>

<details markdown="1">
<summary>北京网通晚高峰</summary>

![北京网通晚高峰]({{ '/assets/images/misaka-ber-opt/北京四网代理单线程测速/北京网通晚高峰.jpg' | relative_url }})

</details>

<details markdown="1">
<summary>北京网通白天</summary>

![北京网通白天]({{ '/assets/images/misaka-ber-opt/北京四网代理单线程测速/北京网通白天.jpg' | relative_url }})

</details>

<details markdown="1">
<summary>北京电信晚高峰</summary>

![北京电信晚高峰]({{ '/assets/images/misaka-ber-opt/北京四网代理单线程测速/北京电信晚高峰.jpg' | relative_url }})

</details>

<details markdown="1">
<summary>北京电信白天</summary>

![北京电信白天]({{ '/assets/images/misaka-ber-opt/北京四网代理单线程测速/北京电信白天.jpg' | relative_url }})

</details>

### 机器性能跑分

<details markdown="1">
<summary>综合性能跑分（YABS·GB5）</summary>

![综合性能跑分]({{ '/assets/images/misaka-ber-opt/综合性能跑分.png' | relative_url }})

</details>

### IP 解锁

<details markdown="1">
<summary>流媒体 / 平台解锁记录</summary>

![解锁情况 1]({{ '/assets/images/misaka-ber-opt/解锁情况/2025-12-17 10.30.59.png' | relative_url }})
![解锁情况 2]({{ '/assets/images/misaka-ber-opt/解锁情况/2025-12-17 10.31.00.png' | relative_url }})

</details>
