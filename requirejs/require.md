module id: ModuleID���URL��ַ
	RequireJS��һ�������baseUrl�ĵ�ַ���������еĴ���
	ҳ�涥��<script>��ǩ����һ�����������data-main��require.jsʹ�����������ű����ع��̣���baseUrlһ�����õ����������һ�µ�Ŀ¼
	<!--This sets the baseUrl to the "scripts" directory, and
    loads a script that will have a module ID of 'main'-->
	<script data-main="scripts/main.js" src="scripts/require.js"></script>
	
	
	baseUrl���ͨ��RequireJS config�ֶ����á����û����ʽָ��config��data-main����Ĭ�ϵ�baseUrlΪ����RequireJS���Ǹ�HTMLҳ�������Ŀ¼��
	
	��ʱ������ܿ�"baseUrl + paths"�Ľ������̣�����ֱ��ָ������ĳһ��Ŀ¼�µĽű�����ʱ���������������һ��module ID������������֮һ����ID������ܿ������"baseUrl + paths"���ã�����ֱ�ӽ������Ϊһ������ڵ�ǰHTML�ĵ��Ľű���
		�� ".js" ����.
		�� "/" ��ʼ.
		���� URL Э��, �� "http:" or "https:".