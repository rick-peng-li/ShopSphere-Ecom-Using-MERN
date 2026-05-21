# 🛍️ ShopSphere - MERN 栈全栈电商平台

ShopSphere 是一个基于 MERN（MongoDB, Express, React, Node.js）栈构建的现代化电子商务平台。它为用户提供流畅的购物体验，并为管理员提供直观的后台管理系统。

## 📖 项目业务介绍

ShopSphere 旨在提供一个完整的电商解决方案，主要功能包括：

### 用户端 (Frontend)
- **产品浏览**：查看最新集合、热门产品以及按类别（男装、女装、童装）分类的产品。
- **产品详情**：查看产品的详细描述、价格、图片等。
- **购物车管理**：添加产品到购物车、调整数量、实时计算总价。
- **用户认证**：支持用户注册和登录功能。
- **响应式设计**：完美适配桌面端和移动端。

### 管理端 (Admin Panel)
- **仪表盘**：管理系统的核心入口。
- **产品管理**：管理员可以轻松添加新产品、上传图片以及删除不再销售的产品。
- **实时同步**：管理端的更改会立即反映在用户端。

---

## 🏗️ 技术架构

项目采用了前后端分离的架构：

### 后端 (Backend)
- **Node.js & Express**：构建高效、可扩展的 RESTful API。
- **MongoDB & Mongoose**：非关系型数据库，用于存储产品、用户和订单数据。
- **JWT (JSON Web Tokens)**：实现安全的用户身份验证和授权。
- **Multer & Cloudinary**：处理图片上传并存储在云端，确保高效的静态资源加载。
- **CORS**：处理跨域资源共享。

### 前端 & 管理端 (Frontend & Admin)
- **React (Vite)**：现代前端框架，提供极速的开发体验和卓越的运行时性能。
- **React Router**：管理单页面应用（SPA）的路由导航。
- **Context API**：用于全局状态管理（如购物车状态、用户状态）。
- **SweetAlert2**：提供美观的用户提示和交互弹窗。
- **CSS3**：自定义样式，实现精美的 UI 设计。

---

## 🚀 启动方式

按照以下步骤在本地环境运行项目：

### 1. 克隆项目
```bash
git clone <repository-url>
cd ShopSphere-Ecom-Using-MERN
```

### 2. 后端配置与启动
1. 进入后端目录：
   ```bash
   cd Backend
   ```
2. 安装依赖：
   ```bash
   npm install
   ```
3. 配置环境变量：在 `Backend` 目录下创建 `.env` 文件，并添加以下内容：
   ```env
   PORT=4000
   MongoAtlasDBUrl=你的MongoDB连接字符串
   CLOUDINARY_CLOUD_NAME=你的Cloudinary名称
   CLOUDINARY_API_KEY=你的Cloudinary API密钥
   CLOUDINARY_API_SECRET=你的Cloudinary API密钥
   SECRET_KEY=你的JWT密钥
   ```
4. 启动后端服务器：
   ```bash
   node index.js
   ```

### 3. 前端端配置与启动
1. 进入前端目录：
   ```bash
   cd ../Frontend
   ```
2. 安装依赖：
   ```bash
   npm install
   ```
3. 启动开发服务器：
   ```bash
   npm run dev
   ```

### 4. 管理端配置与启动
1. 进入管理端目录：
   ```bash
   cd ../Admin
   ```
2. 安装依赖：
   ```bash
   npm install
   ```
3. 启动开发服务器：
   ```bash
   npm run dev
   ```

---

## 🛠️ 故障排除
- **数据库连接失败**：请确保 `.env` 中的 `MongoAtlasDBUrl` 正确，并且你的 IP 已在 MongoDB Atlas 的白名单中。
- **图片上传失败**：请检查 Cloudinary 的配置是否正确。
- **依赖冲突**：建议使用 Node.js LTS 版本。

## 📢 贡献
欢迎提交 Issue 或 Pull Request 来完善这个项目！
