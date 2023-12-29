# BingAI-GPT

一个基于 [ChatGPT-API Demo](https://github.com/anse-app/chatgpt-demo) 二改的程序。

**🍿 在线预览**: https://chat.bing.ecylt.top

二改版本优势：
1. **无需API Key**
2. **国内外服务器均可搭建，无需接口代理**
3. **使用BingAI接口，免费使用GPT-4**

## 本地运行

### 前置环境

1. **Node**: 检查您的开发环境和部署环境是否都使用 `Node v18` 或更高版本。你可以使用 [nvm](https://github.com/nvm-sh/nvm) 管理本地多个 `node` 版本。
   ```bash
    node -v
   ```
2. **PNPM**: 我们推荐使用 [pnpm](https://pnpm.io/) 来管理依赖，如果你从来没有安装过 pnpm，可以使用下面的命令安装：
   ```bash
    npm i -g pnpm
   ```

### 起步运行

1. 安装依赖
   ```bash
    pnpm install
   ```
2. **此项我们已经帮你修改好了，如二次开发则请重新检测此项的设置**
   复制 `.env.example` 文件，重命名为 `.env`，并随便填写一个 [OpenAI API key](https://platform.openai.com/account/api-keys) 到 `.env` 文件中
   ```bash
    OPENAI_API_KEY=114514
   ```
   修改 `OPENAI_API_BASE_URL` 为 `https://bing.ecylt.top`
   ``` bash
    OPENAI_API_BASE_URL=https://bing.ecylt.top
   ```
3. 运行应用，本地项目运行在 `http://localhost:3000/`
   ```bash
    pnpm run dev
   ```

## 部署

### 部署在 Vercel

[![Deploy with Vercel](https://vercel.com/button)](https://vercel.com/new/clone?repository-url=https://github.com/WZH-Team/BingAI-GPT)



> ###### 🔒 需要站点密码？
>
> 携带[`SITE_PASSWORD`](#environment-variables)进行部署

## 常见问题

Q: TypeError: fetch failed (can't connect to OpenAI Api)

A: 配置环境变量 `HTTPS_PROXY`，参考：https://github.com/ddiu8081/chatgpt-demo/issues/34

Q: throw new TypeError(${context} is not a ReadableStream.)

A: Node 版本需要在 `v18` 或者更高，参考：https://github.com/ddiu8081/chatgpt-demo/issues/65

Q: Accelerate domestic access without the need for proxy deployment tutorial?

A: 你可以参考此教程：https://github.com/ddiu8081/chatgpt-demo/discussions/270

## 参与贡献

这个项目的存在要感谢所有做出贡献的人。

感谢我们所有的支持者！🙏

## 支持我们

[爱发电](https://afdian.net/a/wxs7655)

## License

原作者MIT © [ddiu8081](https://github.com/ddiu8081/chatgpt-demo/blob/main/LICENSE)
```
MIT License

Copyright (c) 2023 Diu

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```