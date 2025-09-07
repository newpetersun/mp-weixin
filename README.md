# PeterSun 个人项目展示平台

PeterSun是一个基于uni-app开发的跨平台个人作品展示应用，支持微信小程序、H5和App等多个平台，主要用于展示个人项目、技术栈和联系方式等信息。

## 在线演示

![小程序演示](https://github.com/newpetersun/mp-weixin/blob/master/static/xcx.jpg)

## 项目概述

本项目是一个个人作品展示平台，具有前台展示和后台管理两个部分。前台主要展示个人信息、项目案例、技术栈和联系方式等；后台管理系统支持用户管理、项目管理、数据统计分析等功能。

## 功能特点

### 前台功能

- **个人信息展示**：展示用户基本信息、技术栈、联系方式等
- **项目展示**：展示个人开发的项目案例，支持图片轮播、项目分类和详情查看
- **数据可视化**：包括客户分布地图和访问统计图表
- **联系功能**：提供多种联系方式和留言功能

### 后台管理

- **用户管理**：管理用户信息、权限设置
- **项目管理**：管理项目信息、分类、图片等
- **数据分析**：访问统计、地理分布、热门页面等数据分析
- **系统设置**：系统参数配置、技术栈管理等

## 技术架构

- **前端框架**：uni-app（Vue.js）
- **图表库**：ECharts（用于数据可视化）
- **UI组件**：自定义UI组件
- **后端接口**：RESTful API（配套PHP后端）
- **数据通信**：基于Promise的HTTP请求封装

## 项目结构

```
petersun/
├── components/              # 公共组件
│   ├── FloatingButtons.vue  # 浮动按钮组件
│   └── Loading.vue          # 加载组件
├── config/                  # 配置文件
│   └── config.js            # 项目配置（API地址、静态资源等）
├── pages/                   # 页面文件
│   ├── admin/               # 后台管理页面
│   ├── contact/             # 联系页面
│   ├── index/               # 首页及组件
│   ├── project/             # 项目详情页
│   ├── projects/            # 项目列表页
│   └── splash/              # 启动页
├── static/                  # 静态资源
│   ├── images/              # 图片资源
│   └── svg/                 # SVG图标
├── uni_modules/             # uni-app模块
│   └── qiun-data-charts/    # 图表组件
├── utils/                   # 工具类
│   └── api.js               # API接口封装
├── App.vue                  # 应用入口组件
├── main.js                  # 应用入口文件
├── manifest.json            # 应用配置文件
├── pages.json               # 页面配置文件
├── uni.scss                 # 全局样式变量
└── package.json             # 项目依赖配置
```

## 技术特点

1. **跨平台兼容**：使用uni-app实现一次开发，多端发布（H5、小程序、App等）
2. **模块化设计**：API接口统一管理，组件化开发
3. **响应式布局**：适配不同屏幕尺寸
4. **数据可视化**：集成ECharts实现地图和统计图表展示
5. **用户体验优化**：加载状态、过渡动画等提升体验

## 环境配置

项目支持开发和生产两种环境配置，通过`config.js`进行管理：

- **开发环境**：调试模式开启，接口地址配置为开发服务器
- **生产环境**：调试模式关闭，接口地址配置为生产服务器

## 安装与使用

### 环境要求

- Node.js (v12+)
- HBuilderX (推荐使用)
- 微信开发者工具 (小程序开发时需要)

### 安装步骤

1. 克隆项目到本地
   ```bash
   git clone [repository-url]
   cd petersun
   ```

2. 安装依赖
   ```bash
   npm install
   ```

3. 使用HBuilderX打开项目
   - 导入项目到HBuilderX
   - 配置项目运行参数

4. 运行项目
   - 在HBuilderX中选择运行到浏览器/小程序/模拟器
   - 或使用命令行 `npm run dev`

## 部署

### 微信小程序

1. 在HBuilderX中选择"发行" -> "小程序-微信"
2. 生成小程序代码
3. 在微信开发者工具中上传代码并提交审核

### H5版本

1. 在HBuilderX中选择"发行" -> "网站-H5"
2. 将生成的dist目录下的文件部署到Web服务器

## API接口

项目中的API接口统一通过`utils/api.js`进行管理，主要包括：

- 用户信息接口
- 项目相关接口
- 联系相关接口
- 访问统计接口
- 后台管理接口

## 项目展示特性

- 支持项目图片左右滑动切换
- 客户分布地理数据可视化
- 访问统计图表展示
- 响应式布局适配各种设备

## 贡献

欢迎贡献代码或提出建议，请遵循以下步骤：

1. Fork本仓库
2. 创建您的特性分支 (`git checkout -b feature/amazing-feature`)
3. 提交您的更改 (`git commit -m 'Add some amazing feature'`)
4. 推送到分支 (`git push origin feature/amazing-feature`)
5. 开启一个Pull Request

## 许可证

[MIT License](LICENSE)

## 联系方式

如有问题或建议，请通过以下方式联系：

- 项目作者：PeterSun
- 网站：https://www.sundongliang.cn
