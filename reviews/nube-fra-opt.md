---
layout: default
title: "🇩🇪 Nube FRA 德国法兰克福中国优化 VPS 测评"
seo_keywords: "法兰克福VPS, 牛彼云, CMIN2, 9929, 德国VPS, EPYC"
redirect_from:
  - /reviews/nube-fra-opt.md
  - /REVIEW/reviews/nube-fra-opt.md
---

# 🇩🇪 Nube FRA 德国法兰克福中国优化 VPS 测评

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

- **出站流量**：$0.0125 / GB（仅按出站计费）
- **存储（NVMe）**：$0.05605 / GB / 30 天
- **IP（IPv4 + IPv6 各一个）**：$0.7992 / 30 天

</details>

### 购买链接

- [**官方购买入口**](https://console.nube.sh/zh-cn/vm/place-order?compute=pm_gp_amd_epyc_g3_shared_1c1g&storage=pm_gp_storage_Nvme_NVMe&size=10&ip=pm_gp_ip_ip&network=pm_gp_network_china_direct_group_fra_china_direct_fra&zone=random&cycle=1hr&affId=810967136T9BYK)

## 评

<div style="margin: 1rem 0; padding: 1rem 1.1rem; border: 2px solid #dc2626; border-left-width: 6px; border-radius: 6px; background: #fef2f2; color: #7f1d1d;">
  <p style="margin: 0 0 0.5rem; font-size: 1.05rem; font-weight: 700;">⚠️ 当前评价：不推荐购买</p>
  <p style="margin: 0;">由于该商家服务过于不稳定，且频繁切换线路，当前不推荐购买。下方原测评内容仅反映当时测试状态，不应作为当前购买决策依据。</p>
</div>

牛肉的德国鸡，移动/联通快乐鸡（延迟低，速度快），电信方向尚可。  
国际线路一般般：Telxius（现在还有RETN，但是过段时间会换成Orange），但是考虑到他家特色出站流量按量计费，对少流量用户非常友好，大流量就不太划算了。  
总体而言，推荐移动/联通用户选择，速度很稳，对于电信用户，不同区域差异较大，需谨慎选择。  

电信 CUG VIP(aka 9929) 回程 / RETN 去程  
联通 CUG VIP 回程 / CUG VIP 去程  
移动 CMIN2 回程 / CMIN2 回程  
另 IPv6 有三网方向优化（CMIN2+CUG VIP）

**主要提示：Nube该区域存在两种流量配置，本测评测的是中国优化版本，对应的流量价格不同，其他价格一致。**

## 测

### 路由表现

<details markdown="1">
<summary>线路概览</summary>

**IPv4 路由图**
![ipv4-radar]({{ '/assets/images/nube-fra-opt/4-radar.png' | relative_url }})

**IPv6 路由图**
![ipv6-radar]({{ '/assets/images/nube-fra-opt/6-radar.png' | relative_url }})

</details>

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
  <img src="{{ '/assets/images/nube-fra-opt/IPv4 回程 · ICMP/2025-12-21 15.01.47.png' | relative_url }}" alt="IPv4 回程 ICMP 2" width="32%" />
  <img src="{{ '/assets/images/nube-fra-opt/IPv4 回程 · ICMP/2025-12-15 21.56.41.png' | relative_url }}" alt="IPv4 回程 ICMP 3" width="32%" />
</div>

</details>

<details markdown="1">
<summary>IPv4 回程 · TCP</summary>

<div align="center">
  <img src="{{ '/assets/images/nube-fra-opt/IPv4 回程 · TCP/2025-12-15 21.57.02.png' | relative_url }}" alt="IPv4 回程 TCP 1" width="32%" />
  <img src="{{ '/assets/images/nube-fra-opt/IPv4 回程 · TCP/2025-12-21 15.02.49.png' | relative_url }}" alt="IPv4 回程 TCP 2" width="32%" />
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
<summary>IPv6 回程 · ICMP</summary>

<div align="center">
  <img src="{{ '/assets/images/nube-fra-opt/IPv6 回程 · ICMP/2025-12-15 22.01.59.png' | relative_url }}" alt="IPv6 回程 ICMP 1" width="32%" />
  <img src="{{ '/assets/images/nube-fra-opt/IPv6 回程 · ICMP/2025-12-21 15.03.25.png' | relative_url }}" alt="IPv6 回程 ICMP 2" width="32%" />
  <img src="{{ '/assets/images/nube-fra-opt/IPv6 回程 · ICMP/2025-12-15 22.02.03.png' | relative_url }}" alt="IPv6 回程 ICMP 3" width="32%" />
</div>

</details>

<details markdown="1">
<summary>IPv6 回程 · TCP</summary>

<div align="center">
  <img src="{{ '/assets/images/nube-fra-opt/IPv6 回程 · TCP/2025-12-21 15.03.57.png' | relative_url }}" alt="IPv6 回程 TCP 1" width="32%" />
  <img src="{{ '/assets/images/nube-fra-opt/IPv6 回程 · TCP/2025-12-15 22.06.08.png' | relative_url }}" alt="IPv6 回程 TCP 2" width="32%" />
  <img src="{{ '/assets/images/nube-fra-opt/IPv6 回程 · TCP/2025-12-15 22.09.20.png' | relative_url }}" alt="IPv6 回程 TCP 3" width="32%" />
</div>

</details>

### 北京四网代理单线程测速

<details markdown="1">
<summary>北京移动晚高峰</summary>

![北京移动晚高峰]({{ '/assets/images/nube-fra-opt/北京四网代理单线程测速/北京移动晚高峰.jpg' | relative_url }})

</details>

<details markdown="1">
<summary>北京移动白天</summary>

![北京移动白天]({{ '/assets/images/nube-fra-opt/北京四网代理单线程测速/北京移动白天.jpg' | relative_url }})

</details>

<details markdown="1">
<summary>北京联通晚高峰</summary>

![北京联通晚高峰]({{ '/assets/images/nube-fra-opt/北京四网代理单线程测速/北京联通晚高峰.jpg' | relative_url }})

</details>

<details markdown="1">
<summary>北京联通白天</summary>

![北京联通白天]({{ '/assets/images/nube-fra-opt/北京四网代理单线程测速/北京联通白天.jpg' | relative_url }})

</details>

<details markdown="1">
<summary>北京网通晚高峰</summary>

![北京网通晚高峰]({{ '/assets/images/nube-fra-opt/北京四网代理单线程测速/北京网通晚高峰.jpg' | relative_url }})

</details>

<details markdown="1">
<summary>北京网通白天</summary>

![北京网通白天]({{ '/assets/images/nube-fra-opt/北京四网代理单线程测速/北京网通白天.jpg' | relative_url }})

</details>

<details markdown="1">
<summary>北京电信晚高峰</summary>

![北京电信晚高峰]({{ '/assets/images/nube-fra-opt/北京四网代理单线程测速/北京电信晚高峰.jpg' | relative_url }})

</details>

<details markdown="1">
<summary>北京电信白天</summary>

![北京电信白天]({{ '/assets/images/nube-fra-opt/北京四网代理单线程测速/北京电信白天.jpg' | relative_url }})

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
