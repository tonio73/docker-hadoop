FROM bde2020/hadoop-base

LABEL maintainer="Ivan Ermilov <ivan.s.ermilov@gmail.com>"

ENV HDFS_CONF_dfs_datanode_data_dir=file:///hadoop/dfs/data
RUN mkdir -p /hadoop/dfs/data
VOLUME /hadoop/dfs/data

ADD run.sh /run.sh
RUN chmod a+x /run.sh

ENTRYPOINT ["/run.sh"]
