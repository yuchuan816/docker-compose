FROM atlassian/confluence-server:7.11.2
COPY ./atlassian-agent.jar /opt/atlassian-agent/atlassian-agent.jar
COPY ./mysql-connector-java-8.0.24.jar /opt/atlassian/confluence/confluence/WEB-INF/lib
ENV JAVA_OPTS="-javaagent:/opt/atlassian-agent/atlassian-agent.jar"
