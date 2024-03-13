# Use an official nginx image as a parent image
FROM nginx:latest

# Set the working directory inside the container
WORKDIR /usr/share/nginx/html

# Remove the default nginx static assets
RUN rm -rf ./*

# Copy the static content of your front-end into the container
COPY . .

# Expose port 80 to be accessible from the outside
EXPOSE 80

# Start Nginx and keep it running in the foreground
CMD ["nginx", "-g", "daemon off;"]
