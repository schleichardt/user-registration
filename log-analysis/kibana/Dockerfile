FROM tomcat
MAINTAINER eberhard.wolff@gmail.com
ADD index.html /var/lib/tomcat7/webapps/ROOT/
RUN apt-get install -y wget ; wget https://download.elasticsearch.org/kibana/kibana/kibana-3.1.0.tar.gz ; tar xvzf kibana-3.1.0.tar.gz -C /var/lib/tomcat7/webapps
CMD JAVA_HOME=/usr/lib/jvm/java-7-openjdk-amd64 CATALINA_BASE=/var/lib/tomcat7 CATALINA_HOME=/usr/share/tomcat7 /usr/share/tomcat7/bin/catalina.sh run
EXPOSE 8080