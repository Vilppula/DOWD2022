FROM ubuntu:20.04

EXPOSE 5000

COPY . .

RUN apt update && apt install -y curl
RUN curl -sL https://deb.nodesource.com/setup_14.x | bash
RUN apt install -y nodejs
RUN npm install
RUN npm run build

RUN npm install -g serve

ENTRYPOINT ["serve", "-s", "-l", "5000", "build"]
