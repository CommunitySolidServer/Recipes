FROM node:lts-alpine AS build
WORKDIR /usr/src/app/
COPY /mashlib/ ./
RUN npm clean-install --omit=dev

FROM solidproject/community-server AS production
COPY --from=build /usr/src/app/node_modules/ /community-server/node_modules/
COPY /mashlib/config* /community-server/config/