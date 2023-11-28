# VM1-CentOS-Infraestructura
# -->ansible:
#     image: williamyeh/ansible:alpine3
#     volumes:
#      - ./ansible:/ansible
#
# -->jenkins:
#     image: jenkins/jenkins:lts
#     ports:
#      - 8080:8080
#      - 50000:50000
#     volumes:
#      - jenkins_home:/var/jenkins_home
#
# -->sonarqube:
#     image: sonarqube
#     ports:
#      - 9000:9000
#      - 9092:9092
#     volumes:
#      - sonarqube_conf:/opt/sonarqube/conf
#      - sonarqube_data:/opt/sonarqube/data
#      - sonarqube_extensions:/opt/sonarqube/extensions
#      - sonarqube_bundled-plugins:/opt/sonarqube/lib/bundled-plugins
