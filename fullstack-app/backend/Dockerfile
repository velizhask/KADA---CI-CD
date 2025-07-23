FROM node:18-alpine
WORKDIR /app
COPY . .
RUN npm install
EXPOSE 5000
HEALTHCHECK CMD curl --fail http://localhost:5000 || exit 1
CMD ["node", "index.js"]
