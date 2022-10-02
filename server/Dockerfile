FROM jarredsumner/bun:edge

ARG port

RUN mkdir -p app
WORKDIR /app

COPY ./src/http.ts ./http.ts

EXPOSE $port
CMD bun run http.ts
