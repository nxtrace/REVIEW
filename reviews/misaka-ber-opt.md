---
layout: default
title: Misaka.BER.Opt
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

- [Misaka BER03 S3C-1C512M](https://app.misaka.io/iaas/vm/create/ber03/s3c-1c512m)

## 评

三网回程莫斯科 CN2 GIA。  
官方 Looking Glass：<https://ping.sx/mtr?p=230>

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

引用：<https://t.me/nanaselog/859>

<div align="center">
  <img src="{{ '/assets/images/misaka-ber-opt/IPv4去程/2025-12-17 11.02.19.png' | relative_url }}" alt="IPv4 去程路由 1" width="32%" />
  <img src="{{ '/assets/images/misaka-ber-opt/IPv4去程/2025-12-17 11.02.34.png' | relative_url }}" alt="IPv4 去程路由 2" width="32%" />
  <img src="{{ '/assets/images/misaka-ber-opt/IPv4去程/2025-12-17 11.02.58.png' | relative_url }}" alt="IPv4 去程路由 3" width="32%" />
</div>

</details>

<details markdown="1">
<summary>IPv4 回程 · ICMP</summary>

引用：<https://t.me/nanaselog/862>

<div align="center">
  <img src="{{ '/assets/images/misaka-ber-opt/IPv4 回程 · ICMP/截屏2025-12-17 上午10.43.33.png' | relative_url }}" alt="IPv4 回程 ICMP 1" width="32%" />
  <img src="{{ '/assets/images/misaka-ber-opt/IPv4 回程 · ICMP/截屏2025-12-17 上午10.46.53.png' | relative_url }}" alt="IPv4 回程 ICMP 2" width="32%" />
  <img src="{{ '/assets/images/misaka-ber-opt/IPv4 回程 · ICMP/截屏2025-12-17 上午10.47.01.png' | relative_url }}" alt="IPv4 回程 ICMP 3" width="32%" />
</div>

</details>

<details markdown="1">
<summary>IPv4 回程 · TCP</summary>

引用：<https://t.me/nanaselog/865>

<div align="center">
  <img src="{{ '/assets/images/misaka-ber-opt/IPv4 回程 · TCP/截屏2025-12-17 上午10.47.43.png' | relative_url }}" alt="IPv4 回程 TCP 1" width="32%" />
  <img src="{{ '/assets/images/misaka-ber-opt/IPv4 回程 · TCP/截屏2025-12-17 上午10.47.52.png' | relative_url }}" alt="IPv4 回程 TCP 2" width="32%" />
  <img src="{{ '/assets/images/misaka-ber-opt/IPv4 回程 · TCP/截屏2025-12-17 上午10.49.20.png' | relative_url }}" alt="IPv4 回程 TCP 3" width="32%" />
</div>

</details>

### 实时监控
- **实时三网 ICMP**：<https://ping.nxtrace.org/monitor/goto/HEhVjEINg>
- **实时三网 TCP**：<https://ping.nxtrace.org/monitor/goto/CGCVjPSHg>
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
<summary>综合性能跑分</summary>

![综合性能跑分]({{ '/assets/images/misaka-ber-opt/综合性能跑分.png' | relative_url }})

</details>

### IP 解锁

<details markdown="1">
<summary>流媒体 / 平台解锁记录</summary>

![解锁情况 1]({{ '/assets/images/misaka-ber-opt/解锁情况/2025-12-17 10.30.59.png' | relative_url }})
![解锁情况 2]({{ '/assets/images/misaka-ber-opt/解锁情况/2025-12-17 10.31.00.png' | relative_url }})

</details>
