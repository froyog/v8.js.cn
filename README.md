# v8.js.cn [![Build Status](https://travis-ci.com/justjavac/v8.js.cn.svg?branch=master)](https://travis-ci.com/justjavac/v8.js.cn)

本仓库是 [v8.dev, V8 官方网站](https://v8.dev) 的中文翻译。

所有文章的原始版权归原文章作者所有，文中提到的 V8 的 logo 和商标归 Google 所有。

## 本地安装

1. 克隆本仓库 `git clone https://github.com/justjavac/v8.js.cn.git`
1. 进入项目目录 `cd v8.js.cn`
1. 使用[期望](https://github.com/justjavac/v8.js.cn/blob/master/.nvmrc)的 Node.js 版本 `nvm use`
1. 安装依赖包 `npm install`

运行 `npm run` 可以查看支持的脚本。一些常用的脚本：

- `npm run build` 构建网站并输出到 `dist`.
- `npm run watch` 构建网站并输出到 `dist`，然后监听文件的更改
- `npm start` 启动一个本地 HTTP server

`npm run` 会触发某些 Unix 风格的命令。如果你正在 Windows 系统中使用类 linux 风格的环境，例如 git bash、msys2 或者 Cygwin，可以修改 npm 的配置文件以使用 linux 终端。如果你没有配置，那么默认使用的是 `cmd.exe`。下面是一个修改配置的例子：

```sh
npm config set script-shell "C:\\Program Files\\git\\bin\\bash.exe"
```

或者：

```sh
npm config set script-shell "C:\\msys64\\usr\\bin\\sh.exe"
```

## 参与翻译

当你翻译完一篇文章后，请在 markdown 文件的 meta 信息中添加译者信息。格式如下：

```yml
cn:
  author: '迷渡 ([@justjavac](https://github.com/justjavac))，会写代码'
  avatars:
    - justjavac
  tweet: 'xxxxxx'
```

以上内容都是可选的。

如果你想展示头像，那么你需要在 `src/_img/avatars/` 放 2 张 `.jpg` 格式的图片。尺寸为：

- `file-name.jpg` 96 * 96
- `file-name@2x.jpg` 192 * 192

推荐：当你决定翻译某篇文章时，你应该 fork 本仓库，然后新建一个语义明确的分支，然后向本仓库马上发起一个 [Pull Request](https://github.com/justjavac/v8.js.cn/pulls)，在标题中使用 `WIP` 开头，以标识这是一个 Work In Progress 工作。之所以马上提交一个 pr 也是为了防止不同的开发者翻译了同一个文件。

## 注意事项

1. 请注意中英文标点的使用
2. 英文单词和中文直接保留一个空格
3. 由于 markdown 格式对中文的解析不够友好，因此需要手动在标题后面标注上锚点链接（参考：[src/blog/v8-release-71.md](src/blog/v8-release-71.md)）
