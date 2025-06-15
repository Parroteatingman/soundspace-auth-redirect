# SoundSpace 邮箱验证重定向页面

这个页面用于处理 SoundSpace 应用的邮箱验证重定向。

## 部署到 Cloudflare Pages

1. 创建 GitHub 仓库
2. 上传这些文件到仓库
3. 在 Cloudflare Pages 中连接该仓库
4. 自动部署

## 文件说明

- `index.html` - 主要重定向页面
- `.well-known/apple-app-site-association` - iOS App Links 配置
- `.well-known/assetlinks.json` - Android App Links 配置

## 使用流程

1. 用户收到 Supabase 发送的邮箱验证邮件
2. 点击邮件中的链接（指向这个页面）
3. 页面自动跳转到 SoundSpace 应用
4. 应用完成邮箱验证流程