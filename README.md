<p>
JRIA Ӣ��ȫ��Java Reload In-time Agent. ��ʵ��JVM������̬�ű�һ����ʵ�ּ�ʱ�޸ļ�ʱ������Ч���ܣ�ͬʱ����ס��ǰ������״̬���ݵĹ���,ĿǰJRIA��֧��ԭ����Java�����ؼ���ʵ���⣬��֧��Spring2.0.x~2.5.x, Struts.2.x,Hibernate 3.x,Mybatis 3.0.x��Rigel-tcom��ܺ���������ؼ���ʵ�֡� JRIA�˴���Լ�����У���ȫ��Rigel����ܹ�С�鿪����ɡ�<br>
ĿǰJRIA ֧�ֵ�JDK�汾����Sun JDK5.0.x��6.0.x�����汾��Sun JDK7.0.x���ں�������֧�֣�Ŀǰû�����JDK7���в���
</p>

<p>
<pre>
10�벿�𷽰�. JRIA��ʹ�÷ǳ���, ֻ��Ҫ����һ������

��JRIA.jar�ļ����ص����غ󣬽���������ҪJVM�Ĳ����Ͻ�������
����������˵������:
     java -noverify -javaagent:{path}\JRIA.jar
     {path}��ʾJRIA.jar�ļ����ھ���·��.�� D:/JRIA.jar
</pre>
����������ú� JRIA���Զ���classpath�µ�class�ļ���ʱ������м�飬һ�������ʵ��౻����и��£�JRIA��ʵ���Զ����ء�

</p>

<p>
Eclipse��������
<pre>
����1��Eclipse Tomcat �����װ����
![](http://i.imgur.com/zkOqsQU.png)

�� -noverify �� -javaagent:{path}\JRIA.jar ���õ�JVM���������ϼ���

����2: Eclipse Servers�Դ����
����Run(����)������
![](http://i.imgur.com/VO0gXg8.jpg)
</pre>
��װ��ɺ󣬿�������JVM,��������Ч��

![](http://i.imgur.com/zjE4A0n.png)
</p>

<p>
��������
<pre>
JRIA�ṩ��һЩ�������ù���

Package����:
Package�����ṩ�˶�JRIA���ص�class��Ĺ��˹������á�
����������ã��粻����JRIA�������е�class���ж�̬���أ���ô�����ٶȱȽ���������JRIA�ṩ�����¼�������������ʹ��
-Djria.package ��ʾ��Ҫ���ж�̬���ص�class packageǰ׺��jria.exclude_package�����ȼ�Ҫ����jria.package
-Djria.package=com.baidu.rigel��ʾ���com.baidu.rigel ��ǰ׺��class���ж�̬����֧��

-Djria.exclude_package ��ʾ��Ҫ�����ж�̬���ص�class packageǰ׺
-Djria.exclude_package=org.springframework��ʾ���org.springframework ��ǰ׺��class�����ж�̬����֧��

</pre>

</p>