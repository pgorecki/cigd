FROM fr3nd/collectd:latest
RUN curl https://bootstrap.pypa.io/get-pip.py -o get-pip.py && \
    python get-pip.py && \
    ls -la /etc/collectd && \
    mkdir -p /etc/collectd/plugins && \
    cd /etc/collectd/plugins && \
    git clone https://github.com/lebauce/docker-collectd-plugin.git && \
    pwd && ls -la && \
    cd docker-collectd-plugin && \
    pip install -r requirements.txt
