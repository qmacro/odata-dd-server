# syntax=docker/dockerfile:1

FROM node:24-alpine

LABEL org.opencontainers.image.source=https://github.com/qmacro/odata-dd-server

# Install SAP CAP SDK globally
RUN npm install -g @sap/cds-dk

WORKDIR /
COPY . .

CMD ["cds", "watch", "northbreeze"]
