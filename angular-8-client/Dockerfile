# Stage 1: Build Angular frontend
FROM node:18.10.0-alpine AS frontend-builder

WORKDIR /app

# Copy the entire Angular project
COPY . .

# Install dependencies
RUN npm install
RUN npm install -g @angular/cli

#Environment variables
#ENV  NODE_OPTIONS=--openssl-legacy-provider

# Run the Angular app using the ng serve command
CMD ["ng", "serve", "--port", "8081"]