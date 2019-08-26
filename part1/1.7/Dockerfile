FROM ubuntu:18.04

RUN apt-get update && apt-get install -y curl

WORKDIR /script
COPY start.sh .
RUN chmod +x ./start.sh

CMD [ "./start.sh" ]
