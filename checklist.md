# ✅ 项目启动 Checklist（第一次智能体实战课）

为了顺利开启「懂你的协作助手」智能体开发，请在开课前完成下列准备。建议按顺序逐项勾选，排除环境和资源风险。

---

## 🖥️ 一、基础环境

- 操作系统：**macOS / Linux / Windows** 均可
- 网络：可稳定访问 GitHub（若需请提前准备代理/镜像）

---

## 🛠️ 二、核心软件

### 1. Python（必备）
- 版本：**Python ≥ 3.12**
- 推荐管理工具：[`pyenv`](https://github.com/pyenv/pyenv#installation) / [`Miniconda`](https://docs.anaconda.com/miniconda/)
- 安装指引：参考上述链接完成安装后，新建 3.12 环境
- 自检命令：
  ```bash
  python3 --version
  pyenv versions
  ```

### 2. Node.js（必备）
- 版本：**Node.js ≥ 18.x**
- 推荐使用 [`nvm`](https://github.com/nvm-sh/nvm#installing-and-updating) 管理版本
- 安装指引：按照链接步骤安装 nvm 后执行 `nvm install 18`
- 自检：
  ```bash
  node -v
  npm -v
  ```

~ % nvm --version
0.40.3
~ % nvm install 18
Downloading and installing node v18.20.8...
Downloading https://nodejs.org/dist/v18.20.8/node-v18.20.8-darwin-arm64.tar.xz...
############################################# 100.0%
Computing checksum with sha256sum
Checksums matched!
Now using node v18.20.8 (npm v10.8.2)
Creating default alias: default -> 18 (-> v18.20.8)
~ % node -v      
v18.20.8

  
- 安装示例：
  ```bash
  nvm install 18
  ```

### 3. 包管理器
- 任选其一：`npm`（随 Node.js 自带）或 [`pnpm`](https://pnpm.io/installation)（推荐）
- 安装 `pnpm`：
  ```bash
  npm install -g pnpm
  ```

### 4. Git（必备）
- 用途：管理课程代码 & 克隆官方仓库
- 安装指引：参考 [Git 官方下载页](https://git-scm.com/downloads) 选择对应系统；macOS 也可使用 `brew install git`
- 自检：
  ```bash
  git --version
  ```
- 常见配置：
  ```bash
  git config --global user.name "你的名字"
  git config --global user.email "你的邮箱"
  ```
~ % git --version
git version 2.39.5 (Apple Git-154)

### 5. Docker（必备）
- 用途：运行课程中的本地服务
- 安装建议：
  - macOS：Docker Desktop（https://www.docker.com/products/docker-desktop/）
  - Windows：Docker Desktop / WSL2 + Docker（同上链接）
  - Linux：根据发行版安装 `docker` + `docker-compose`（参考 https://docs.docker.com/engine/install/）
- 自检：
  ```bash
  docker --version
  docker compose version
  ```
**~ % docker --version
Docker version 27.3.1, build ce12230
**---

## 🔑 三、API Key 准备

- 至少准备 **1 个可用 LLM 服务** 的 API Key
- 推荐性价比渠道（含 15 元新用户福利）：https://ppio.com/user/register?invited_by=1X35A7
- 想使用海外大模型？推荐 **Grok 4.1**（性价比之王），可通过 https://zenmux.ai/invite/1ECQGA 快速注册获取额度
- 记得妥善保存 Key，以便课堂练习直接使用

---

## 📦 四、预先克隆课程仓库

为避免课堂时遭遇 GitHub 限速，请提前 clone：

1. **Open WebUI**（本地/私有 AI 工作台）
   ```bash
   git clone https://github.com/open-webui/open-webui.git
   ```
项目295MB，国内直接git clone可能较慢，可用其他国内同步镜像，如GitCode https://gitcode.com/kynot321/open-webui
   
2. **MemMachine**（长期记忆能力）
   ```bash
   git clone https://github.com/MemMachine/MemMachine.git
   ```

如网络不佳，请准备代理或使用镜像源。

---

## 📚 五、你将完成的核心能力

- 将大模型接入本地 WebUI，打造自己的控制台
- 为智能体构建“长期记忆”，实现持续学习与上下文追溯
- 让智能体吸收你的写作风格，实现个性化输出
- 打造专属的「AI 协作助手」并部署到真实场景
