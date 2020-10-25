ARG ELK_VERSION

# https://www.docker.elastic.co/
FROM docker.elastic.co/elasticsearch/elasticsearch:${ELK_VERSION}

# 安装中文分词插件
ARG ELK_VERSION
ADD https://github.com/medcl/elasticsearch-analysis-ik/releases/download/v${ELK_VERSION}/elasticsearch-analysis-ik-${ELK_VERSION}.zip /tmp/
RUN /usr/share/elasticsearch/bin/elasticsearch-plugin install --batch file:///tmp/elasticsearch-analysis-ik-${ELK_VERSION}.zip

RUN rm -rf /tmp/*

# Add your elasticsearch plugins setup here
# Example: RUN elasticsearch-plugin install analysis-icu
