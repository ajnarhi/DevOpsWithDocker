FROM ubuntu:16.04 
WORKDIR /mydir
EXPOSE 8000
COPY . . 
RUN apt-get update && apt-get install -y curl 
RUN curl -sL https://deb.nodesource.com/setup_10.x | bash && apt install -y nodejs
RUN npm install
CMD ["npm","start"]
