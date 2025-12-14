# Misaka.HKG.Opt

716GB 单向计费 @ 无端口限速 = 21 USD / 月。

> 提示：文中所有 Telegram 链接目前仅作为临时截图来源，后续会改为引用仓库内的本地图片。

## 买

### 规格对照（可展开查看）

<details>
<summary>S3N · Standard NVMe · Gen3 · AMD EPYC</summary>

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

<details>
<summary>S3P2 · Standard NVMe · Gen3 · WAN Latency Optimized</summary>

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
- **线路策略**：三网「尽力而为」的优化，重点改善国内回程体验。
- **定位**：适合需要香港落地、对延迟/回国线路敏感的场景。

## 评

三网回程策略的「尽力而为」在测试样本中表现稳定，香港落地对北方地区延迟控制不错，配合 716GB 单向计费和不限端口的设定，适合需要少量高质量线路的回国业务，但带宽峰值与超量费用仍需关注。

## 测

### 路由表现
- **IPv4 去程**：<https://t.me/nanaselog/602>
- **IPv4 回程（ICMP）**：<https://t.me/nanaselog/737>
- **IPv4 回程（TCP）**：<https://t.me/nanaselog/730>

### 实时监控
- **实时三网 ICMP**：<https://ping.nxtrace.org/goto/yQTjSoMvR>
- **实时三网 TCP**：<https://ping.nxtrace.org/goto/6JCjITGvR>
- **Looking Glass**：<https://ping.sx/mtr?p=234>
- 北京三网延迟监控截图稍后会补到 `assets/images/misaka-hkg-opt/`，目前可直接查看上述实时页面。

### 北京四网代理单线程测速
- 截图：<https://t.me/nanaselog/1638>

### 机器性能跑分
- 截图：<https://t.me/nanaselog/1639>

### IP 解锁
- 观测截图：<https://t.me/nanaselog/1640>

### 后续扩展
- 建议将测速、路由与跑分截图按章节命名后存放到 `assets/images/misaka-hkg-opt/`，并使用 `![描述](相对路径)` 引用，便于 GitHub 在线阅读。
- 如需补充更多测试维度（多线程、UDP、特殊时段等），可继续在本节下新增子节。
