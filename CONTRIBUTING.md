# 贡献指南

感谢您对本项目的关注！我们欢迎所有形式的贡献，包括但不限于提交测评、改进文档、修复错误等。

## 📝 如何贡献测评

### 1. 准备工作

- Fork 本仓库到您的 GitHub 账号
- Clone 您 fork 的仓库到本地
- 创建新的分支进行工作

```bash
git clone https://github.com/<YOUR-USERNAME>/REVIEW.git
cd REVIEW
git checkout -b add-review-provider-name
```

### 2. 编写测评

1. 使用提供的模板 `templates/review-template.md`
2. 在 `reviews/` 目录下创建或选择对应的服务商文件夹
3. 创建新的测评文档，文件名建议格式：`服务商-产品型号-YYYY-MM-DD.md`

**目录组织示例**：
```
reviews/
├── vultr/
│   ├── vultr-high-frequency-2023-01-15.md
│   └── vultr-cloud-compute-2023-02-20.md
├── digitalocean/
│   └── do-basic-droplet-2023-03-10.md
└── bandwagonhost/
    └── bwh-cn2-gia-2023-04-05.md
```

### 3. 测评内容要求

#### 必须包含的内容

- ✅ 基本信息（服务商、价格、配置等）
- ✅ 硬件配置详情
- ✅ 至少一项性能测试（CPU/磁盘/内存）
- ✅ 网络测试（速度/延迟/路由）
- ✅ 综合评价（优缺点、适用场景）

#### 推荐包含的内容

- 📊 多项性能跑分
- 🌐 详细的路由追踪
- 📺 流媒体解锁情况
- 🔒 IP 质量检测
- 📈 长期稳定性监控

#### 内容准则

- **客观真实**：所有测试数据必须真实可靠
- **详细完整**：提供足够的测试细节和截图
- **时效性**：注明测评日期，避免过时信息
- **中立立场**：保持中立，不夸大也不贬低

### 4. 格式规范

- 使用 Markdown 格式编写
- 遵循模板结构，保持文档一致性
- 代码块使用正确的语法高亮
- 表格对齐整齐
- 使用 emoji 适度增强可读性（可选）

### 5. 提交规范

**Commit 消息格式**：

```
类型: 简短描述

详细说明（可选）
```

**类型说明**：
- `add`: 添加新测评
- `update`: 更新已有测评
- `fix`: 修复错误
- `docs`: 文档改进
- `style`: 格式调整

**示例**：
```
add: 添加 Vultr High Frequency 测评

- 测试了 CPU 性能
- 完成了全球网络延迟测试
- 包含流媒体解锁检测
```

### 6. 提交 Pull Request

1. 推送您的分支到 GitHub

```bash
git add .
git commit -m "add: 添加 XXX 服务商测评"
git push origin add-review-provider-name
```

2. 在 GitHub 上创建 Pull Request
3. 填写 PR 描述，说明测评的主要内容
4. 等待维护者审核

## 🔍 测评质量标准

我们会从以下方面审核提交的测评：

- ✅ 内容完整性（是否包含必要的测试项）
- ✅ 数据真实性（测试结果是否合理）
- ✅ 格式规范性（是否遵循模板和规范）
- ✅ 时效性（测评日期是否标注）
- ✅ 可读性（排版是否清晰易读）

## 🛠️ 推荐测试工具

### 性能测试
- **CPU**: [sysbench](https://github.com/akopytov/sysbench), [UnixBench](https://github.com/kdlucas/byte-unixbench), [Geekbench](https://www.geekbench.com/)
- **磁盘**: [dd](https://linux.die.net/man/1/dd), [fio](https://fio.readthedocs.io/)
- **内存**: sysbench memory

### 网络测试
- **速度**: [speedtest-cli](https://github.com/sivel/speedtest-cli), [iperf3](https://iperf.fr/)
- **路由**: [mtr](https://www.bitwizard.nl/mtr/), [nexttrace](https://github.com/nxtrace/NTrace-core)
- **多地ping**: [ping.pe](https://ping.pe)

### 综合测试
- **一键脚本**: 
  - [bench.sh](https://github.com/teddysun/across)
  - [LemonBench](https://github.com/LemonBench/LemonBench)
  - [superbench](https://github.com/oooldking/script)

### 流媒体测试
- [RegionRestrictionCheck](https://github.com/lmc999/RegionRestrictionCheck)

## ❓ 常见问题

### Q: 我没有足够的测试经验怎么办？

A: 可以使用一键测试脚本（如 bench.sh），它会自动完成大部分测试并生成报告。

### Q: 测评中的某些项目我无法测试怎么办？

A: 没关系，填写您能完成的部分即可。必须包含的内容请尽量完成。

### Q: 可以更新其他人的测评吗？

A: 可以！如果服务商配置或性能有变化，欢迎提交更新。请在文件名和内容中注明更新日期。

### Q: 发现测评中的错误怎么办？

A: 请提交 Issue 或直接 PR 修复。

## 📧 联系方式

如有任何问题或建议，欢迎：
- 提交 [Issue](../../issues)
- 发起 [Discussion](../../discussions)

---

再次感谢您的贡献！您的每一份测评都将帮助更多人做出更好的选择。
