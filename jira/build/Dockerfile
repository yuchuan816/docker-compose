FROM cptactionhank/atlassian-jira-software:8.1.0
COPY ./atlassian-agent.jar /opt/atlassian-agent/atlassian-agent.jar
ENV JAVA_OPTS="-javaagent:/opt/atlassian-agent/atlassian-agent.jar"
