# flux-panel转发面板


本项目基于 [go-gost/gost](https://github.com/go-gost/gost) 和 [go-gost/x](https://github.com/go-gost/x) 两个开源库，实现了转发面板。
---
## 文档地址
- [文档地址](https://tes.cc)
---
## 特性

- 支持按 **隧道账号级别** 管理流量转发数量，可用于用户/隧道配额控制
- 支持 **TCP** 和 **UDP** 协议的转发
- 支持两种转发模式：**端口转发** 与 **隧道转发**
- 可针对 **指定用户的指定隧道进行限速** 设置
- 支持配置 **单向或双向流量计费方式**，灵活适配不同计费模型
- 提供灵活的转发策略配置，适用于多种网络代理场景


---
# 流量统计算法

## 流量流向定义

```
用户端 ←→ 转发服务器 ←→ 目标服务器/出口节点
```

## 使用场景

> 💡 **提示**：可以在创建隧道时选择不同的流量计算方式，灵活适配不同的业务需求
---

## 部署流程

### 源码编译部署

```bash

暂时没时间写，能源码部署的都是大佬，不差我这点文档
```
---
### Docker Compose部署
#### 快速部署

```bash
curl -L https://raw.githubusercontent.com/loadinghtml/flux-panel/refs/heads/main/panel_install.sh -o panel_install.sh && chmod +x panel_install.sh && ./panel_install.sh

```

#### 节点更新

```bash
curl -L https://raw.githubusercontent.com/loadinghtml/flux-panel/refs/heads/main/install.sh -o install.sh && chmod +x install.sh && ./install.sh

```

#### 默认管理员账号

- **账号**: admin_user
- **密码**: admin_user

> ⚠️ 首次登录后请立即修改默认密码！
