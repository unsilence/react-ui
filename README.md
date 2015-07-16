

A collection of components for React.
文档 [戳这里](http://lobos.github.io/react-ui/)

# 使用

 - 直接引用

[在线生成需要的组件](http://lobos.github.io/react-ui/#/build)，在页面中引用即可。（注意需要先引用 react-with-addons 和 [es5-shim](https://github.com/es-shims/es5-shim)）
```
<script src="js/es5-shim.min.js"></script>
<script src="js/react-with-addons.js"></script>
<script src="js/ReactUI.js"></script>
```

 - npm install
```
npm install rctui
```
```
var ReactUI = require('rctui')
var Form = ReactUI.Form
...
// 或者单独使用一个组件
var Input = require('rctui/input')
var CheckboxGroup = require('rctui/checkbox-group')
```

# build
使用 [webpack](http://webpack.github.io/) 打包，可以修改 'src/js/index.js' 自定义需要的组件。
```
docs:    webpack --config webpack-docs.config.js [--min]
```

# Components
目前完成的组件，后续应该会不断加入新的组件

- [Button](http://lobos.github.io/react-ui/#/button)
- [Checkbox](http://lobos.github.io/react-ui/#/checkbox)
- [Checkbox group](http://lobos.github.io/react-ui/#/checkbox-group)
- [Datetime](http://lobos.github.io/react-ui/#/datetime)
- [Form](http://lobos.github.io/react-ui/#/form)
- [Form Control](http://lobos.github.io/react-ui/#/form-control)
- [Icon](http://lobos.github.io/react-ui/#/icon)
- [Loading](http://lobos.github.io/react-ui/#/loading)
- [Message](http://lobos.github.io/react-ui/#/message)
- [Pagination](http://lobos.github.io/react-ui/#/pagination)
- [Radio group](http://lobos.github.io/react-ui/#/radio-group)
- [Rating](http://lobos.github.io/react-ui/#/rating)
- [Select](http://lobos.github.io/react-ui/#/select)
- [Tree](http://lobos.github.io/react-ui/#/tree)

# Change log
v0.2.3

 - 修改一些小bug
 - [增加在线build](http://lobos.github.io/react-ui/#/build)

v0.2.2

 - 使用webpack打包，减少体积，去除了 `Reflux` 和 `superagent` 依赖。
 - 放弃bootstrap，使用yahoo/pure。
 - 在webpack中使用了`babel-loader`，所以用了部分es6语法，参考 [babel](https://babeljs.io/docs/learn-es2015/) 的文档，没有使用需要 polyfill 支持的部分（因为需要额外引入45KB左右的 polyfill 包）。不要忘记在页面中加入 [es5-shim](https://github.com/es-shims/es5-shim) 引用。

