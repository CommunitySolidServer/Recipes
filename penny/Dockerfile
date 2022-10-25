FROM node:lts-alpine AS build
WORKDIR /usr/src/app/
COPY /penny/ ./
RUN npm clean-install --omit=dev

FROM solidproject/community-server AS production
COPY --from=build /usr/src/app/node_modules/ /community-server/node_modules/
COPY /penny/config* /community-server/config/