FROM bde2020/spark-base:seafix-3.2.1-hadoop2.7

LABEL maintainer="Gezim Sejdiu <g.sejdiu@gmail.com>, Giannis Mouchakis <gmouchakis@gmail.com>"

COPY master.sh /

COPY hive-site.xml /spark/conf/

ENV SPARK_MASTER_PORT 7077
ENV SPARK_MASTER_WEBUI_PORT 9090
ENV SPARK_MASTER_LOG /spark/logs

EXPOSE 9090 7077 6066

CMD ["/bin/bash", "/master.sh"]
