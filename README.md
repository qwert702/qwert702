# qwert702

**AetherOS 作者与维护者。**

我在做一个从内核之上重新构建的桌面操作系统：Linux 内核 + 全自研 Rust 用户态 +
带逐工具权限闸门的 AI 中枢。目标不是重写内核，而是证明“内核之上那一层”也可以
从 PID 1、窗口合成器、终端、中文输入法到 AI 操作全部自己写，并且仍然能安装和运行
真实的 Linux 软件。

## AetherOS

- 官网：<https://aether.cbnac.com/>
- 源码：<https://github.com/qwert702/AetherOS>
- 文档入口：<https://github.com/qwert702/AetherOS/blob/main/docs/README.md>
- 下载：<https://github.com/qwert702/AetherOS/releases/tag/v0.1.1>

当前阶段：**v0.1.1 早期版本**。可在 QEMU / VirtualBox / VMware 启动，能安装真实
Linux 软件；物理机、生产更新源和 ISO 发布闭环仍在推进。具体数字与未验证项以仓库
文档为准，不在这里手抄。

## 我关注的东西

- **可验证**：单元测试、门禁、像素回归、CI 结果必须能复跑，不靠“我觉得没问题”。
- **安全默认**：权限分级、确认令牌、审计日志、更新签名、无口令必须显式选择。
- **诚实的边界**：没在真机跑过的，就写“未验证”；不把 VM 结果说成物理机结果。
- **可维护的代码**：先拆职责，再谈功能；大文件不应该是长期状态。

## 技术栈

Rust · Linux · Buildroot · framebuffer compositing · PTY/VT · Wayland（探索中） ·
Ed25519 签名 · GitHub Actions

## 联系

- Bug / 功能请求：<https://github.com/qwert702/AetherOS/issues>
- 代码贡献：欢迎提 PR；请先读仓库的 `CONTRIBUTING.md` 与 `docs/README.md`

---

*This profile is intentionally short. The project is the portfolio: see the pinned
AetherOS repository for architecture, evidence, and current limits.*