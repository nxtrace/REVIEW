---
layout: default
title: "🇺🇸 DMIT.LAX.T1 美国洛杉矶 高性能 VPS 测评"
seo_keywords: "DMIT 洛杉矶, DMIT 美国, 洛杉矶VPS, 美国VPS, EPYC, US, Genoa, Turin, Zen5"
redirect_from:
  - /reviews/dmit-lax-t1.md
  - /REVIEW/reviews/dmit-lax-t1.md
---

# 🇺🇸 DMIT.LAX.T1 美国洛杉矶 高性能 VPS 测评

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

- [**官方购买入口**](https://www.dmit.io/cart.php?region=los-angeles&generation=an5&network=tier-1&aff=3487)

### 规格对照

> 该系列流量均为单向计费  
硬件有 AS3 / AN5 两档，性能差异较大（见下方跑分）。

<details>
<summary>AS3 系列（CPU：AMD EPYC 7003）</summary>

<div class="spec-table" markdown="1">

| 套餐 | CPU | vCPU | 内存 | SSD | 高速区流量额度 | 高速端口 | 超额后不限流量限速 | 月付价格 |
|---|---|---:|---:|---:|---:|---:|---:|---:|
| WEE | EPYC 7003 | 1 | 1GB | 20GB | 1TB | 4Gbps | 100Mbps | $3.08 |
| TINY | EPYC 7003 | 1 | 1GB | 20GB | 2TB | 4Gbps | 200Mbps | $6.90 |
| STARTER | EPYC 7003 | 2 | 2GB | 40GB | 4TB | 10Gbps | 200Mbps | $12.90 |
| MINI | EPYC 7003 | 2 | 4GB | 80GB | 8TB | 10Gbps | 200Mbps | $21.90 |
| MICRO | EPYC 7003 | 4 | 4GB | 120GB | 16TB | 10Gbps | 500Mbps | $32.90 |

</div>

</details>

<details>
<summary>AN5 · VOLUME 系列（流量额度多，CPU：AMD EPYC 9005）</summary>

<div class="spec-table" markdown="1">

| 型号 | CPU | vCPU | 内存 | SSD | 高速区流量额度 | 高速端口 | 超额后不限流量限速 | 月付价格 |
|---|---|---:|---:|---:|---:|---:|---:|---:|
| V2C2G | EPYC 9005 | 2 | 2GB | 40GB | 5TB | 10Gbps | 100Mbps | $14.90 |
| V2C4G | EPYC 9005 | 2 | 4GB | 80GB | 10TB | 10Gbps | 200Mbps | $23.90 |
| V4C4G | EPYC 9005 | 4 | 4GB | 120GB | 20TB | 10Gbps | 200Mbps | $36.90 |
| V4C8G | EPYC 9005 | 4 | 8GB | 160GB | 40TB | 10Gbps | 500Mbps | $52.90 |
| V8C16G | EPYC 9005 | 8 | 16GB | 240GB | 80TB | 10Gbps | 500Mbps | $119.90 |
| V12C24G | EPYC 9005 | 12 | 24GB | 320GB | 160TB | 10Gbps | 500Mbps | $199.90 |

</div>

</details>

<details>
<summary>AN5 · GENERAL 系列（硬件规格高，CPU：AMD EPYC 9005）</summary>

<div class="spec-table" markdown="1">

| 型号 | CPU | vCPU | 内存 | SSD | 高速区流量额度 | 高速端口 | 超额后不限流量限速 | 月付价格 |
|---|---|---:|---:|---:|---:|---:|---:|---:|
| G2C4G | EPYC 9005 | 2 | 4GB | 80GB | 4TB | 10Gbps | 100Mbps | $16.90 |
| G4C8G | EPYC 9005 | 4 | 8GB | 160GB | 8TB | 10Gbps | 100Mbps | $36.90 |
| G8C16G | EPYC 9005 | 8 | 16GB | 320GB | 12TB | 10Gbps | 200Mbps | $79.90 |
| G12C24G | EPYC 9005 | 12 | 24GB | 480GB | 24TB | 10Gbps | 200Mbps | $119.90 |
| G16C32G | EPYC 9005 | 16 | 32GB | 640GB | 32TB | 10Gbps | 200Mbps | $199.90 |

</div>

</details>

## 评

DMIT 高性能建站/落地小鸡，性能/稳定性/国际互联优异，大带宽，接入 GSL/GTT/1299 线路。  
无中国路由优化，如需中国访问建议搭配精品线路机器使用。  

## 测

### 路由表现

<details markdown="1">
<summary>线路概览</summary>

**IPv4 路由图**
![ipv4-radar]({{ '/assets/images/dmit-lax-t1/4-radar.png' | relative_url }})

**IPv6 路由图**
![ipv6-radar]({{ '/assets/images/dmit-lax-t1/6-radar.png' | relative_url }})

</details>

### 实时监控
- **官方 Looking Glass**：<https://lg.dmit.sh/?server=lax-t1>

### CDN 测速

<details markdown="1">
<summary>Apple CDN</summary>

![Apple CDN 测速]({{ '/assets/images/dmit-lax-t1/CDN测速/2026-05-08 20.55.14.png' | relative_url }})

</details>

<details markdown="1">
<summary>Cloudflare CDN</summary>

![Cloudflare CDN 测速]({{ '/assets/images/dmit-lax-t1/CDN测速/2026-05-08 20.55.15.png' | relative_url }})

</details>

### 机器性能跑分

<details markdown="1">
<summary>AS3 综合性能跑分（YABS·GB6）</summary>

![综合性能跑分·AS3]({{ '/assets/images/dmit-lax-t1/综合性能跑分·AS3.png' | relative_url }})

</details>

<details markdown="1">
<summary>AN4 综合性能跑分（YABS·GB6）</summary>

![综合性能跑分·AN4]({{ '/assets/images/dmit-lax-t1/综合性能跑分·AN4.png' | relative_url }})

</details>

<details markdown="1">
<summary>AN5 综合性能跑分（YABS·GB6）</summary>

![综合性能跑分·AN5]({{ '/assets/images/dmit-lax-t1/综合性能跑分·AN5.jpg' | relative_url }})

</details>

### IP 解锁

<details markdown="1">
<summary>流媒体 / 平台解锁记录</summary>

![解锁情况 1]({{ '/assets/images/dmit-lax-t1/解锁情况/2025-12-21 13.45.03.png' | relative_url }})
![解锁情况 2]({{ '/assets/images/dmit-lax-t1/解锁情况/2025-12-21 13.45.18.png' | relative_url }})

</details>
