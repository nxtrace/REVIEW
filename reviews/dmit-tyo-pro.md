---
layout: default
title: DMIT.TYO.Pro
redirect_from:
  - /reviews/dmit-tyo-pro.md
  - /REVIEW/reviews/dmit-tyo-pro.md
---

# DMIT.TYO.Pro

<div class="toc-container" markdown="1">

## 目录
{: .no_toc }

* TOC
{:toc}

</div>

## 买

（待补充）

## 评

三网 CTG GIA 回程（aka CN2 GIA）；去程方面移动 CMI，电信 / 联通 CTG GIA。IPv6 有三网优化（163 + CMI 可用性尚可）。

## 测

### 路由表现

<details markdown="1">
<summary>IPv4 去程</summary>

<div align="center">
  <img src="{{ '/assets/images/dmit-tyo-pro/IPv4去程/2025-12-15 15.43.04.png' | relative_url }}" alt="IPv4 去程路由 1" width="32%" />
  <img src="{{ '/assets/images/dmit-tyo-pro/IPv4去程/2025-12-15 15.43.05.png' | relative_url }}" alt="IPv4 去程路由 2" width="32%" />
  <img src="{{ '/assets/images/dmit-tyo-pro/IPv4去程/2025-12-15 15.43.06.png' | relative_url }}" alt="IPv4 去程路由 3" width="32%" />
</div>

</details>

<details markdown="1">
<summary>IPv4 回程 · ICMP</summary>

<div align="center">
  <img src="{{ '/assets/images/dmit-tyo-pro/IPv4 回程 · ICMP/2025-12-15 15.41.00.png' | relative_url }}" alt="IPv4 回程 ICMP 1" width="32%" />
  <img src="{{ '/assets/images/dmit-tyo-pro/IPv4 回程 · ICMP/2025-12-15 15.41.02.png' | relative_url }}" alt="IPv4 回程 ICMP 2" width="32%" />
  <img src="{{ '/assets/images/dmit-tyo-pro/IPv4 回程 · ICMP/2025-12-15 15.41.04.png' | relative_url }}" alt="IPv4 回程 ICMP 3" width="32%" />
</div>

</details>

<details markdown="1">
<summary>IPv4 回程 · TCP</summary>

<div align="center">
  <img src="{{ '/assets/images/dmit-tyo-pro/IPv4 回程 · TCP/2025-12-15 15.41.41.png' | relative_url }}" alt="IPv4 回程 TCP 1" width="32%" />
  <img src="{{ '/assets/images/dmit-tyo-pro/IPv4 回程 · TCP/2025-12-15 15.41.56.png' | relative_url }}" alt="IPv4 回程 TCP 2" width="32%" />
  <img src="{{ '/assets/images/dmit-tyo-pro/IPv4 回程 · TCP/2025-12-15 15.41.57.png' | relative_url }}" alt="IPv4 回程 TCP 3" width="32%" />
</div>

</details>

<details markdown="1">
<summary>IPv6 去程</summary>

<div align="center">
  <img src="{{ '/assets/images/dmit-tyo-pro/IPv6去程/2025-12-15 15.53.39.png' | relative_url }}" alt="IPv6 去程路由 1" width="32%" />
  <img src="{{ '/assets/images/dmit-tyo-pro/IPv6去程/2025-12-15 15.53.41.png' | relative_url }}" alt="IPv6 去程路由 2" width="32%" />
  <img src="{{ '/assets/images/dmit-tyo-pro/IPv6去程/2025-12-15 15.53.43.png' | relative_url }}" alt="IPv6 去程路由 3" width="32%" />
</div>

</details>

<details markdown="1">
<summary>IPv6 回程 · TCP</summary>

<div align="center">
  <img src="{{ '/assets/images/dmit-tyo-pro/IPv6 回程 · TCP/2025-12-15 16.40.32.png' | relative_url }}" alt="IPv6 回程 TCP 1" width="32%" />
  <img src="{{ '/assets/images/dmit-tyo-pro/IPv6 回程 · TCP/2025-12-15 16.40.36.png' | relative_url }}" alt="IPv6 回程 TCP 2" width="32%" />
  <img src="{{ '/assets/images/dmit-tyo-pro/IPv6 回程 · TCP/2025-12-15 16.40.39.png' | relative_url }}" alt="IPv6 回程 TCP 3" width="32%" />
