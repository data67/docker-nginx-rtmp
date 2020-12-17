docker build -t 6ack/nginx-rtmp .
docker tag 6ack/nginx-rtmp registry.cn-zhangjiakou.aliyuncs.com/6ack/nginx-rtmp:latest
docker push registry.cn-zhangjiakou.aliyuncs.com/6ack/nginx-rtmp:latest



docker pull registry.cn-zhangjiakou.aliyuncs.com/6ack/nginx-rtmp:latest



docker run -it --rm -p1935:1935 -p8848:80 --mount type=bind,src=/c/var/xc,dst=/opt/athena/share --name nginx-rtmp 6ack/nginx-rtmp