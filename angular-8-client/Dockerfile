# Stage 1: Build Angular frontend
FROM node:14.17.0-alpine AS frontend-builder

WORKDIR /app

# Copy the entire Angular project
COPY . .

# Install dependencies
RUN npm install

# Build the Angular app
RUN npm run build

# Expose the desired port (8081) for the ng serve command
EXPOSE 8081

# Run the Angular app using the ng serve command
CMD ["ng", "serve", "--port", "8081"]
