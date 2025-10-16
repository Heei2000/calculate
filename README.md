# 魏专属计算器

一个专为支付开发工程师设计的利润计算工具，支持多种部署方式。

## 项目简介

这是一个基于 Java Spring Boot 开发的利润计算器，同时提供了 GitHub Pages 静态版本，方便在不同场景下使用。

## 功能特性

- 💰 **利润计算**：支持多种利润计算模式
- 📊 **数据分析**：提供详细的计算结果和建议
- 🎨 **现代化UI**：响应式设计，支持移动端
- 🔒 **安全可靠**：输入验证和错误处理

## 部署方式

### 1. GitHub Pages 版本（推荐用于演示）

**优势：**
- ✅ 完全免费
- ✅ 自动部署
- ✅ HTTPS 支持
- ✅ 全球 CDN 加速
- ✅ 无需服务器维护

**访问地址：** https://heei2000.github.io/calculate/

**本地测试：**
```bash
# 启动本地服务器
python3 -m http.server 3000
# 访问 http://localhost:3000
```

### 2. Spring Boot 版本（用于生产环境）

**优势：**
- ✅ 完整后端功能
- ✅ 数据库支持
- ✅ API 接口
- ✅ 高并发处理
- ✅ 可扩展性强

**启动方式：**
```bash
# 开发环境
./mvnw spring-boot:run

# 生产环境
./mvnw clean package
java -jar target/demo-0.0.1-SNAPSHOT.jar
```

**外网访问（使用 ngrok）：**
```bash
# 启动 ngrok 隧道
./ngrok http 8081
```

## 技术栈

### 前端技术
- HTML5 + CSS3
- JavaScript (ES6+)
- 响应式设计
- 现代化 UI 组件

### 后端技术（Spring Boot 版本）
- Java 17
- Spring Boot 2.7+
- Maven 构建工具
- RESTful API

## 支付系统开发最佳实践

作为支付开发工程师，本项目展示了以下最佳实践：

### 1. 多环境部署策略
- **开发环境**：本地 Spring Boot + ngrok
- **演示环境**：GitHub Pages 静态版本
- **生产环境**：云服务器 + Nginx + SSL

### 2. 高可用性设计
- 前后端分离架构
- 静态资源 CDN 加速
- 容错处理和优雅降级

### 3. 安全性考虑
- HTTPS 强制加密
- 输入数据验证
- XSS 防护
- CSRF 保护

## 项目结构

```
demo/
├── src/main/java/           # Spring Boot 后端代码
├── src/main/resources/      # 配置文件和静态资源
├── index.html              # GitHub Pages 版本
├── pom.xml                 # Maven 配置
├── ngrok                   # ngrok 客户端
└── README.md              # 项目说明
```

## 快速开始

### 方式一：GitHub Pages（推荐新手）

1. 访问 https://heei2000.github.io/calculate/
2. 直接使用在线版本

### 方式二：本地开发

1. 克隆项目
```bash
git clone https://github.com/Heei2000/calculate.git
cd calculate
```

2. 启动 Spring Boot
```bash
./mvnw spring-boot:run
```

3. 启动 ngrok（可选）
```bash
./ngrok http 8081
```

## 支付开发工程师专用功能

- 🔢 **精确计算**：支持高精度数值计算，避免浮点数误差
- 📈 **性能监控**：内置性能指标监控
- 🛡️ **安全防护**：多层安全验证机制
- 🔄 **幂等性**：支持重复请求幂等处理
- 📊 **日志审计**：完整的操作日志记录

## 贡献指南

欢迎提交 Issue 和 Pull Request！

## 许可证

MIT License

## 联系方式

如有问题，请提交 Issue 或联系项目维护者。

---

**注意：** 本项目专为支付开发工程师设计，在生产环境使用时请确保遵循相关安全规范和合规要求。