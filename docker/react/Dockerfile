FROM node 

WORKDIR /app

RUN apt update && \
    apt install git -y

RUN git clone  https://github.com/youssef-of-web/internationalization.git .

RUN npm install

EXPOSE 3000

# CMD [ "npm" , "start" ]

#react with nginx 
#commainter   EXPOSE 3000 et  CMD [ "npm" , "start" ] 
#en mode production 
#add to node as  builder
#FROM node as builder

# RUN npm run build
# FROM nginx:1.21.0-alpine as production
# COPY --from=builder /app/build /usr/share/nginx/html
# EXPOSE 80
# CMD [ "nginx" , "-g" , "daemon off ;"]