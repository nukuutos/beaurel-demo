FROM mongo:5.0

ARG DATABASE_URI
ARG USERNAME
ARG PASSWORD

ENV DATABASE_URI ${DATABASE_URI}
ENV USERNAME ${USERNAME}
ENV PASSWORD ${PASSWORD}

COPY timezones.json .
COPY users.json .

CMD mongoimport --username ${USERNAME} --password ${PASSWORD} --uri ${DATABASE_URI} --collection timezones --drop --file timezones.json --jsonArray && \
    mongoimport --username ${USERNAME} --password ${PASSWORD} --uri ${DATABASE_URI} --collection users --drop --file users.json --jsonArray
