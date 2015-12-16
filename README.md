#Installation steps

1. Install java 7 or higher

        sudo yum install java

2. Import Elasticsearch public GPG key

        sudo rpm --import http://packages.elasticsearch.org/GPG-KEY-elasticsearch

3. Create a repo file for logstash

        touch /etc/yum.repos.d/logstash.repo

4. Fill this file with logstash repo details

        [logstash-2.1]
        name=Logstash repository for 2.1.x packages
        baseurl=http://packages.elastic.co/logstash/2.1/centos
        gpgcheck=1
        gpgkey=http://packages.elastic.co/GPG-KEY-elasticsearch
        enabled=1


