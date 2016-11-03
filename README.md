# IE
<h2>兼容IE的各种玩意</h2>
<img src="https://dongeg.github.io/public-images/css-triangle/ie.jpg" />

<h3>1.指定IE解析模式</h3>
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
<h3>2.IE条件判断</h3>
通过IE条件判断来给HTML设置不同的class，然后在CSS中通过给不同的class下的子class设置不同的样式即可实现
```html
<!--[if lt IE 7 ]> <html class="ie6"> <![endif]-->
<!--[if IE 7 ]> <html class="ie7"> <![endif]-->
<!--[if IE 8 ]> <html class="ie8"> <![endif]-->
<!--[if IE 9 ]> <html class="ie9"> <![endif]-->
<!--[if (gt IE 9)|!(IE)]><!--> <html class=""> <!--<![endif]-->

<!--[if lt IE 7]> <html class="lt-ie9 lt-ie8 lt-ie7"> <![endif]-->
<!--[if IE 7]> <html class="lt-ie9 lt-ie8"> <![endif]-->
<!--[if IE 8]> <html class="lt-ie9"> <![endif]-->
<!--[if gt IE 8]><!--> <html class=""> <!--<![endif]-->
```
