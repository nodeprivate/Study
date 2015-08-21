module id: ModuleID替代URL地址
	RequireJS以一个相对于baseUrl的地址来加载所有的代码
	页面顶层<script>标签含有一个特殊的属性data-main，require.js使用它来启动脚本加载过程，而baseUrl一般设置到与该属性相一致的目录
	<!--This sets the baseUrl to the "scripts" directory, and
    loads a script that will have a module ID of 'main'-->
	<script data-main="scripts/main.js" src="scripts/require.js"></script>
	
	
	baseUrl亦可通过RequireJS config手动设置。如果没有显式指定config及data-main，则默认的baseUrl为包含RequireJS的那个HTML页面的所属目录。
	
	有时候你想避开"baseUrl + paths"的解析过程，而是直接指定加载某一个目录下的脚本。此时可以这样做：如果一个module ID符合下述规则之一，其ID解析会避开常规的"baseUrl + paths"配置，而是直接将其加载为一个相对于当前HTML文档的脚本：
		以 ".js" 结束.
		以 "/" 开始.
		包含 URL 协议, 如 "http:" or "https:".