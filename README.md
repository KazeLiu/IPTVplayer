# 悦视

## 项目简介

这是一个基于 Tauri 2 和 Vue 3 开发的现代化电视流媒体播放器应用。支持通过 M3U 地址和 EPG 地址自动解析和播放直播流。

## 截图
![QQ20241206-171020.png](readImage%2FQQ20241206-171020.png)
![QQ20241206-171005.png](readImage%2FQQ20241206-171005.png)
![QQ20241206-171123.png](readImage%2FQQ20241206-171123.png)
![QQ20241206-171129.png](readImage%2FQQ20241206-171129.png)
![QQ20241206-171200.png](readImage%2FQQ20241206-171200.png)

## 使用方法
1. 自己在网上找 M3u 订阅地址
2. 自己在网上找 EPG 订阅地址
3. 点击卡片开始看电视

## 警告
程序是 alpha 版本，可能存在一些问题，请按流程使用，不要尝试其他的动作（例如卡住了就F5刷新，暂时还没有屏蔽这种按钮）。

## 技术栈

- **前端**: Vue 3, Vite
- **桌面框架**: Tauri 2
- **UI 组件**: Element Plus
- **状态管理**: Pinia
- **样式**: Tailwind CSS

## 功能特性

- 输入 M3U 地址自动解析频道列表
- 支持 EPG 节目指南
- 跨平台桌面应用
- 响应式设计

## 预想功能

- [x] 能添加单个频道
- [x] 频道能分组
- [ ] 使用DynamicScroller解决列表卡顿
- [x] 能同时播放多个频道
- [x] 能全屏播放，且在全屏播放下有界面
- [ ] 特定的台如果源有问题直接访问网站来播放
- [ ] 添加源的有效性检测
- [ ] 录制节目
- [ ] 屏幕截图
- [ ] 读取音频流添加字幕&翻译
- [ ] 界面更好看
- [ ] IPv6和IPv4的判定

## 开源致谢

感谢以下开源项目和库的贡献：

### 框架和开发工具

- [Tauri](https://tauri.app/) - 使用 Web 前端构建轻量级跨平台桌面应用
- [Vue.js](https://vuejs.org/) - 渐进式 JavaScript 框架
- [Vite](https://vitejs.dev/) - 高性能前端构建工具
- [Pinia](https://pinia.vuejs.org/) - Vue 状态管理库

### UI 和样式

- [Element Plus](https://element-plus.org/) - Vue 3 组件库
- [Tailwind CSS](https://tailwindcss.com/) - 实用优先的 CSS 框架
- [Font Awesome](https://fontawesome.com/) - 图标库

### 媒体处理

- [hls.js](https://github.com/video-dev/hls.js) - HLS 流媒体播放库
- [m3u8-parser](https://github.com/videojs/m3u8-parser) - M3U8 解析工具
- [epg-parser](https://github.com/freearhey/epg-parser) - EPG 数据解析库

### 网络和数据请求

- [Axios](https://axios-http.com/) - 基于 Promise 的 HTTP 客户端
- [Reqwest](https://github.com/seanmonstar/reqwest) - Rust HTTP 客户端

### 开发和构建工具

- [Rust](https://www.rust-lang.org/) - 系统编程语言
- [PostCSS](https://postcss.org/) - CSS 转换工具
- [Sass](https://sass-lang.com/) - CSS 预处理器

## 未来贡献者

我们预留了特别的感谢位置，期待未来更多优秀的贡献者加入！

## 特别感谢

在前期不熟练的开发中，碰到的坑，感谢他们帮我解决

- [目棃](https://github.com/BTMuli)
- [Goodjooy](https://github.com/Goodjooy)

## 免责声明
本程序仅供个人学习和研究使用。程序的开发初衷是为帮助开发者学习 Tauri 2 框架，并提升个人技术水平。程序并不意图侵犯任何版权或其他合法权益。如果您在使用过程中发现任何版权问题或侵犯了他人合法权益，请立即停止使用，并告知我们，我们将采取适当的措施。

我们对程序中的内容、服务和第三方资源的合法性、准确性、完整性不作任何保证。用户在使用本程序时应自行承担相关风险，开发者不承担因此产生的任何法律责任。

本程序不用于商业用途，并且不含任何恶意软件或广告。

## 许可证

MIT

## 开发

```bash
# 安装依赖
npm install

# 开发模式
npm run dev

# 构建应用
npm run tauri build
```

## 贡献

欢迎通过 Issue 和 Pull Request 参与贡献！

*项目持续建设中，感谢每一位开源贡献者！*