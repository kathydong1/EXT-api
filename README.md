Ext.Viewport.add({
    xtype: 'panel',
    html: '<div style="font-size:24px;color:green">Hello World!</div>'
});
Ext.Viewport是一个专门的容器，可以自动调整大小以适应浏览器视口的大小，并方便地管理添加到视口中的组件的大小和位置
   配置项：
       xtype：“xtype”属性的特殊之处在于它表示我们要创建的组件的类型。
       html:html配置非常简单。 html配置的值被添加为我们组件的主要内容。
       
       autoLoad：
    自动加载，实际上你会发现在Ext4.X中这个属性没有多少意义，后面会做解释。
autoSync：
    自动同步，比如我们用普通editingGrid的时候，修改了数据自动保存到store（不是保存到后台）
clearOnLoad：
    在加载之前删除原来的所有子节点，可能在4.X中都会遇到tree第二次加载的时候数据重复，造成混乱，你可以试试这个属性。
clearRemovedOnLoad：
    你加载一个节点的时候，会自动把已经删除的节点记录清除，可以参考getRemovedRecords() 函数
defaultRootId：
    默认的根节点（root）id，这个是在异步加载树种很重要的，就是展开根节点的时候向后台发送请求的参数（稍后讲解）
defaultRootProperty：
    子节点的属性名，用处不大。就是修改什么属性作为子节点解析用的。
fields：
    属性域，跟Ext.data.Store的fields一样使用。
filters：
    过滤器。
folderSort：
    排序，设置为true自动为子节点排序
listeners：
    监听器。定义触发事件。
model：
    跟Ext.data.Store的model一样。
nodeParam：
    节点参数，注意这个是参数名，defaultRootId是参数值。
proxy：
    数据代理。这个跟Ext.data.Store一样。
root：
    根节点，ExtJs的树允许你设置一个默认的根节点，也就是说不加载数据的情况下会显示这个作为基础的节点。通常我们使用这个节点代替treePanel的title。用来标示这棵树的目的。
storeId：store的唯一性标示，便于Ext.data.StoreManager管理，可以参看Ext.data.StoreManager. lookup( String/Object store ) : Ext.data.Store


       
