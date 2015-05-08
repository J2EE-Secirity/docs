
'SecurityExample'
-----------------------------------[ Spring(3.0.5.RELEASE) Security + JBoss-config ]
https://github.com/Home-SignUp/SecurityExample >> http://devcolibri.com/4575
+++++++++++++++++
http://localhost:8081/example/
http://localhost:8081/example/secured/secured1.html
http://localhost:8081/example/secured/secured2.html
http://localhost:8081/example/public/public.html
=============================================================================================================
В этом случае ролевые права доступа настраиваются на самом сервере-приложений JBoss.
Мы имеем какие-либо ресурсы (веб-ресурсы, ресурсы-сервера/файлы, ...).
Исходя из этого, все конфигурационные данные о безопасном доступе приложение берет из сервере-приложений JBoss И далее мы можем попасть на...


'sshwa'
-----------------------------------[ Spring(4) Security + Java(8) ]
https://github.com/Home-Spring/sshwa (https://github.com/elennaro/sshwa/tree/0.2-SNAPSHOT)
+++++++++++++++++
> /opt/tomcat8/tomcat start
http://localhost:8080/sshwa/
http://localhost:8080/sshwa/login >> 'user/user' >> http://localhost:8080/sshwa/helloworld/
http://localhost:8080/sshwa/login?logout
http://localhost:8080/sshwa/login >> 'admin/admin' >> http://localhost:8080/sshwa/protected
http://localhost:8080/sshwa/login?logout
http://localhost:8080/sshwa/login >> 'superadmin/superadmin' >> http://localhost:8080/sshwa/confidential
=============================================================================================================
В этом случае ролевые права доступа настраиваются через классы Spring-Security именно в коде приожения "AppSecurityConfig" (WebSecurityConfigurerAdapter).


'AddressBook'
-----------------------------------[ Spring(3.0.5.RELEASE) Security + XML-config ]
https://github.com/Home-Spring/AddressBook
+++++++++++++++++
http://localhost:8081/AddressBook/list?sort=fio
http://localhost:8081/AddressBook/login.jsp >> user/1111 | admin/pass
=============================================================================================================
В этом случае ролевые права доступа настраиваются через XML-кофигурационные файлы.
src/main/webapp/WEB-INF/web.xml
src/main/webapp/WEB-INF/spring/: 'servlet-context.xml', 'data.xml', 'security.xml', 'appServer/controllers.xml'
(Конфиогурация Spring(а) выполняется полностью черех XML)


'angular_bootstrap_spring'
-----------------------------------[ Spring(4.0.2) Security + AngularJS ]
https://github.com/J2EE-Secirity/angular_bootstrap_spring
+++++++++++++++++
=============================================================================================================
В этом случае пример секюрности-Spring(а) настроен для работы совместно с AngularJS


'spring-security-angular'
-----------------------------------[ Spring(4.0.2) Security + AngularJS ]
https://github.com/J2EE-Secirity/spring-security-angular
+++++++++++++++++
=============================================================================================================
В этом случае имеются разные пример секюрности (basic, oauth2-vanilla, oauth2, proxy, single, spring-session)





(Безопасность в J2EE)
http://www.codenet.ru/webmast/java/j2ee.php
http://javagu.ru/portal/dt?last=false&provider=javaguru&ArticleId=GURU_ARTICLE_81114&SecID=GURU_SECTION_80693
http://habrahabr.ru/post/245415/
https://github.com/Home-Spring/AddressBook-1
https://github.com/Home-SignUp/SecurityExample


(j2ee security example)
http://www.pramati.com/docstore/1270002/index.htm
https://isu.ifmo.ru/docs/IAS904/web.904/b10325/jaas_inb.htm
http://habrahabr.ru/post/137543/
http://devcolibri.com/4575
http://localhost:8091/addressbook/list?sort=fio
http://localhost:8080/sshwa/


