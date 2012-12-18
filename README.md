# Popup

---

Popup 是可触发的浮层组件。封装了当用户点击、hover、focus 到指定元素时，可以触发另一个浮层显示的行为。

---

## 配置说明

### element `element|string`

弹出的浮层元素。也可以使用 template 参数传递模板来代替这个参数。

### trigger `element|string`

触发元素。

### triggerType `string`

触发类型，可选[hover|click|focus]，默认为 hover。

### effect `string`

基础的动画效果，可选[fade|slide]，默认为空。fade 和 slide 可以并行。

### duration `number`

动画时长，默认 250 毫秒。

### delay `number`

延迟 hover 触发显示的时长，默认 70 毫秒。

### disabled `boolean`

是否能触发弹出效果，可用`.set('disabled', true)`进行开关。


> 若有范例和演示中有其他参数（如 align），请参见 Popup 的父类 [Overlay](http://aralejs.org/overlay/)。


## 最佳实践

```js
seajs.use(['arale/popup/{{版本号}}/popup'], function(Popup){
    var example = new Popup({
        trigger: '#triggerId',
        element: '#targetId'
    });
});
```

另外，Popup 已从 Overlay 继承了点击页面空白处浮层消失，以及窗口改变大小后浮层重新定位等被动属性，
详细请查看 [演示文档](http://aralejs.org/popup/examples/)。


## 感谢

* Bootstrap Dropdown

