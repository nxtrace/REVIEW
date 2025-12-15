---
layout: default
title: Misaka.HKG.Opt
redirect_from:
  - /reviews/misaka-hkg-opt.md
  - /REVIEW/reviews/misaka-hkg-opt.md
---

# Misaka.HKG.Opt

<div class="toc-container" markdown="1">

## 目录
{: .no_toc }

* TOC
{:toc}

</div>

## 买

### 规格对照

<details markdown="1">
<summary>Standard NVMe (Gen3, AMD EPYC)</summary>

| 套餐 | vCPU | 内存 | 本地 NVMe SSD | 流量（单向 In+Out） | 月付 |
|---|---:|---:|---:|---:|---:|
| S3N-1C1G | 1 | 1 GiB | 16 GiB | 1 TiB | $10 |
| S3N-1C2G | 1 | 2 GiB | 32 GiB | 2 TiB | $20 |
| S3N-2C3G | 2 | 3 GiB | 48 GiB | 3 TiB | $30 |
| S3N-2C4G | 2 | 4 GiB | 64 GiB | 4 TiB | $40 |
| S3N-4C6G | 4 | 6 GiB | 96 GiB | 6 TiB | $60 |
| S3N-4C8G | 4 | 8 GiB | 112 GiB | 8 TiB | $80 |
| S3N-6C12G | 6 | 12 GiB | 128 GiB | 12 TiB | $120 |
| S3N-8C16G | 8 | 16 GiB | 144 GiB | 16 TiB | $160 |
| S3N-8C24G | 8 | 24 GiB | 160 GiB | 24 TiB | $240 |
| S3N-16C32G | 16 | 32 GiB | 240 GiB | 32 TiB | $320 |

</details>

<details markdown="1">
<summary>Standard NVMe (Gen3, WAN Latency Optimized, AMD EPYC)</summary>

| 套餐 | vCPU | 内存 | 本地 NVMe SSD | 流量（单向 In+Out） | 月付 |
|---|---:|---:|---:|---:|---:|
| S3P2-1C1G | 1 | 1 GiB | 16 GiB | 716 GiB | $21 |
| S3P2-1C2G | 1 | 2 GiB | 32 GiB | 1.4 TiB | $42 |
| S3P2-2C3G | 2 | 3 GiB | 48 GiB | 2.1 TiB | $63 |
| S3P2-2C4G | 2 | 4 GiB | 64 GiB | 2.8 TiB | $84 |
| S3P2-4C6G | 4 | 6 GiB | 96 GiB | 4.2 TiB | $126 |
| S3P2-4C8G | 4 | 8 GiB | 112 GiB | 5.6 TiB | $168 |
| S3P2-6C12G | 6 | 12 GiB | 128 GiB | 8.4 TiB | $252 |
| S3P2-8C16G | 8 | 16 GiB | 144 GiB | 11.2 TiB | $336 |
| S3P2-8C24G | 8 | 24 GiB | 160 GiB | 16.8 TiB | $504 |
| S3P2-16C32G | 16 | 32 GiB | 240 GiB | 22.4 TiB | $672 |

</details>

> 说明：规格表仅供对照，库存状态以 Misaka 控制台为准。

### 购买信息
- **官方开通入口**：<https://app.misaka.io/iaas/vm/create/hkg12/s3p2-1c1g>

## 评

三网有尽力而为的优化，目前的情况仅适合落地用途使用，适合预算充裕且对国际线路和机器稳定性有较高要求的客户（该商家极少发生故障停机现象，国际线路端口充足）。

## 测

### 路由表现

<details markdown="1">
<summary>IPv4 去程</summary>

<div align="center">
  <img src="{{ '/assets/images/misaka-hkg-opt/IPv4去程/526252138-997f0bcf-77c8-4266-abaa-655088725eb1.jpg' | relative_url }}" alt="IPv4 去程路由 1" width="32%" />
  <img src="{{ '/assets/images/misaka-hkg-opt/IPv4去程/526252184-8465bed7-a350-40ab-81d8-c5188e0a52e3.jpg' | relative_url }}" alt="IPv4 去程路由 2" width="32%" />
  <img src="{{ '/assets/images/misaka-hkg-opt/IPv4去程/526252181-63246c11-8087-46ba-83f9-972aafb5be05.jpg' | relative_url }}" alt="IPv4 去程路由 3" width="32%" />
</div>

</details>

<details markdown="1">
<summary>IPv4 回程 · ICMP</summary>

