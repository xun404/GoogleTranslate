<p align="center">
  <a href="https://github.com/xun404/GoogleTranslate">
    <img alt="Google Translate" src="https://cdn.jsdelivr.net/gh/xun404/GoogleTranslate@main/.readme/5b38a1b1dcc25.png" width="600">
  </a>
</p>

<p align="center">
  <a href="https://github.com/xun404/GoogleTranslate/releases"><img alt="GitHub release" src="https://img.shields.io/github/release/xun404/GoogleTranslate.svg?style=for-the-badge"></a>
  <a href="https://travis-ci.org/xun404/GoogleTranslate"><img alt="Build Status" src="https://img.shields.io/travis/xun404/GoogleTranslate/dev.svg?style=for-the-badge"></a>
  <a href="./LICENSE"><img alt="LICENSE GPL" src="https://img.shields.io/badge/license-gpl-yellow.svg?style=for-the-badge"></a>
  <a href="https://github.com/prettier/prettier"><img alt="Code Style: Prettier" src="https://img.shields.io/badge/code_style-prettier-ff69b4.svg?style=for-the-badge"></a>
</p>

> 🌐 Google 翻译 Mac 客户端（这是 2.1 版本的分支）

> 🥸 原仓已经很久没有更新，这里是 fork 仓，只要解决一些 BUG。

## 状态：公测版

所有已知问题都已经修复，并优化了用户体验，但可能依然有少量 BUG。  
如果你在使用中发现了问题，请在[这里](https://github.com/xun404/GoogleTranslate/issues/new)报告问题，非常感谢！

## 预览

<img alt="预览动态图" src="https://cdn.jsdelivr.net/gh/xun404/GoogleTranslate@main/.readme/5b4dfbda30200.gif" width="420">
<img alt="更改语言" src="https://cdn.jsdelivr.net/gh/xun404/GoogleTranslate@main/.readme/5b4dfc253a5d7.png" width="420">
<img alt="应用程序设置" src="https://cdn.jsdelivr.net/gh/xun404/GoogleTranslate@main/.readme/5b4dfc25357a1.png" width="420">

## 功能

- [x] 基本翻译
- [x] 语音朗读
- [x] 顶端显示
- [x] 开机启动
- [x] ~~自动更新~~
- [x] 全局快捷键呼出
- [x] 内置多种翻译引擎

> 主要计划解决的问题

- [ ] 修复失效接口，目前百度和有道接口均失效，将改为直接调用官方接口。
- [ ] 谷歌接口替换为直接调用，不在过代理层。
- [ ] 修复交互逻辑 bug。

## 下载

您可以在[这里](https://github.com/xun404/GoogleTranslate/releases/latest)手动下载最新版本

## FAQ

Q：Electron 不是跨平台的吗？为什么只有 Mac 版本？  
A：因为 UI 的交互设计不适用于其他操作系统

Q：为什么不能自动更新？  
A：因为我没有加入 [Apple Developer Program](https://developer.apple.com/programs/)（需要缴纳年费），无法进行[代码签名](https://electronjs.org/docs/tutorial/code-signing)，所以无法使用自动更新功能

Q：所有翻译引擎都提示当前翻译接口不可用？  
A：在新版本中，无论你使用哪种翻译引擎，都会先调用国内谷歌翻译的检测语言接口。出现这种情况一般是你的代理节点出现流量异常，导致请求被谷歌拦截，需要输入验证码（你还可以使用 <kbd>option</kbd> + <kbd>command</kbd> + <kbd>I</kbd> 打开调试工具查看请求结果是否正确）所以如果出现这个问题，请更换你的代理节点或不使用代理直接使用国内谷歌引擎。

Q：无法打开应用，提示该应用来自身份不明的开发者？  
A：在终端中输入 `sudo spctl –master-disable` 然后按回车确认，密码是系统开机密码。  
然后打开系统偏好设置 ⇨ 安全性和隐私 ⇨ 任何来源，勾选即可。

## 参与贡献

1.  Fork it!
2.  将自己添加为贡献者：`npm run contributors`
3.  创建功能分支：`git checkout -b my-new-feature`
4.  提交你的更改：`git commit -am 'Add some feature'`
5.  推送这个分支：`git push origin my-new-feature`
6.  提交一个拉取请求 :D

## 贡献者

感谢这些美好的人 ([emoji key](https://github.com/kentcdodds/all-contributors#emoji-key)):

<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
<!-- prettier-ignore-start -->
<!-- markdownlint-disable -->
<table>
  <tr>
    <td align="center"><a href="https://qwq.cat"><img src="https://avatars2.githubusercontent.com/u/20062482?v=4?s=100" width="100px;" alt=""/><br /><sub><b>さくら</b></sub></a><br /><a href="https://github.com/MoeFE/GoogleTranslate/commits?author=u3u" title="Code">💻</a> <a href="https://github.com/MoeFE/GoogleTranslate/commits?author=u3u" title="Documentation">📖</a> <a href="#design-u3u" title="Design">🎨</a> <a href="#ideas-u3u" title="Ideas, Planning, & Feedback">🤔</a></td>
    <td align="center"><a href="https://github.com/Batur24"><img src="https://avatars1.githubusercontent.com/u/9591690?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Batur</b></sub></a><br /><a href="#question-Batur24" title="Answering Questions">💬</a> <a href="https://github.com/MoeFE/GoogleTranslate/issues?q=author%3ABatur24" title="Bug reports">🐛</a> <a href="#ideas-Batur24" title="Ideas, Planning, & Feedback">🤔</a> <a href="https://github.com/MoeFE/GoogleTranslate/commits?author=Batur24" title="Tests">⚠️</a></td>
    <td align="center"><a href="https://github.com/mantou132"><img src="https://avatars3.githubusercontent.com/u/3841872?v=4?s=100" width="100px;" alt=""/><br /><sub><b>mantou</b></sub></a><br /><a href="https://github.com/MoeFE/GoogleTranslate/commits?author=mantou132" title="Code">💻</a> <a href="#ideas-mantou132" title="Ideas, Planning, & Feedback">🤔</a></td>
    <td align="center"><a href="https://rmbz.net/"><img src="https://avatars.githubusercontent.com/u/10024821?v=4?s=100" width="100px;" alt=""/><br /><sub><b>I'm xun.</b></sub></a><br /><a href="https://github.com/MoeFE/GoogleTranslate/issues?q=author%3Axun404" title="Bug reports">🐛</a> <a href="https://github.com/MoeFE/GoogleTranslate/commits?author=xun404" title="Code">💻</a> <a href="https://github.com/MoeFE/GoogleTranslate/commits?author=xun404" title="Documentation">📖</a></td>
  </tr>
</table>

<!-- markdownlint-restore -->
<!-- prettier-ignore-end -->

<!-- ALL-CONTRIBUTORS-LIST:END -->

该项目遵循 [all-contributors](https://github.com/kentcdodds/all-contributors) 规范，欢迎任何形式的贡献！

## 协议

[GNU General Public License v3.0](./LICENSE)  
本项目仅供学习交流和私人使用，禁止商业用途

> [qwq.cat](https://qwq.cat) · GitHub [@u3u](https://github.com/u3u) · Twitter [@hanser0v0](https://twitter.com/hanser0v0)
