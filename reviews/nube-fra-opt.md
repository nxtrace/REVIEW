---
layout: default
title: Nube.FRA.Opt
redirect_from:
  - /reviews/nube-fra-opt.md
  - /REVIEW/reviews/nube-fra-opt.md
---

# Nube.FRA.Opt

<div class="toc-container" markdown="1">

## 目录
{: .no_toc }

* TOC
{:toc}

</div>

## 买

### 规格对照

> 说明：Nube 为按量计费（出站流量计费），以下为常见配置的「30 天」价格参考。

<details markdown="1">
<summary>计算规格（AMD EPYC · 共享型）</summary>

| 规格 | vCPU | 内存 | 价格（30 天） |
|---|---:|---:|---:|
| a3s.1c1g | 1 | 1 GB | $0.841 |
| a3s.1c2g | 1 | 2 GB | $1.8047 |
| a3s.2c2g | 2 | 2 GB | $5.3541 |
| a3s.2c4g | 2 | 4 GB | $9.798 |
| a3s.4c4g | 4 | 4 GB | $11.6817 |
| a3s.4c8g | 4 | 8 GB | $21.2898 |
| a3s.8c8g | 8 | 8 GB | $25.3103 |
| a3s.8c16g | 8 | 16 GB | $45.9649 |
| a3s.16c16g | 16 | 16 GB | $54.5144 |
| a3s.16c32g | 16 | 32 GB | $98.7027 |

</details>

<details markdown="1">
<summary>计费项</summary>

- **出站流量**：$0.0117 / GB（仅按出站计费）
- **存储（NVMe）**：$0.05605 / GB / 30 天
- **IP（IPv4 + IPv6 各一个）**：$0.6048 / 30 天

</details>

### 购买链接

