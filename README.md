## 说明
此版本是在`layDate 5.0.85`版本上进行修改的。
1. 增加了时间过滤日期的功能。参数如下：
```js
laydate.render({
    elem: '#test1',
    value: '2017-11-30',
    min: '2017-11-10',
    max: '2017-11-20',
    uselessDate: {                      // 增加了配置字段
        list: ['2017-11-11', '2017-11-13', '2017-11-15']  // 过滤时间列表
    },
    done: function (data) {
        alert(data)
    }
});
```

2. 增加了选择最近的功能。参数如下：
```js
laydate.render({
    elem: '#test1',
    value: '2017-11-30', //必须遵循format参数设定的格式
    min: '2017-11-10',
    max: '2017-11-20',
    uselessDate: {
        list: ['2017-11-11', '2017-11-13', '2017-11-15']
    },
    btns: ['last'],         // 增加了配置属性 last, 事件钩子同样适用，注意：一定要配合max和min参数一起使用
    done: function (data) {
        alert(data)
    }
});
```
注意：一定要配合max和min参数一起使用

## 概要
全面重写的 layDate 包含了大量的更新，其中主要以：年选择器、年月选择器、日期选择器、时间选择器、日期时间选择器 五种类型的选择方式为基本核心，并且均支持范围选择（即双控件）。内置强劲的自定义日期格式解析和合法校正机制，含中文版和国际版，主题简约却又不失灵活多样。由于内部采用的是零依赖的原生 JavaScript 编写，因此又可作为独立组件使用。毫无疑问，这是 layui 的虔心之作。

## 官网
[http://www.layui.com/laydate/](http://www.layui.com/laydate/)

## 相关
[文档](http://www.layui.com/doc/modules/laydate.html)、[社区](http://fly.layui.com)