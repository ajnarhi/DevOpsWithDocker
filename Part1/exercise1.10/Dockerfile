FROM ubuntu:16.04 
WORKDIR /mydir
EXPOSE 5000
COPY . . 
RUN apt-get update && apt-get install -y curl 
RUN curl -sL https://deb.nodesource.com/setup_10.x | bash && apt install -y nodejs
RUN npm install
RUN npm install -g serve
RUN npm run build
CMD ["serve","-s","-l","5000","dist"]
