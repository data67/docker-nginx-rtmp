docker build -t 6ack/nginx-rtmp .
docker tag 6ack/nginx-rtmp registry.cn-zhangjiakou.aliyuncs.com/6ack/nginx-rtmp:latest
docker push registry.cn-zhangjiakou.aliyuncs.com/6ack/nginx-rtmp:latest