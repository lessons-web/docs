# 前端开发规范

## 工具篇

### 开发环境必备

 - [Node.js](https://nodejs.org/en) 最好 18.0.0 以上的稳定版本。

 - npm：跟随 Nodejs 即可。

### IDE

统一使用 [VSCode](https://code.visualstudio.com/) 进行代码开发。

### 浏览器

统一使用 [Google Chrome](https://www.google.com/chrome/) 浏览器进行代码预览。

### 安装包

统一使用 `yarn` 进行安装包安装。

```bash
npm install -g yarn
```

### 版本管理工具

代码版本统一使用 Git 进行管理，详细可以查看 [Git 使用文档](../git/README.md)。

## 代码开发规范

### 技术栈

技术栈统一使用 Vite + React.js + React-Router-Dom [+ 状态管理] 进行开发。相关文档：

 - [React.js](https://react.dev/)

 - [Vite](https://vitejs.dev/)

 - [React-Router-Dom](https://reactrouter.com/)

 - 状态管理: 状态管理视项目复杂度而定，并不一定必须选择项目管理，如果选择可以使用如下几种方案
    
    - [valito](https://valtio.pmnd.rs/)
    
    - [zustand](https://zustand-demo.pmnd.rs/)

> 关于状态管理不选择 `redux` 以及周边生态的原因，因为在 Hooks 时代，`redux` 过于臃肿，带来的项目复杂度升高，维护成本也随之提高，不利于协同开发。

### 代码规范

代码规范是团队协同开发最重要的一个环节，一个良好的代码开发习惯能够让团队所有人收益成长，并且让团队的代码变得容易维护方便管理，是一个双方都受益的约束条件。关于代码规范，简单列举如下几点：

#### Typescript

#### Eslint

#### Prettier

#### Commitlint

### CSS 规范

之所以将 CSS 规范单独列出来讲，是因为 React.js 社区有很多优秀的 CSS 技术方案，他们之间各有优劣并且没有统一的标准来区分到底孰好孰坏，因此这里简单罗列一下并给出个人建议：

#### CSS Basic Rule

#### Less/Scss Module

#### Styled Components

#### Tailwind CSS

关于上述开发规范，各人有如下建议：

- Web PC 中后台模式化页面较多的场景，无需太多自定义样式代码编写的，可以统一使用 UI 框架 + `styled-components` 的技术方案，比如 `ant-design + styled-components`。

- H5 或者自定义样式较多的场景，统一使用 Tailwind CSS 的技术方案，这样能最大的保证代码灵活性。

> 当然，上述的技术方案只是地基，最后整个项目的完整性还是要依靠开发者自身的熟练度以及代码规范来保持的。