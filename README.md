# myelectron

**Electron: 使用 JavaScript, HTML 和 CSS 构建跨平台的桌面应用**
 
 Electron 可以让你使用纯 JavaScript 调用丰富的原生(操作系统) APIs 来创造桌面应用。   
 你可以把它看作一个专注于桌面应用的 Node. js 的变体，而不是 Web 服务器。
 
- demo
  - Beautiful Cloud Drive Markdown NoteBook Desktop App: https://github.com/IceEnd/Yosoro

* github: https://github.com/electron/electron
* website: https://electronjs.org
* doc: https://electronjs.org/docs/tutorial/first-app


- install
```
  全局安装: npm install electron -g
  在项目中作为development dependency安装: npm install electron --save-dev
```

- Quick start
```
  git clone https://github.com/electron/electron-quick-start
  cd electron-quick-start
  npm install
  npm start
```

* start info
```
从开发的角度来看, Electron application 本质上是一个 Node. js 应用程序。 
应用启动的入口是一个与 Node.js 模块相同的 package.json 文件。 一个最基本的 Electron 应用一般来说会有如下的目录结构：

your-app/
  ├── package.json
  ├── main.js
  └── index.html

为你的新Electron应用创建一个新的空文件夹。 打开你的命令行工具，然后从该文件夹运行npm init

npm init

npm 会帮助你创建一个基本的 package.json 文件。 其中的 main 字段所表示的脚本为应用的启动脚本，它将会在主进程中执行。
如下片段是一个 package.json 的示例：

{
    "name": "your-app",
    "version": "0.1.0",
    "main": "main.js"
  }

注意：如果 main 字段没有在 package.json 中出现，那么 Electron 将会尝试加载 index.js 文件（就像 Node.js 自身那样）。
如果你实际开发的是一个简单的 Node 应用，那么你需要添加一个 start 脚本来指引 node 去执行当前的 package：

{
    "name": "your-app",
    "version": "0.1.0",
    "main": "main.js",
    "scripts": {
      "start": "node ."
    }
  }

把这个 Node 应用转换成一个 Electron 应用也是非常简单的，我们只不过是把 node 运行时替换成了 electron 运行时。

{
    "name": "your-app",
    "version": "0.1.0",
    "main": "main.js",
    "scripts": {
      "start": "electron ."
    }
  }
```
