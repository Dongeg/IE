# IE
兼容IE的各种玩意

通用方法

1.指定兼容模式
```html
<meta http-equiv="X-UA-Compatible" content="IE=Edge"> <!--使用当前的最高版本进行文档的解析-->    
```
X-UA-Compatible
```
X-UA-Compatible值	说明
IE=5	             让浏览器使用Quirks mode来显示，实际上是使用Internet Explorer 7 的 Quirks 模式来显示内容，这个模式和IE5非常相似。
IE=edge	           这个设置是让IE使用当前的最高版本进行文档的解析，官方文档指明，edge模式仅适用在测试环境，不建议在生产环境中使用
IE=7	             使用标准IE7来处理
IE=EmulateIE7	     模拟IE7来处理，遵循 指令，如果文档有当前有一个合法的，就使用IE7模式，否者使用Quirks模式（Internet Explorer 5 Quirks），
                   对于大部分网站来说，这是首选的兼容性模式
IE=8	             标准IE8
IE=EmulateIE8	     模拟IE8，遵循 指令，参照IE=EmulateIE7说明
IE=9	             标准IE9
IE=EmulateIE9	     模拟IE9，遵循 指令，参照IE=EmulateIE7说明
chrome=1	         强制使用Chrome，需要IE下Chrome插件支持
IE=EmulateIE10	   模拟IE10
IE=10	             标准IE10，遵循 指令，参照IE=EmulateIE7说明
```
