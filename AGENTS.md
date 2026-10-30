# 项目技术上下文

## 项目类型
纯静态 HTML 项目（Mise 运行时策略）

## 技术栈
- 无框架、无构建工具
- 单一入口：Index.html
- 开发服务器：http-server (Node.js)

## 运行命令
- 安装依赖：`mise run install`
- 开发预览：`mise run dev`（端口 3015）
- 构建：`mise run build`（静态项目无需构建）

## 部署配置
- 模式：static
- 输出目录：.（当前目录）

## 注意事项
- 项目为纯静态 HTML，无 CSS/JS 资源文件
- Index.html 引用了相对路径的 CSS 文件（index_files/），但这些文件不存在于项目中
- 页面可能缺少样式支持
