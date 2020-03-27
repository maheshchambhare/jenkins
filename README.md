# jenkins
installation and practice

1) install java letest version

link :- https://www.edureka.co/blog/install-jenkins/

2) install apache tomcat

* wget tomcat link
* tar xvf tomcat tar file
* go into tomcat folder
* make changes in /conf/tomcat-user.xml :-
 

 <role rolename="manager-gui"/>
 <role rolename="manager-script"/>
 <role rolename="manager-jmx"/>
 <role rolename="managger-status"/>
 <role rolename="admin-gui"/>
 <role rolename="admin-script"/>
 <user username="***********" password="*****" roles="manager-gui,manager-script,manager-jmx,managger-status,admin-gui,admin-script"/>


* next make changes in two context files
 1) /home/ec2-user/tomcat8/webapps/manager/META-INF/context.xml
 2) /home/ec2-user/tomcat8/webapps/host-manager/META-INF/context.xml
  
* comment this text in above context files
 
  
  <!--  <Valve className="org.apache.catalina.valves.RemoteAddrValve"
         allow="127\.\d+\.\d+\.\d+|::1|0:0:0:0:0:0:0:1" /> -->

* after this restart apache tomcat and run it again

3) download jenkins war file

4) deploy that jenkins war file through tomcat and login


***Refrance yuotube link***

https://www.youtube.com/watch?v=68WNroQBUts

https://www.youtube.com/watch?v=GkyUSSajFEg


