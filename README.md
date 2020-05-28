# umi project

这是一个用来验证 umi issue 问题的包

> https://github.com/umijs/umi/issues/4780

yarn 安装阶段就会出错，提示 umi general temp 失败，把 src/pages/test/model.js 改名为其他名称（如 modal.js）后才能继续。

恢复 model.js 名称，执行 umi dev ，还是报错，改名为其他名称（如 modal.js）后，umi dev 正常

实际上，如果在 pages 目录下如果有 model.js 文件，model.js 文件中又含有 jsx 语法，umi 的几乎所有命令都报错，甚至 umi -v 也报错，并且报错信息没有任何实质性的帮助。

## Getting Started

Install dependencies,

```bash
$ yarn
```

Start the dev server,

```bash
$ yarn start
```
