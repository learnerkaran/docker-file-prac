FROM ubuntu:latest
LABEL 3tierappem="employeesfrontend"

RUN  apt install -y nodejs npm 
RUN npm install -g n
RUN n 14.17.0
RUN  git clone https://github.com/shubhamkalsait/devops-fullstack-app.git
RUN apt-get clean 
WORKDIR devops-fullstack-app/frontend/
RUN npm install


EXPOSE 3000

CMD ["npm" ,"start"]