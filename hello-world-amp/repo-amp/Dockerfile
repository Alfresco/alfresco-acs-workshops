FROM alfresco/alfresco-content-repository-community:${alfresco.repository.version}

COPY target/hello-world-repo-amp-*.amp /usr/local/tomcat/amps/

# Install amps on alfresco repository
RUN java -jar /usr/local/tomcat/alfresco-mmt/alfresco-mmt*.jar install \
              /usr/local/tomcat/amps /usr/local/tomcat/webapps/alfresco -directory -nobackup -force
