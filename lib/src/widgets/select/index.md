---
widget: select
title: 选择器
---

类似 Select2 的选择器。

## `widget` 自定义属性

参数 | 说明 | 类型 | 默认值
----|------|-----|------
allowClear | 支持清除 | `boolean` | `false`
autoFocus | 默认获取焦点 | `boolean` | `false`
dropdownClassName | 下拉菜单的 className 属性 | `string` | -
dropdownMatchSelectWidth | 下拉菜单和选择器同宽 | `boolean` | `true`
dropdownStyle | 下拉菜单的 style 属性 | `object` | -
serverSearch | 是否使用服务端搜索，当为 true 时，将不再在前端对 nz-option 进行过滤 | `boolean` | `false`
filterOption | 是否根据输入项进行筛选。当其为一个函数时，会接收 `inputValue` `option` 两个参数，当 `option` 符合筛选条件时，应返回 `true`，反之则返回 `false`。 | `(input?: string, option?: NzOptionComponent) => boolean;` | -
maxMultipleCount | 最多选中多少个标签| `number` | `Infinity`
mode | 设置 nz-select 的模式 | `multiple,tags,default` | `default`
notFoundContent | 当下拉列表为空时显示的内容 | `string` | -
showSearch | 使单选模式可搜索 | `boolean` | `false`
searchChange | 搜索内容变化回调函数，参数为搜索内容，必须返回 `Promise` 对象 | `Function` | -
openChange | 下拉菜单打开关闭回调函数 | `Function` | -
scrollToBottom | 下拉菜单滚动到底部回调，可用于作为动态加载的触发条件 | `Function` | -

## Demo

**基础**

```json
"type": {
    "type": "string",
    "title": "类型",
    "default": "tom",
    "widget": {
        "id": "select",
        "data": [
            { "value": "jack", "label": "Jack" },
            { "value": "lucy", "label": "Lucy" },
            { "value": "tom", "label": "Tom", "disabled": true }
        ]
    }
}
```
