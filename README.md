Ext.Viewport.add({
    xtype: 'panel',
    html: '<div style="font-size:24px;color:green">Hello World!</div>'
});
Ext.Viewport是一个专门的容器，可以自动调整大小以适应浏览器视口的大小，并方便地管理添加到视口中的组件的大小和位置
   配置项：
       xtype：“xtype”属性的特殊之处在于它表示我们要创建的组件的类型。
       html:html配置非常简单。 html配置的值被添加为我们组件的主要内容。
       
