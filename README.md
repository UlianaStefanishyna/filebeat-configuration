# Filebeat configuration

1) Change owner of the filebeat.yml to root

2) Install docker container:
 - sudo docker run -d --net=host \
-v /var/volume:/var/volume \
-v /home/core/beatLogs:/home/core/beatLogs \
-v /home/core/filebeat.yml:/usr/share/filebeat/filebeat.yml \
docker.elastic.co/beats/filebeat:6.4.0
