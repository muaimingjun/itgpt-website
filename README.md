# ITGPT - AI 智能体一站式开发平台

这是一个为 "ITGPT" 品牌打造的现代化、响应式的前端网站。项目使用 Vue 3 和 Vite 构建，并拥有一个灵感来源于 `dora.run/ai` 的未来感设计。

## ✨ 特性

- **现代化的 UI/UX**: 采用深色主题、玻璃拟态效果和流畅的动画，提供卓越的用户体验。
- **完全响应式**: 无论是在桌面还是移动设备上，都能完美展示。
- **组件化架构**: 使用 Vue 3 构建，代码结构清晰，易于维护和扩展。
- **Docker 支持**: 提供 `Dockerfile`，可轻松将应用容器化并进行部署。

## 🛠️ 技术栈

- **框架**: [Vue 3](https://vuejs.org/)
- **构建工具**: [Vite](https://vitejs.dev/)
- **语言**: JavaScript, HTML, CSS
- **部署**: [Docker](https://www.docker.com/), [Nginx](https://www.nginx.com/)

---

## 🚀 本地开发

### 1. 克隆项目
```sh
git clone <your-repo-url>
cd itgpt-website
```

### 2. 安装依赖
```sh
npm install
```

### 3. 启动开发服务器
```sh
npm run dev
```
应用将在 `http://localhost:5173` (或另一个可用端口) 上运行。

### 4. 构建生产版本
```sh
npm run build
```
构建后的静态文件将位于 `dist` 目录中。

---

## 🐳 使用 Docker 部署

### 1. 构建 Docker 镜像
确保你的设备上已安装 Docker。在项目根目录下，运行以下命令：
```sh
docker build -t itgpt-website .
```

### 2. 运行 Docker 容器
构建完成后，使用以下命令启动容器：
```sh
docker run -d -p 8080:80 --name itgpt-container itgpt-website
```
- `-d`: 在后台运行容器。
- `-p 8080:80`: 将主机的 8080 端口映射到容器的 80 端口。
- `--name itgpt-container`: 为容器指定一个名称。

现在，你可以通过访问 `http://localhost:8080` 来查看正在运行的应用。

### 3. 管理容器
- **查看日志**: `docker logs itgpt-container`
- **停止容器**: `docker stop itgpt-container`
- **移除容器**: `docker rm itgpt-container`