<div align="center">
  <img src="{{ '/assets/images/misaka-hkg-opt/IPv4 回程 · ICMP/526252214-580671ff-19bc-4703-a60c-9a36456d9194.jpg' | relative_url }}" alt="IPv4 回程 ICMP 1" width="32%" />
  <img src="{{ '/assets/images/misaka-hkg-opt/IPv4 回程 · ICMP/526252218-7f83cd28-1fef-4355-b711-c6191873e0b3.jpg' | relative_url }}" alt="IPv4 回程 ICMP 2" width="32%" />
  <img src="{{ '/assets/images/misaka-hkg-opt/IPv4 回程 · ICMP/526252224-15a0cff6-6f7e-430e-a11f-95e7352899a8.jpg' | relative_url }}" alt="IPv4 回程 ICMP 3" width="32%" />
</div>

</details>

<details markdown="1">
<summary>IPv4 回程 · TCP</summary>

<div align="center">
  <img src="{{ '/assets/images/misaka-hkg-opt/IPv4 回程 · TCP/526252250-6e778222-9a33-49df-820a-20c806b3653f.jpg' | relative_url }}" alt="IPv4 回程 TCP 1" width="32%" />
  <img src="{{ '/assets/images/misaka-hkg-opt/IPv4 回程 · TCP/526252252-f06e99c8-d672-4b30-aa44-a0de6de3752a.jpg' | relative_url }}" alt="IPv4 回程 TCP 2" width="32%" />
  <img src="{{ '/assets/images/misaka-hkg-opt/IPv4 回程 · TCP/526252258-bd132f11-b4bc-4d7e-9d6d-b27a293a379e.jpg' | relative_url }}" alt="IPv4 回程 TCP 3" width="32%" />
</div>

</details>

### 实时监控
- **实时三网 ICMP**：<https://ping.nxtrace.org/goto/yQTjSoMvR>
- **实时三网 TCP**：<https://ping.nxtrace.org/goto/6JCjITGvR>
- **Looking Glass**：<https://ping.sx/mtr?p=234>
- **北京三网延迟监控截图**：
  <details markdown="1">
  <summary>展开查看</summary>
  
  ![北京三网延迟监控截图]({{ '/assets/images/misaka-hkg-opt/北京三网延迟监控截图(近七天).png' | relative_url }})

  </details>

### 北京四网代理单线程测速

<details markdown="1">
<summary>北京移动晚高峰</summary>

![北京移动晚高峰]({{ '/assets/images/misaka-hkg-opt/北京四网代理单线程测速/北京移动晚高峰.jpg' | relative_url }})

</details>

<details markdown="1">
<summary>北京移动白天</summary>

![北京移动白天]({{ '/assets/images/misaka-hkg-opt/北京四网代理单线程测速/北京移动白天.jpg' | relative_url }})

</details>

<details markdown="1">
<summary>北京联通晚高峰</summary>

![北京联通晚高峰]({{ '/assets/images/misaka-hkg-opt/北京四网代理单线程测速/北京联通晚高峰.jpg' | relative_url }})

</details>

<details markdown="1">
<summary>北京联通白天</summary>

![北京联通白天]({{ '/assets/images/misaka-hkg-opt/北京四网代理单线程测速/北京联通白天.jpg' | relative_url }})

</details>

<details markdown="1">
<summary>北京网通晚高峰</summary>

![北京网通晚高峰]({{ '/assets/images/misaka-hkg-opt/北京四网代理单线程测速/北京网通晚高峰.jpg' | relative_url }})

</details>

<details markdown="1">
<summary>北京网通白天</summary>

![北京网通白天]({{ '/assets/images/misaka-hkg-opt/北京四网代理单线程测速/北京网通白天.jpg' | relative_url }})

</details>

<details markdown="1">
<summary>北京电信晚高峰</summary>

![北京电信晚高峰]({{ '/assets/images/misaka-hkg-opt/北京四网代理单线程测速/北京电信晚高峰.jpg' | relative_url }})

</details>

<details markdown="1">
<summary>北京电信白天</summary>

![北京电信白天]({{ '/assets/images/misaka-hkg-opt/北京四网代理单线程测速/北京电信白天.jpg' | relative_url }})

</details>

### 机器性能跑分

<details markdown="1">
<summary>综合性能跑分（YABS·GB5）</summary>

![综合性能跑分]({{ '/assets/images/misaka-hkg-opt/综合性能跑分.jpg' | relative_url }})

</details>

### IP 解锁

<details markdown="1">
<summary>流媒体 / 平台解锁记录</summary>

![解锁情况 1]({{ '/assets/images/misaka-hkg-opt/解锁情况/526252446-066e3164-5206-4025-b23f-341c214715f3.jpg' | relative_url }})
![解锁情况 2]({{ '/assets/images/misaka-hkg-opt/解锁情况/526252448-d39a069c-6bf6-4cc2-bb29-146c0a8322e7.jpg' | relative_url }})

</details>
