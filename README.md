# OCI Start 部署指南

## 系统要求
- JDK 8 或更高版本
- 支持 Debian/Ubuntu 系统

## 在 Render 上部署

1. 在 Render 平台上创建新的 Web Service
2. 选择 "Build and deploy from a Git repository"
3. 连接您的 Git 仓库
4. 使用以下配置：
   - Environment: Docker
   - Plan: Free
   - Build Command: 已在 render.yaml 中配置
   - Start Command: 已在 render.yaml 中配置

## 使用方法

部署完成后，您可以使用以下命令：

- 启动应用程序：`./oci-start.sh start`
- 停止应用程序：`./oci-start.sh stop`
- 重启应用程序：`./oci-start.sh restart`
- 更新到最新版本：`./oci-start.sh update`
- 完全卸载应用：`./oci-start.sh uninstall`

## 注意事项

- 新版本会检测安装 Redis，如果之前安装了 Redis 可能会有影响
- 确保系统有足够的磁盘空间和内存 