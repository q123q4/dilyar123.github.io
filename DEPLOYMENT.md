# 项目部署说明

本项目已准备好部署到GitHub，包含前后端完整代码结构。

## 项目结构

```
github/
├── README.md           # 项目说明文档
├── .gitignore          # Git忽略文件配置
├── frontend/           # 前端代码
│   ├── package.json    # 前端依赖配置
│   ├── vite.config.js  # Vite构建配置
│   └── src/            # 前端源代码
└── backend/            # 后端代码
    ├── package.json    # 后端依赖配置
    ├── app.js          # Express应用配置
    ├── server.js       # 服务器入口
    ├── controllers/    # 控制器
    ├── models/         # 数据模型
    ├── routes/         # 路由配置
    ├── middlewares/    # 中间件
    ├── config/         # 配置文件
    └── uploads/        # 文件上传目录
```

## 部署步骤

### 1. 创建GitHub仓库

在GitHub上创建一个新的仓库，然后将本目录下的所有文件上传到该仓库。

### 2. 安装依赖

#### 前端依赖安装
```bash
cd frontend
npm install
```

#### 后端依赖安装
```bash
cd backend
npm install
```

### 3. 配置环境变量

在后端目录下创建`.env`文件，配置必要的环境变量。

### 4. 构建前端项目

```bash
cd frontend
npm run build
```

### 5. 启动服务

```bash
cd backend
npm start
```

## 注意事项

1. 确保Node.js版本兼容（推荐Node.js 14+）
2. 数据库连接配置需要根据实际环境调整
3. 文件上传目录需要确保有写入权限
4. 部署前请删除不必要的测试文件
