FROM jarredsumner/bun:edge

RUN mkdir -p app
WORKDIR /app

COPY ./src/http.js ./http.js

EXPOSE 3000
CMD bun run http.js
