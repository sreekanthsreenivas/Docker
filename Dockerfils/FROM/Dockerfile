# Use AlmaLinux as base image
FROM almalinux:8

# Install NGINX
RUN dnf -y install nginx && \
    dnf clean all

# Expose NGINX port
EXPOSE 80

# Copy custom HTML content (optional)
COPY index.html /usr/share/nginx/html/index.html

# Start NGINX service
CMD ["nginx", "-g", "daemon off;"]
