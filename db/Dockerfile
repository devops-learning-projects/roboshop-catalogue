FROM          docker.io/redhat/ubi9
COPY          mongo.repo /etc/yum.repos.d/mongo.repo
RUN           dnf install mongodb-mongosh -y
RUN           mkdir /app
COPY          run.sh /app
COPY          *.js /app/
ENTRYPOINT    ["bash", "/app/run.sh"]

