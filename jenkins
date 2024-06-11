rm -rf /var/lib/jenkins/workspace/practic-B11
docker run -d -p 9889:80 --name practic-B11 -v src=/var/lib/jenkins/workspace/practic-B11/,dst=/usr/share/nginx/html/ nginx
curl -Is http://localhost:9889 | head -1
echo -n 'http://localhost:9889/index.html' | openssl md5 -hex
docker stop practic-B11
docker rm practic-B11
