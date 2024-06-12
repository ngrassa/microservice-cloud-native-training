git clone https://github.com/ngrassa/microservice-cloud-native-training.git \
cd microservice-cloud-native-training \
cd lab-01
# construction d'un artifact
1- installation maven :\
sudo yum install -y maven \
2- contruction d'un livrable applicatif:\
mvn clean install \
3- déployer le livrable monolith : 
java --jar target/monolitic-1.4.4.RELEASE-exec.jar \
4- test dans le navigateur:\
http://<ip_enp0s8>:8081

# installation du fontend pour consommer le back-end
5-  sudo yum install -y httpd \
6-  sudo copy  test.php /var/www/html/index.html \
7- http://<ip_enp0s8>
