## Easy Mock Group CLI

[![npm version](https://img.shields.io/npm/v/easy-mock-group-cli.svg?style=flat-square)](https://www.npmjs.com/package/easy-mock-group-cli)
Easy Mock Module CLI 是一个基于 [Easy Mock CLI](https://github.com/easy-mock/easy-mock-cli) 的修改, 按照文件夹分组生成 `API` 调用文件的命令行工具。
如果你正在使用 Easy Mock 伪造接口数据，那一定不要错过 Easy Mock CLI。

## 原链接和说明文档

- [Documentation](https://easy-mock.github.io/easy-mock-cli/)

## 安装

```bash
npm install -g easy-mock-module-cli
```

## 使用

1. 在 package.json 中的 scripts 区域, 加入:

```json
"toceanmock": "toceanmock init"
```

2. 原配置文件.easymockrc.json 中, projects 配置项中只需要配置 easy-mock 的项目 id, 例如:

```json
{
  "host": "http://devos.toceansoft.com:7300",
  "output": "src/api",
  "template": "axios",
  "projects": [
    {
      "id": "5d146c6b3505c600844d1a74",
      "name": "devos"
    },
    {
      "id": "5d15e4423505c600844d1c72",
      "name": "devos2"
    }
  ]
}
```

3. 执行:

```cmd
toceanmock init
```

4、增强功能

- 支持后台多项目多模块安排 api
- 把 js 改成 ts 风格 api
- 支持同时安装官方 cli（你可以保留 easymock init）
- 改进了https://github.com/liuyingqq123/easy-mock-group-cli 生成多个 instance.js 文件的冗余和对修改造成的工作量问题

5、改进

- 作者：narci2010@qq.com
- 建议和意见：由于作者比较忙，有好的建议和意见，麻烦发邮件或者在本项目中提 issue。
