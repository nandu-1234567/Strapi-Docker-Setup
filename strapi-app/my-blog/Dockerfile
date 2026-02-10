FROM node:20

WORKDIR /strapi/app

ENV HOST=0.0.0.0
ENV PORT=1337
ENV APP_KEYS=key1,key2,key3,key4
ENV API_TOKEN_SALT=api_token_salt_123
ENV ADMIN_JWT_SECRET=admin_jwt_secret_123
ENV JWT_SECRET=jwt_secret_123

COPY package*.json ./
RUN npm install

COPY . .

RUN mkdir -p public/uploads

EXPOSE 1337

CMD ["npm", "run", "develop"]
