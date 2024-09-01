FROM node:14

WORKDIR /app

COPY . . 

RUN npm install

# ARG vs ENV
# ARG is used to pass build-time variables to the image
# ENV is used to set environment variables in the image; 컨테이너 시작에도 사용됨
ENV COLOR=blue

USER node

EXPOSE 3000

ENTRYPOINT [ "npm" ]

CMD ["start"]