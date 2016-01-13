FROM ubuntu:latest
MAINTAINER Ivan <ivan@marsudirini-bks.sch.id>

RUN apt-get update && apt-get install -y software-properties-common

RUN apt-get install -y nginx && apt-get clean

EXPOSE 80 443

CMD ["nginx", "-g", "daemon off;"]
