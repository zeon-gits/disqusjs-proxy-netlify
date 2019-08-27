# disqusjs-proxy-netlify

一个使用 [Netlify](https://www.netlify.com/) 部署 Disqus API Proxy 的示例。

## 简介

Netlify 提供 Serverless 部署服务，支持包括静态网页、微服务等。在这里我们使用 Netlify 的重定向功能部署一个 Disqus API 的反代。

## 使用教程

[![Deploy to Netlify](https://www.netlify.com/img/deploy/button.svg)](https://app.netlify.com/start/deploy?repository=https://github.com/ysc3839/disqusjs-proxy-netlify) 👈点此直接部署

或
1. [使用此模板创建仓库](https://github.com/ysc3839/disqusjs-proxy-netlify/generate) (可以创建为私有仓库，不会影响 Netlify 的功能)。
2. [前往 Netlify 创建新项目](https://app.netlify.com/start)，根据提示登录 GitHub 账号并选择刚才创建的仓库。
3. 测试你的反代是否可以使用：访问你的反代域名，应该会跳转到 Disqus API 文档页面。
   > 因为直接访问 `https://disqus.com/api/` 便会跳转到 `https://disqus.com/api/docs/`。反代也会返回 3xx 状态码。
4. 修改你的服务中 Disqus API Endpoint 的配置；如果你正在使用 [DisqusJS](https://github.com/SukkaW/DisqusJS)，这个配置是 DisqusJS 中的 `api` 字段。

## 注意事项

- Netlify 提供免费的 Plan，但是有每月 100GB 的流量限制