- [Nube](https://nube.sh/invite/810967136T9BYK)

## 评

（待补充）

## 测

### 路由表现

<details markdown="1">
<summary>IPv4 去程</summary>

<div align="center">
  <img src="{{ '/assets/images/nube-fra-opt/IPv4去程/2025-12-15 21.59.13.png' | relative_url }}" alt="IPv4 去程路由 1" width="32%" />
  <img src="{{ '/assets/images/nube-fra-opt/IPv4去程/2025-12-15 21.59.15.png' | relative_url }}" alt="IPv4 去程路由 2" width="32%" />
  <img src="{{ '/assets/images/nube-fra-opt/IPv4去程/2025-12-15 21.59.16.png' | relative_url }}" alt="IPv4 去程路由 3" width="32%" />
</div>

</details>

<details markdown="1">
<summary>IPv4 回程 · ICMP</summary>

<div align="center">
  <img src="{{ '/assets/images/nube-fra-opt/IPv4 回程 · ICMP/2025-12-15 21.56.38.png' | relative_url }}" alt="IPv4 回程 ICMP 1" width="32%" />
  <img src="{{ '/assets/images/nube-fra-opt/IPv4 回程 · ICMP/2025-12-15 21.56.40.png' | relative_url }}" alt="IPv4 回程 ICMP 2" width="32%" />
  <img src="{{ '/assets/images/nube-fra-opt/IPv4 回程 · ICMP/2025-12-15 21.56.41.png' | relative_url }}" alt="IPv4 回程 ICMP 3" width="32%" />
</div>

</details>

<details markdown="1">
<summary>IPv4 回程 · TCP</summary>

<div align="center">
  <img src="{{ '/assets/images/nube-fra-opt/IPv4 回程 · TCP/2025-12-15 21.57.02.png' | relative_url }}" alt="IPv4 回程 TCP 1" width="32%" />
  <img src="{{ '/assets/images/nube-fra-opt/IPv4 回程 · TCP/2025-12-15 21.57.15.png' | relative_url }}" alt="IPv4 回程 TCP 2" width="32%" />
  <img src="{{ '/assets/images/nube-fra-opt/IPv4 回程 · TCP/2025-12-15 21.57.16.png' | relative_url }}" alt="IPv4 回程 TCP 3" width="32%" />
</div>

</details>

<details markdown="1">
<summary>IPv6 去程</summary>

<div align="center">
  <img src="{{ '/assets/images/nube-fra-opt/IPv6去程/2025-12-15 21.59.51.png' | relative_url }}" alt="IPv6 去程路由 1" width="32%" />
  <img src="{{ '/assets/images/nube-fra-opt/IPv6去程/2025-12-15 21.59.53.png' | relative_url }}" alt="IPv6 去程路由 2" width="32%" />
  <img src="{{ '/assets/images/nube-fra-opt/IPv6去程/2025-12-15 21.59.54.png' | relative_url }}" alt="IPv6 去程路由 3" width="32%" />
</div>

</details>

<details markdown="1">
<summary>IPv6 回程 · TCP</summary>

<div align="center">
  <img src="{{ '/assets/images/nube-fra-opt/IPv6 回程 · TCP/2025-12-15 22.06.07.png' | relative_url }}" alt="IPv6 回程 TCP 1" width="32%" />
  <img src="{{ '/assets/images/nube-fra-opt/IPv6 回程 · TCP/2025-12-15 22.06.08.png' | relative_url }}" alt="IPv6 回程 TCP 2" width="32%" />
  <img src="{{ '/assets/images/nube-fra-opt/IPv6 回程 · TCP/2025-12-15 22.09.20.png' | relative_url }}" alt="IPv6 回程 TCP 3" width="32%" />
</div>

</details>

<details markdown="1">
<summary>IPv6 回程 · ICMP</summary>

<div align="center">
  <img src="{{ '/assets/images/nube-fra-opt/IPv6 回程 · ICMP/2025-12-15 22.01.59.png' | relative_url }}" alt="IPv6 回程 ICMP 1" width="32%" />
  <img src="{{ '/assets/images/nube-fra-opt/IPv6 回程 · ICMP/2025-12-15 22.02.02.png' | relative_url }}" alt="IPv6 回程 ICMP 2" width="32%" />
  <img src="{{ '/assets/images/nube-fra-opt/IPv6 回程 · ICMP/2025-12-15 22.02.03.png' | relative_url }}" alt="IPv6 回程 ICMP 3" width="32%" />
</div>

</details>

### 北京四网代理单线程测速

<details markdown="1">
<summary>北京移动晚高峰</summary>

![北京移动晚高峰]({{ '/assets/images/nube-fra-opt/北京四网代理单线程测速/北京移动晚高峰.jpg' | relative_url }})

</details>

<details markdown="1">
<summary>北京联通晚高峰</summary>

![北京联通晚高峰]({{ '/assets/images/nube-fra-opt/北京四网代理单线程测速/北京联通晚高峰.jpg' | relative_url }})

</details>

<details markdown="1">
<summary>北京网通晚高峰</summary>

![北京网通晚高峰]({{ '/assets/images/nube-fra-opt/北京四网代理单线程测速/北京网通晚高峰.jpg' | relative_url }})

</details>

<details markdown="1">
<summary>北京电信晚高峰</summary>

![北京电信晚高峰]({{ '/assets/images/nube-fra-opt/北京四网代理单线程测速/北京电信晚高峰.jpg' | relative_url }})

</details>

### 机器性能跑分

<details markdown="1">
<summary>综合性能跑分（YABS·GB5）</summary>

![综合性能跑分]({{ '/assets/images/nube-fra-opt/综合性能跑分.png' | relative_url }})

</details>

### IP 解锁

<details markdown="1">
<summary>流媒体 / 平台解锁记录</summary>

![解锁情况 1]({{ '/assets/images/nube-fra-opt/解锁情况/2025-12-15 21.54.25.png' | relative_url }})
![解锁情况 2]({{ '/assets/images/nube-fra-opt/解锁情况/2025-12-15 21.54.47.png' | relative_url }})

</details>
