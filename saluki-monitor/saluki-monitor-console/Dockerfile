FROM yingjunjiao/runtime-image:1.0
ENV TZ="Asia/Shanghai"
ENV LANG C.UTF-8
ADD saluki-monitor/saluki-monitor-console/target/saluki-monitor-console-1.5.3-SNAPSHOT.jar /root/app.jar
ADD bin /root/
RUN chmod +x /root/*.sh;mkdir /root/logs
ENV JAVA_OPTS ""
ENV APP_NAME saluki-monitor-web
WORKDIR /root
CMD ["./start.sh"]