FROM openjdk:7
LABEL maintaner="Udo Meijer (udo.meijer@gmail.com)"

RUN wget -O /tmp/AuditConsole-0.4.6-13-standalone.zip https://auditconsole.com/downloads/auditconsole/0.4.7/AuditConsole-0.4.7.1-1-standalone.zip \
 && unzip /tmp/AuditConsole-0.4.6-13-standalone.zip -d /opt \
 && rm -f /tmp/AuditConsole-0.4.6-13-standalone.zip \
 && chmod 755 /opt/AuditConsole/bin/*.sh

EXPOSE 8080

CMD ["/opt/AuditConsole/bin/catalina.sh", "run"]
