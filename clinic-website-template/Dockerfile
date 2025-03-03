# Use an official Nginx image to serve the HTML files
FROM nginx:alpine

# Copy the entire project into the Nginx server
COPY . /usr/share/nginx/html

# Expose the port the app will run on
EXPOSE 80

# Run the Nginx server
CMD ["nginx", "-g", "daemon off;"]