</div>

</details>

<details markdown="1">
<summary>IPv6 回程 · ICMP</summary>

<div align="center">
  <img src="{{ '/assets/images/dmit-tyo-pro/IPv6 回程 · ICMP/2025-12-15 16.39.59.png' | relative_url }}" alt="IPv6 回程 ICMP 1" width="32%" />
  <img src="{{ '/assets/images/dmit-tyo-pro/IPv6 回程 · ICMP/2025-12-15 16.40.04.png' | relative_url }}" alt="IPv6 回程 ICMP 2" width="32%" />
  <img src="{{ '/assets/images/dmit-tyo-pro/IPv6 回程 · ICMP/2025-12-15 16.40.06.png' | relative_url }}" alt="IPv6 回程 ICMP 3" width="32%" />
</div>

</details>

### 实时监控
- **实时三网 ICMP**：<https://ping.nxtrace.org/goto/sOhaZeSNg>
- **实时三网 TCP**：<https://ping.nxtrace.org/goto/haLnM6IHg>
- **Looking Glass**：<https://lg.dmit.sh/?server=tyo-pro>
- **北京三网延迟监控截图**：
  <details markdown="1">
  <summary>展开查看</summary>
  
  ![北京三网延迟监控截图]({{ '/assets/images/dmit-tyo-pro/北京三网延迟监控截图.png' | relative_url }})
  
  </details>

### 北京四网代理单线程测速

<details markdown="1">
<summary>北京移动晚高峰</summary>

![北京移动晚高峰]({{ '/assets/images/dmit-tyo-pro/北京四网代理单线程测速/北京移动晚高峰.jpg' | relative_url }})

</details>

<details markdown="1">
<summary>北京移动白天</summary>

![北京移动白天]({{ '/assets/images/dmit-tyo-pro/北京四网代理单线程测速/北京移动白天.jpg' | relative_url }})

</details>

<details markdown="1">
<summary>北京联通晚高峰</summary>

![北京联通晚高峰]({{ '/assets/images/dmit-tyo-pro/北京四网代理单线程测速/北京联通晚高峰.jpg' | relative_url }})

</details>

<details markdown="1">
<summary>北京联通白天</summary>

![北京联通白天]({{ '/assets/images/dmit-tyo-pro/北京四网代理单线程测速/北京联通白天.jpg' | relative_url }})

</details>

<details markdown="1">
<summary>北京网通晚高峰</summary>

![北京网通晚高峰]({{ '/assets/images/dmit-tyo-pro/北京四网代理单线程测速/北京网通晚高峰.jpg' | relative_url }})

</details>

<details markdown="1">
<summary>北京网通白天</summary>

![北京网通白天]({{ '/assets/images/dmit-tyo-pro/北京四网代理单线程测速/北京网通白天.jpg' | relative_url }})

</details>

<details markdown="1">
<summary>北京电信晚高峰</summary>

![北京电信晚高峰]({{ '/assets/images/dmit-tyo-pro/北京四网代理单线程测速/北京电信晚高峰.jpg' | relative_url }})

</details>

<details markdown="1">
<summary>北京电信白天</summary>

![北京电信白天]({{ '/assets/images/dmit-tyo-pro/北京四网代理单线程测速/北京电信白天.jpg' | relative_url }})

</details>

### 机器性能跑分

<details markdown="1">
<summary>综合性能跑分</summary>

![综合性能跑分]({{ '/assets/images/dmit-tyo-pro/综合性能跑分.png' | relative_url }})

</details>

### IP 解锁

<details markdown="1">
<summary>流媒体 / 平台解锁记录</summary>

![解锁情况 1]({{ '/assets/images/dmit-tyo-pro/解锁情况/2025-12-15 15.36.38.png' | relative_url }})
![解锁情况 2]({{ '/assets/images/dmit-tyo-pro/解锁情况/2025-12-15 15.36.50.png' | relative_url }})

</details>

#DMIT #review

