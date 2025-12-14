# Misaka.HKG.Opt

716GB 单向计费 @ 无端口限速 = 21 USD / 月。

> 提示：本文中的截图来自 GitHub 附件，便于读者直接展开查看；实时监控等动态数据依旧通过官方链接获取。

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

<details>
<summary>IPv4 去程</summary>

![IMAGE 2025-12-14 13:27:53](https://github.com/user-attachments/assets/997f0bcf-77c8-4266-abaa-655088725eb1)
![IMAGE 2025-12-14 13:28:52](https://github.com/user-attachments/assets/8465bed7-a350-40ab-81d8-c5188e0a52e3)
![IMAGE 2025-12-14 13:28:47](https://github.com/user-attachments/assets/63246c11-8087-46ba-83f9-972aafb5be05)

</details>

<details>
<summary>IPv4 回程 · ICMP</summary>

![IMAGE 2025-12-14 13:29:37](https://github.com/user-attachments/assets/580671ff-19bc-4703-a60c-9a36456d9194)
![IMAGE 2025-12-14 13:29:40](https://github.com/user-attachments/assets/7f83cd28-1fef-4355-b711-c6191873e0b3)
![IMAGE 2025-12-14 13:29:43](https://github.com/user-attachments/assets/15a0cff6-6f7e-430e-a11f-95e7352899a8)

</details>

<details>
<summary>IPv4 回程 · TCP</summary>

![IMAGE 2025-12-14 13:30:12](https://github.com/user-attachments/assets/6e778222-9a33-49df-820a-20c806b3653f)
![IMAGE 2025-12-14 13:30:15](https://github.com/user-attachments/assets/f06e99c8-d672-4b30-aa44-a0de6de3752a)
![IMAGE 2025-12-14 13:30:17](https://github.com/user-attachments/assets/bd132f11-b4bc-4d7e-9d6d-b27a293a379e)

</details>

### 实时监控
- **实时三网 ICMP**：<https://ping.nxtrace.org/goto/yQTjSoMvR>
- **实时三网 TCP**：<https://ping.nxtrace.org/goto/6JCjITGvR>
- **Looking Glass**：<https://ping.sx/mtr?p=234>
- 北京三网延迟监控截图会补到 `assets/images/misaka-hkg-opt/latency-beijing.png`，届时同样采用折叠展示；当前可直接查看以上实时页面。

### 北京四网代理单线程测速

<details>
<summary>北京移动晚高峰</summary>

![北京移动晚高峰](https://github.com/user-attachments/assets/16ea14c9-4938-4829-8dd8-23b0e248217d)

</details>

<details>
<summary>北京移动白天</summary>

![北京移动白天](https://github.com/user-attachments/assets/75bfe783-d8e3-4852-94ca-90bb91f98d17)

</details>

<details>
<summary>北京联通晚高峰</summary>

![北京联通晚高峰](https://github.com/user-attachments/assets/dc104038-d5cf-4a6f-906d-55af5d0113dd)

</details>

<details>
<summary>北京联通白天</summary>

![北京联通白天](https://github.com/user-attachments/assets/7a1543ae-493c-4ba1-a198-52aebca1e666)

</details>

<details>
<summary>北京网通 / 鹏博士晚高峰</summary>

![北京网通晚高峰](https://github.com/user-attachments/assets/2d9e4efa-2107-4407-aabe-7f219bc496d4)

</details>

<details>
<summary>北京网通 / 鹏博士白天</summary>

![北京网通白天](https://github.com/user-attachments/assets/bf5df076-3099-450e-8e83-b828ff8ecc6b)

</details>

<details>
<summary>北京电信晚高峰</summary>

![北京电信晚高峰](https://github.com/user-attachments/assets/cdd66c39-4925-457c-8e1e-287c293e16ad)

</details>

<details>
<summary>北京电信白天</summary>

![北京电信白天](https://github.com/user-attachments/assets/67b8af64-c6cc-4e30-916c-b5c0450dd1f7)

</details>

### 机器性能跑分

<details>
<summary>综合性能跑分</summary>

![IMAGE 2025-12-14 13:34:19](https://github.com/user-attachments/assets/2e4e78cb-102a-4cf3-b122-a76033379523)

</details>

### IP 解锁

<details>
<summary>流媒体 / 平台解锁记录</summary>

![IMAGE 2025-12-14 13:34:28](https://github.com/user-attachments/assets/066e3164-5206-4025-b23f-341c214715f3)
![IMAGE 2025-12-14 13:34:31](https://github.com/user-attachments/assets/d39a069c-6bf6-4cc2-bb29-146c0a8322e7)

</details>

### 后续扩展
- 新增截图时，沿用 `<details>` 模板可保持页面紧凑，并在折叠正文中补充测试时间/环境说明。
- 如需补充多线程、UDP、节假日等场景，可继续在「测」章节增加子节，与现有结构一致。
