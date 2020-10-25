ARG ELK_VERSION

# https://www.docker.elastic.co/
FROM docker.elastic.co/elasticsearch/elasticsearch:${ELK_VERSION}

# 安装中文分词插件
ADD elasticsearch-analysis-ik-7.9.2 /usr/share/elasticsearch/plugins/elasticsearch-analysis-ik
# Add your elasticsearch plugins setup here
# Example: RUN elasticsearch-plugin install analysis-icu
